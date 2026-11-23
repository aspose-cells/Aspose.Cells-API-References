---
title: "DeleteBlankOptions.StartIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DeleteBlankOptions. Spécifie l'index de ligne/colonne de départ de la plage à vérifier et à supprimer les lignes/colonnes vides"
type: docs
url: /fr/net/aspose.cells/deleteblankoptions/startindex/
---
## DeleteBlankOptions.StartIndex property

Spécifie l'index de début de ligne/colonne de la plage à vérifier et à supprimer les lignes/colonnes vides.

```csharp
public int StartIndex { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyStartIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplissez certaines cellules avec des valeurs
            cells[2, 0].PutValue("Row 3");
            cells[5, 0].PutValue("Row 6");
            cells[9, 0].PutValue("Row 10");

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i <= 10; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }

            // Supprimer les lignes vides à partir de l'index 4 (Ligne 5) jusqu'à l'index 7 (Ligne 8)
            DeleteBlankOptions options = new DeleteBlankOptions();
            options.StartIndex = 4;
            options.EndIndex = 7;
            cells.DeleteBlankRows(options);

            Console.WriteLine("\nAfter deleting blank rows from Row 5 to Row 8:");
            for (int i = 0; i <= 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }
        }
    }
}
```

### Voir aussi

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


