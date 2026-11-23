---
title: "DataSorterKey.Index"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorterKey. Obtient l'index de colonne triée, position absolue (colonne A = 0, B = 1)"
type: docs
url: /fr/net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

Obtient l'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...).

```csharp
public int Index { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIndexDemo
    {
        public static void Run()
        {
            // Créer un objet classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à trier
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Créer un trieur de données et ajouter une clé de tri
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Trier les données
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Démontrer l'utilisation de la propriété Index
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Column index being sorted: {key.Index}");
            }

            // Enregistrer le résultat
            workbook.Save("DataSorterKeyExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


