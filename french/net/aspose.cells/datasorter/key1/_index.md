---
title: "DataSorter.Key1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. Représente l'indice de la première colonne triée, position absolue, la colonne A est 0, B est 1"
type: docs
url: /fr/net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

Représente l'index de la première colonne triée (position absolue, la colonne A vaut 0, B vaut 1, ...).

```csharp
public int Key1 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey1Demo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);

            // Créer un trieur de données et définir Key1 pour trier par la colonne Score (colonne B)
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 1; // Column index 1 (B)
            sorter.Order1 = SortOrder.Descending;

            // Définir la zone de tri (lignes 1-4, toutes les colonnes de données)
            CellArea sortArea = new CellArea();
            sortArea.StartRow = 1;
            sortArea.EndRow = 4;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;

            // Effectuez le tri
            sorter.Sort(cells, sortArea);

            // Enregistrer le résultat
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


