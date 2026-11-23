---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractFormulaChangeMonitor. L'événement qui sera déclenché lorsque la formule d'une cellule est modifiée"
type: docs
url: /fr/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

L'événement qui sera déclenché lorsque la formule d'une cellule est modifiée.

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | L'index de la feuille de la cellule modifiée |
| rowIndex | Int32 | L'index de la ligne de la cellule modifiée |
| columnIndex | Int32 | L'index de la colonne de la cellule modifiée |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de notre classe de démonstration qui hérite de AbstractFormulaChangeMonitor
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // Définir une formule dans une cellule pour déclencher le changement
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // Appeler OnCellFormulaChanged avec l'index de feuille 0, ligne 0, colonne 0 (A1)
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // Implémentation pour gérer le changement de formule
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### Voir aussi

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


