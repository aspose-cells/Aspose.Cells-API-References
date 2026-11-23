---
title: "StyleFlag.Indent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre de niveau d'indentation sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/indent/
---
## StyleFlag.Indent property

Le paramètre de niveau d'indentation sera appliqué.

```csharp
public bool Indent { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyIndentDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style avec un niveau d'indentation
            Style style = workbook.CreateStyle();
            style.IndentLevel = 2;
            style.HorizontalAlignment = TextAlignmentType.Left;

            // Créer un indicateur de style avec la propriété Indent définie
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Indent = true;

            // Appliquer des données aux cellules
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                }
            }

            // Appliquer le style avec l'indentation à une plage
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 5, 5);
            range.ApplyStyle(style, styleFlag);

            // Vérifier que le style a été appliqué
            Cell cell = worksheet.Cells["A1"];
            Style appliedStyle = cell.GetStyle();
            Console.WriteLine($"Indent Level: {appliedStyle.IndentLevel}");
            Console.WriteLine($"Alignment: {appliedStyle.HorizontalAlignment}");

            // Enregistrez le classeur
            workbook.Save("IndentStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


