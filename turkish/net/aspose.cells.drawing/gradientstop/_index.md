---
title: "GradientStop sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GradientStop sınıfı. Gradyan durak noktasını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Gradyan durak noktasını temsil eder.

```csharp
public class GradientStop
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Bu gradyan durak noktasının rengini alır. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | Durdurma noktasının konumu. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Gradyan doldurma ile bir şekil ekle.
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // Gradyan durdurma için renk oluştur.
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // Gradyan durdurma ekle.
                gradientFill.GradientStops.Add(0, color, 30);

                // Gradyan durdurmaya eriş.
                GradientStop stop = gradientFill.GradientStops[0];

                // Temel işlevselliği gösterin
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // Özellikleri değiştir.
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // Çalışma kitabını kaydedin
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


