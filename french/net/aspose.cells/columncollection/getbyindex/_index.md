---
title: "ColumnCollection.GetByIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ColumnCollection méthode. Obtient l'objet colonne par l'indice"
type: docs
url: /fr/net/aspose.cells/columncollection/getbyindex/
---
## ColumnCollection.GetByIndex method

Obtient l'objet colonne par l'indice.

```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 |  |

### Valeur de retour

Renvoie l'objet colonne.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Columns.GetColumnByIndex(). Cette propriété sera supprimée 12 mois plus tard à compter de juin 2010. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des colonnes dans la collection en définissant les largeurs
            worksheet.Cells.Columns[0].Width = 15;  // Column 0
            worksheet.Cells.Columns[2].Width = 20;  // Column 2
            worksheet.Cells.Columns[4].Width = 25;  // Column 4

            try
            {
                // Obtenir la deuxième colonne de ColumnCollection (index 1)
                Column column = worksheet.Cells.Columns.GetByIndex(1);

                Console.WriteLine($"Retrieved column at collection index 1");
                Console.WriteLine($"Worksheet column index: {column.Index}");
                Console.WriteLine($"Original width: {column.Width}");

                // Modifier la colonne récupérée
                column.Width = 35;
                Console.WriteLine($"Updated width: {column.Width}");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ColumnCollectionGetByIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


