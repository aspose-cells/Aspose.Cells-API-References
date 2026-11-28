---
title: "Sınıf PatternFill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.PatternFill sınıfı. Desen dolgu biçimini temsil eden nesneyi kapsüller."
type: docs
url: /tr/net/aspose.cells.drawing/patternfill/
---
## PatternFill class

Desen dolgu biçimini temsil eden nesneyi kapsüller.

```csharp
public class PatternFill : Fill
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundCellsColor](../../aspose.cells.drawing/patternfill/backgroundcellscolor/) { get; set; } | Ön plan [`CellsColor`](../../aspose.cells/cellscolor/) nesnesini alır ve ayarlar. |
| [BackgroundColor](../../aspose.cells.drawing/patternfill/backgroundcolor/) { get; set; } | Arka plan [`Area`](../area/) rengini alır veya ayarlar. |
| [BackTransparency](../../aspose.cells.drawing/patternfill/backtransparency/) { get; set; } | Arka plan renginin şeffaflığını alır veya ayarlar. |
| [ForegroundCellsColor](../../aspose.cells.drawing/patternfill/foregroundcellscolor/) { get; set; } | Ön plan [`CellsColor`](../../aspose.cells/cellscolor/) nesnesini alır ve ayarlar. |
| [ForegroundColor](../../aspose.cells.drawing/patternfill/foregroundcolor/) { get; set; } | Ön plan rengini alır veya ayarlar. |
| [ForeTransparency](../../aspose.cells.drawing/patternfill/foretransparency/) { get; set; } | Ön plan renginin şeffaflığını alır veya ayarlar. |
| [Pattern](../../aspose.cells.drawing/patternfill/pattern/) { get; set; } | Dolgu deseni tipini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Şuradan [`Fill`](../fill/) devralınmıştır.) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Karma kodu alır. (Şuradan [`Fill`](../fill/) devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassPatternFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Arka plan tipi deseni kullanarak hücre için stil oluştur.
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.DiagonalStripe;
            style.ForegroundColor = Color.LightBlue;
            style.BackgroundColor = Color.DarkBlue;

            worksheet.Cells["B2"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("PatternFill Demo");

            // Şekil oluştur ve desen dolgusunu yapılandır
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 100);
            shape.Fill.FillType = FillType.Pattern;
            
            PatternFill shapePatternFill = shape.Fill.PatternFill;
            shapePatternFill.Pattern = FillPattern.DiagonalBrick;
            shapePatternFill.ForegroundColor = Color.LightBlue;
            shapePatternFill.BackgroundColor = Color.DarkBlue;
            shapePatternFill.ForeTransparency = 0.2;
            shapePatternFill.BackTransparency = 0.3;

            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Color = Color.Gold;
            shapePatternFill.ForegroundCellsColor = cellsColor;

            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


