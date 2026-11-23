---
title: "Classe AbstractFormulaChangeMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.AbstractFormulaChangeMonitor. Moniteur pour l'utilisateur afin de suivre les changements de formules pendant certaines opérations"
type: docs
url: /fr/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

Permet à l'utilisateur de suivre les modifications des formules pendant certaines opérations.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | L'événement qui sera déclenché lorsque la formule d'une cellule est modifiée. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | L'événement qui sera déclenché lorsque la formule de FormatCondition est modifiée. |

### Remarques

Par exemple, lors de la suppression/insertion d'une plage de cellules, les formules d'autres cellules peuvent être modifiées en raison du décalage des références. Veuillez noter que les méthodes du moniteur peuvent être invoquées plusieurs fois pour un même objet contenant la formule.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassAbstractFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Définissez quelques formules dans les cellules
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // Insérez des lignes qui déclencheront des changements de formules
            worksheet.Cells.InsertRows(0, 2, options);
        }
    }

    public class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        private readonly WorksheetCollection mWorksheets;
        
        public MyFormulaChangeMonitor(WorksheetCollection worksheets)
        {
            mWorksheets = worksheets;
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Formula changed in {mWorksheets[sheetIndex].Name}!{CellsHelper.CellIndexToName(rowIndex, columnIndex)}");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


