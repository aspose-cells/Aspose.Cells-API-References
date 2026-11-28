---
title: "Sınıf CellsColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellsColor sınıfı. Tüm renk türlerini temsil eder"
type: docs
url: /tr/net/aspose.cells/cellscolor/
---
## CellsColor class

Tüm renk türlerini temsil eder.

```csharp
public class CellsColor
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | 32 bitlik ARGB değerinden rengi alır ve ayarlar. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | RGB rengi alır ve ayarlar. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | Renk paletindeki renk indeksini alır ve ayarlar. Yalnızca indeksli renkler için geçerlidir. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | Hücreye veya şekle uygulanacak rengi alır ve ayarlar. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | Tema rengini alır. Yalnızca tema rengi türü için geçerlidir. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | Şeffaflığı 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır ve ayarlar. |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | Renk türü. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | Şekil renginin tonunu ayarla |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorDemo
    {
        public static void CellsColorExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücre aralığı oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // Bir CellsColor örneği oluştur
            CellsColor cellsColor = workbook.CreateCellsColor();

            // CellsColor özelliklerini ayarla
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // CellsColor'ı aralığa uygula
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Çalışma kitabını kaydedin
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


