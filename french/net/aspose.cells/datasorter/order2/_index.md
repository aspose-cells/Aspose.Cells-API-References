---
title: "DataSorter.Order2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. Représente l'ordre de tri de la deuxième clé"
type: docs
url: /fr/net/aspose.cells/datasorter/order2/
---
## DataSorter.Order2 property

Représente l'ordre de tri de la deuxième clé.

```csharp
public SortOrder Order2 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder2Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            worksheet.Cells["A5"].PutValue("Eve");
            worksheet.Cells["B5"].PutValue(92);

            // Initialiser DataSorter
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.Key1 = 1; // Sort by Score (column B)
            dataSorter.Order1 = SortOrder.Descending;
            dataSorter.Key2 = 0; // Then sort by Name (column A)
            dataSorter.Order2 = SortOrder.Ascending;

            // Définir la zone de tri
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // Effectuez le tri
            dataSorter.Sort(worksheet.Cells, area);

            // Afficher les résultats dans la console
            Console.WriteLine("Sorted Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine($"{worksheet.Cells[i, 0].StringValue}: {worksheet.Cells[i, 1].IntValue}");
            }
        }
    }
}
```

### Voir aussi

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


