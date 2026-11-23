---
title: "Workbook.DataSorter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient un objet DataSorter pour trier les données"
type: docs
url: /fr/net/aspose.cells/workbook/datasorter/
---
## Workbook.DataSorter property

Obtient un objet DataSorter pour trier les données.

```csharp
public DataSorter DataSorter { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataSorterDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple
            ws.Cells["A1"].PutValue("Name");
            ws.Cells["B1"].PutValue("Age");
            ws.Cells["C1"].PutValue("Score");
            
            ws.Cells["A2"].PutValue("John");
            ws.Cells["B2"].PutValue(25);
            ws.Cells["C2"].PutValue(85);
            
            ws.Cells["A3"].PutValue("Alice");
            ws.Cells["B3"].PutValue(30);
            ws.Cells["C3"].PutValue(92);
            
            ws.Cells["A4"].PutValue("Bob");
            ws.Cells["B4"].PutValue(22);
            ws.Cells["C4"].PutValue(78);

            // Configurer DataSorter
            wb.DataSorter.Order1 = SortOrder.Ascending;
            wb.DataSorter.Key1 = ws.Cells["C1"].Column; // Sort by Score
            
            // Définir la plage de tri
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 2;

            // Effectuez le tri
            wb.DataSorter.Sort(ws.Cells, area);

            // Afficher les données triées
            Console.WriteLine("Sorted Data:");
            for (int row = 0; row <= 4; row++)
            {
                Console.WriteLine($"{ws.Cells[row, 0].StringValue}, {ws.Cells[row, 1].IntValue}, {ws.Cells[row, 2].IntValue}");
            }
        }
    }
}
```

### Voir aussi

* class [DataSorter](../../datasorter/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


