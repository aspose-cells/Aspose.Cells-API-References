---
title: "ColumnCollection.GetColumnByIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ColumnCollection méthode. Obtient l'objet Column par la position dans la liste"
type: docs
url: /fr/net/aspose.cells/columncollection/getcolumnbyindex/
---
## ColumnCollection.GetColumnByIndex method

Obtient le [`Column`](../../column/) objet par la position dans la liste.

```csharp
public Column GetColumnByIndex(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | La position dans la liste. |

### Valeur de retour

Renvoie l'objet colonne.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la colonne A
            worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";

            try
            {
                // Obtenir la référence de la collection de colonnes
                ColumnCollection columns = worksheet.Cells.Columns;

                // Accéder à la colonne à l'index 0 (colonne A) en utilisant GetColumnByIndex
                Column column = columns.GetColumnByIndex(0);

                // Modifier la largeur de la colonne pour démontrer l'accès à la colonne
                column.Width = 25;

                Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


