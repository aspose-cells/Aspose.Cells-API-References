---
title: "DataSorter.Keys"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. Obtient la liste des clés du trieur de données"
type: docs
url: /fr/net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Obtient la liste des clés du DataSorter.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKeysDemo
    {
        public static void Run()
        {
            // Créer un objet classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Initialiser le trieur de données
            DataSorter sorter = workbook.DataSorter;
            
            // Ajouter une clé de tri pour la colonne A (indice 0)
            sorter.AddKey(0, SortOrder.Ascending);

            // Trier les données
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Démontrer l'utilisation de la propriété Keys
            DataSorterKeyCollection keys = sorter.Keys;
            Console.WriteLine("Sort Keys Information:");
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
            }

            // Enregistrez le classeur
            workbook.Save("DataSorterKeysDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


