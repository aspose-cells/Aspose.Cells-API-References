---
title: "RowCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode RowCollection. Supprime l'élément de ligne à la position d'index spécifiée dans cette collection"
type: docs
url: /fr/net/aspose.cells/rowcollection/removeat/
---
## RowCollection.RemoveAt method

Supprime l'élément de ligne à l'index (position) spécifié dans cette collection.

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| index | Int32 | Index basé sur zéro (position, pas [`Index`](../../row/index/)) de l'élément de ligne existant dans cette collection. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données aux cellules des premières lignes
            worksheet.Cells["A1"].PutValue("Row 1");
            worksheet.Cells["A2"].PutValue("Row 2");
            worksheet.Cells["A3"].PutValue("Row 3");
            worksheet.Cells["A4"].PutValue("Row 4");

            // Affichez le nombre initial de lignes
            Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");

            try
            {
                // Appelez la méthode RemoveAt pour supprimer la ligne à l'index 1 (deuxième ligne)
                worksheet.Cells.Rows.RemoveAt(1);

                Console.WriteLine("Method executed successfully. Row at index 1 removed.");

                // Affichez le nombre de lignes mis à jour
                Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");

                // Montrez l'effet - la ligne 2 doit être supprimée, la ligne 3 devient la ligne 2
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


