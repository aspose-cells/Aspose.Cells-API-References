---
title: "DataSorter.Key2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. Représente l'index de la deuxième colonne triée, position absolue : la colonne A est 0, B est 1"
type: docs
url: /fr/net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Représente l'index de la deuxième colonne triée (position absolue, la colonne A vaut 0, B vaut 1, ...).

```csharp
public int Key2 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey2Demo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Créer DataSorter et définir les propriétés
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.Key1 = 0; // Sort by first column (Name)
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key2 = 1; // Then sort by second column (Age)
            sorter.Order2 = SortOrder.Descending;

            // Trier la plage de données
            sorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Afficher les données triées pour démontrer l'utilisation de Key2
            Console.WriteLine("Sorted Data:");
            for (int i = 0; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[i, 0].StringValue} - {worksheet.Cells[i, 1].IntValue}");
            }
        }
    }
}
```

### Voir aussi

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


