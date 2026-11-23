---
title: "DeleteOptions.FormulaChangeMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DeleteOptions. Obtient/definit le moniteur pour suivre les changements causés par la suppression"
type: docs
url: /fr/net/aspose.cells/deleteoptions/formulachangemonitor/
---
## DeleteOptions.FormulaChangeMonitor property

Obtient/définit le moniteur pour suivre les modifications causées par la suppression.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Configurer les données de test
            cells["A1"].Formula = "=A5";
            cells["A5"].Value = 10;
            
            // Ajouter une mise en forme conditionnelle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.Add(CellArea.CreateCellArea(0, 3, 1, 4), FormatConditionType.Expression,
                OperatorType.Equal, "=A8>0", "");

            // Créer et assigner le moniteur
            CustomFormulaChangeMonitor monitor = new CustomFormulaChangeMonitor();
            DeleteOptions options = new DeleteOptions
            {
                FormulaChangeMonitor = monitor,
                UpdateReference = true
            };

            // Supprimer la ligne qui devrait déclencher des changements de formule
            cells.DeleteRows(2, 1, options);

            // Afficher les résultats de la surveillance
            Console.WriteLine("Cell formula changes detected: " + monitor.CellChangesDetected);
            Console.WriteLine("Format condition changes detected: " + monitor.FormatConditionChangesDetected);
        }
    }

    public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        public bool CellChangesDetected { get; private set; }
        public bool FormatConditionChangesDetected { get; private set; }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            CellChangesDetected = true;
            Console.WriteLine($"Cell formula changed at Sheet {sheetIndex}, Row {rowIndex}, Column {columnIndex}");
        }

        public override void OnFormatConditionFormulaChanged(FormatCondition fc)
        {
            FormatConditionChangesDetected = true;
            Console.WriteLine("Format condition formula changed");
        }
    }
}
```

### Voir aussi

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


