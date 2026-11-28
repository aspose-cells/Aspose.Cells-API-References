---
title: "PatternFill.ForeTransparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PatternFill özelliği. Ön plan renginin şeffaflığını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Ön plan renginin şeffaflığını alır veya ayarlar.

```csharp
public double ForeTransparency { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Desen doldurmayı göstermek için bir dikdörtgen şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Doldurma tipini desene ayarlayın
            shape.Fill.FillType = FillType.Pattern;

            // PatternFill örneğini alın
            PatternFill patternFill = shape.Fill.PatternFill;

            // Desen doldurma özelliklerini yapılandırın
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // İlk ForeTransparency değerini gösterin
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // Yeni ForeTransparency değerini ayarlayın (%50 şeffaflık)
                patternFill.ForeTransparency = 0.5;

                // Güncellenmiş ForeTransparency değerini gösterin
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // Çalışma kitabını kaydedin
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


