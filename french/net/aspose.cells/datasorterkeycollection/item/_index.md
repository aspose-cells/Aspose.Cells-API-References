---
title: "DataSorterKeyCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorterKeyCollection. Obtient et définit DataSorterKey par indice"
type: docs
url: /fr/net/aspose.cells/datasorterkeycollection/item/
---
## DataSorterKeyCollection indexer

Obtient et définit [`DataSorterKey`](../../datasorterkey/) par indice.

```csharp
public DataSorterKey this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class DataSorterKeyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["B4"].PutValue(78);

            // Créer un objet liste (table)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Ajouter une clé de tri (trier par la colonne Score en ordre décroissant)
            table.AutoFilter.Sorter.AddKey(1, SortOrder.Descending);
            table.AutoFilter.Sorter.Sort();

            // Démontrer l'utilisation de la propriété Item
            DataSorterKey key = table.AutoFilter.Sorter.Keys[0];
            Console.WriteLine("Sort Key Index: {0}, Order: {1}", key.Index, key.Order);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


