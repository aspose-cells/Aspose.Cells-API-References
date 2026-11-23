---
title: "StyleFlag.Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "StyleFlag propriété. Les paramètres de police seront appliqués"
type: docs
url: /fr/net/aspose.cells/styleflag/font/
---
## StyleFlag.Font property

Les paramètres de police seront appliqués.

```csharp
public bool Font { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var shape = workbook.Worksheets[0].Shapes.AddButton(0, 0, 100, 100, 100, 100);
            shape.Text = "Sample Text";
            
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.Name = "Arial";
            font.Size = 14;
            font.Color = Color.Blue;
            font.IsBold = true;
            
            StyleFlag flag = new StyleFlag();
            flag.Font = true;
            
            shape.FormatCharacters(0, shape.Text.Length, font, flag);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


