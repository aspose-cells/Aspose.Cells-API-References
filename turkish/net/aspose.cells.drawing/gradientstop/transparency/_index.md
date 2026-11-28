---
title: "GradientStop.Transparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GradientStop özelliği. Bölgenin şeffaflık derecesini 0.0 opak'tan 1.0 şeffaf'a kadar bir değer olarak döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/gradientstop/transparency/
---
## GradientStop.Transparency property

Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar.

```csharp
public double Transparency { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gradyan doldurma ile bir şekil ekle.
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

            // Gradyan durdurma için renk oluştur.
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;

            // İlk şeffaflıkla bir gradient durak ekle
            gradientFill.GradientStops.Add(0, color, 30);

            // Gradyan durdurmaya eriş.
            GradientStop stop = gradientFill.GradientStops[0];

            // Şeffaflığı göster ve değiştir
            Console.WriteLine("Initial Transparency: " + stop.Transparency);
            stop.Transparency = 0.7;
            Console.WriteLine("Modified Transparency: " + stop.Transparency);

            // Görsel karşılaştırma için başka bir durak ekle
            CellsColor color2 = workbook.CreateCellsColor();
            color2.Color = Color.Green;
            gradientFill.GradientStops.Add(1, color2, 30);

            // Çalışma kitabını kaydedin
            workbook.Save("GradientStopTransparencyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


