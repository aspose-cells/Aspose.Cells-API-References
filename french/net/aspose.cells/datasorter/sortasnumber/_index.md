---
title: "DataSorter.SortAsNumber"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. Indique si le tri concerne tout ce qui ressemble à un nombre"
type: docs
url: /fr/net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

Indique si le tri considère tout ce qui ressemble à un nombre.

```csharp
public bool SortAsNumber { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortAsNumberDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des nombres mixtes et des nombres sous forme de texte
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Créer une zone de cellules à trier
            CellArea ca = CellArea.CreateCellArea("A1", "A4");

            // Créer un trieur de données
            DataSorter sorter = workbook.DataSorter;
            int idx = CellsHelper.ColumnNameToIndex("A");

            // Ajouter une clé de tri (colonne A)
            sorter.AddKey(idx, SortOrder.Ascending);

            // Trier comme nombres (true) ou chaînes (false)
            sorter.SortAsNumber = true;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("Sorted as numbers:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Réinitialiser les données pour le deuxième tri
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Trier comme chaînes
            sorter.SortAsNumber = false;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("\nSorted as strings:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Voir aussi

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


