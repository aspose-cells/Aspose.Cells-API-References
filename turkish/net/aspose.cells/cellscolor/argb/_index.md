---
title: "CellsColor.Argb"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsColor özelliği. Rengi 32 bitlik ARGB değerinden alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

32 bitlik ARGB değerinden rengi alır ve ayarlar.

```csharp
public int Argb { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyArgbDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralık ve stil oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
            Style style = workbook.CreateStyle();

            // Argb özelliğini kullanarak CellsColor oluşturun ve yapılandırın
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue

            // Rengi stile uygulayın
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            
            // Stili aralığa uygulayın
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Çalışma kitabını kaydedin
            workbook.Save("CellsColorArgbDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


