---
title: "DataSorter.Key3"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. Représente l'index de la troisième colonne triée, position absolue, la colonne A est 0, B est 1"
type: docs
url: /fr/net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Représente l'index de la troisième colonne triée (position absolue, la colonne A vaut 0, B vaut 1, ...).

```csharp
public int Key3 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey3Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["C1"].PutValue("Grade");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["C2"].PutValue("B");
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["C3"].PutValue("A");
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);
            cells["C4"].PutValue("C");
            cells["A5"].PutValue("Eve");
            cells["B5"].PutValue(92);
            cells["C5"].PutValue("A");

            // Créer un trieur de données
            DataSorter sorter = workbook.DataSorter;
            
            // Trier par Score (décroissant), puis par Nom (croissant), puis par Note (décroissant)
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Column B (Score)
            
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 0; // Column A (Name)
            
            sorter.Order3 = SortOrder.Descending;
            sorter.Key3 = 2; // Column C (Grade)
            
            // Trier la plage de données
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));

            // Enregistrez le classeur
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


