---
title: "Enum GradientColorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GradientColorType enum. Belirtilen doldurma için gradyan renk tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Belirtilen dolgu için degrade renk türünü temsil eder.

```csharp
public enum GradientColorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Gradyan renk yok |
| OneColor | `1` | Tek gradyan renk |
| PresetColors | `2` | Önceden ayarlanmış gradyan renkler |
| TwoColors | `3` | İki degrade rengi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Degrade doldurmayı göstermek için bir şekil ekleyin
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // Degrade doldurma tipini ayarlayın
                fill.FillType = FillType.Gradient;

                // Farklı GradientColorType enum değerlerini gösterin
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // Mevcut degrade renk tipini okuyun ve görüntüleyin (özellik yalnızca okunur)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // Çalışma kitabını kaydedin
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


