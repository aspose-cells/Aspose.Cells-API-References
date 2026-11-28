---
title: "GradientStop.CellsColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GradientStop özelliği. Bu gradient durakının rengini alır"
type: docs
url: /tr/net/aspose.cells.drawing/gradientstop/cellscolor/
---
## GradientStop.CellsColor property

Bu gradyan durak noktasının rengini alır.

```csharp
public CellsColor CellsColor { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyCellsColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
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

                // Gradient durakına eriş ve CellsColor özelliklerini göster
                GradientStop stop = gradientFill.GradientStops[0];
                CellsColor stopColor = stop.CellsColor;

                Console.WriteLine("Gradient Stop CellsColor Properties:");
                Console.WriteLine("Color Type: " + stopColor.Type);
                Console.WriteLine("RGB Color: " + stopColor.Color);
                Console.WriteLine("ARGB Value: " + stopColor.Argb);
                Console.WriteLine("Transparency: " + stopColor.Transparency);

                // Çalışma kitabını kaydedin
                workbook.Save("GradientStopCellsColorDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


