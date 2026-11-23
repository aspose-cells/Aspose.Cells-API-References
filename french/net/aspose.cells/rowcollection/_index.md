---
title: "Classe RowCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.RowCollection classe. Collecte les objets Row qui représentent les lignes individuelles dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/rowcollection/
---
## RowCollection class

Collecte les objets [`Row`](../row/) qui représentent les lignes individuelles dans une feuille de calcul.

```csharp
public class RowCollection : IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Obtient le nombre de lignes dans cette collection. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Obtient un objet [`Row`](../row/) par l'index de ligne donné. L'objet Row de l'index de ligne donné sera instancié s'il n'existe pas auparavant. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Effacer toutes les lignes et cellules. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Obtient un énumérateur qui parcourt les lignes de cette collection |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Obtient un énumérateur qui parcourt les lignes de cette collection |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Obtient l'objet ligne par sa position dans la liste. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Supprime l'élément de ligne à l'index (position) spécifié dans cette collection. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionDemo
    {
        public static void RowCollectionExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Obtention de la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // Obtenir la collection Rows
            RowCollection rows = worksheet.Cells.Rows;

            // Obtenir le nombre de lignes dans la collection
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // Obtenir la première ligne
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // Parcourir les lignes en utilisant GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // Obtenir une ligne par index
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // Effacer toutes les lignes et cellules
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // Enregistrez le classeur
            workbook.Save("RowCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


