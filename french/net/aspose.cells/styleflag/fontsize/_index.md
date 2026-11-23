---
title: "StyleFlag.FontSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre de taille de police sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/fontsize/
---
## StyleFlag.FontSize property

Le paramètre de taille de police sera appliqué.

```csharp
public bool FontSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Sample Text");

            Style style = workbook.CreateStyle();
            style.Font.Size = 18;
            style.Font.IsBold = true;

            StyleFlag styleFlag = new StyleFlag
            {
                FontSize = true,
                FontBold = true
            };

            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A1");
            range.ApplyStyle(style, styleFlag);

            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


