---
title: "WorksheetCollection.CreateRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Crée un objet Range à partir d'une adresse de la plage"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Crée un objet [`Range`](../../range/) à partir d'une adresse de la plage.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| address | String | L'adresse de la plage. |
| sheetIndex | Int32 | L'index de la feuille. |

### Valeur de retour

Un objet [`Range`](../../range/)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 6; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Créer une plage en utilisant une adresse sous forme de chaîne et l'index de la feuille
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);

            // Démontrer l'utilisation de la plage
            Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
            Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
            Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


