---
title: "Sınıf GradientFill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GradientFill sınıfı. Degrade dolguyu temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/gradientfill/
---
## GradientFill class

Gradyan doldurmayı temsil eder.

```csharp
public class GradientFill : Fill
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | Doğrusal dolgunun açısı. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | Degrade yön türünü alır. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | Degrade dolgu türünü alır. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | Gradyan durak noktası koleksiyonunu temsil eder. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Şuradan [`Fill`](../fill/) devralınmıştır.) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Karma kodu alır. (Şuradan [`Fill`](../fill/) devralınmıştır.) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | Degrade dolgu türünü ve yönünü ayarlayın. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | Belirtilen dolguyu tek renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | Önceden ayarlanmış tema degrade dolgusunu ayarlar. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassGradientFillDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına tüm gerekli parametrelerle bir dikdörtgen şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);

            // Degrade dolgu özelliklerine erişmek için dolgu tipini degrade olarak ayarlayın
            shape.Fill.FillType = FillType.Gradient;

            // Şekilden mevcut degrade dolgu örneğini alın
            GradientFill gradientFill = shape.Fill.GradientFill;

            // Mevcut örneği kullanarak degradeyi iki renk ile yapılandırın
            gradientFill.SetTwoColorGradient(
                Color.LightSkyBlue,  // First color
                Color.DarkBlue,      // Second color
                GradientStyleType.Horizontal, // Gradient style
                1                    // Variant
            );

            // Çalışma kitabını kaydedin
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


