---
title: "Cells.Rows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient la collection d'objets Row qui représente les lignes individuelles de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/rows/
---
## Cells.Rows property

Obtient la collection d'objets [`Row`](../../row/) qui représente les lignes individuelles de cette feuille de calcul.

```csharp
public RowCollection Rows { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRowsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la largeur de la colonne et la hauteur de la ligne
            worksheet.Cells.SetColumnWidthPixel(0, 200);
            worksheet.Cells.Rows[0].Height = 50;
            
            // Accédez aux propriétés des lignes via la collection Rows
            Row row = worksheet.Cells.Rows[0];
            Console.WriteLine($"Row 0 height: {row.Height}");
            Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
            
            // Modifier les propriétés des lignes
            row.IsHeightMatched = true;
            row.Height = 60;
            
            // Vérifier les modifications
            Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
            Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
            
            // Enregistrez le classeur
            workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


