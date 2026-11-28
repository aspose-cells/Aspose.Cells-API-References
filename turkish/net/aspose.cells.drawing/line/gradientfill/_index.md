---
title: "Line.GradientFill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Line özelliği. Degrade doldurmayı temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/line/gradientfill/
---
## Line.GradientFill property

Gradyan doldurmayı temsil eder.

```csharp
public GradientFill GradientFill { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;

    public class LinePropertyGradientFillDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // İlk serinin ilk noktasını al
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            try
            {
                // Noktanın Line nesnesine (kenar) eriş
                Line line = point.Border;

                // GradientFill özelliğini oku (yalnızca‑okunur)
                GradientFill gradient = line.GradientFill;

                // Mevcut degrade doldurma ayrıntılarını göster
                Console.WriteLine("Current GradientFill:");
                Console.WriteLine($"  FillType       = {gradient.FillType}");
                Console.WriteLine($"  DirectionType = {gradient.DirectionType}");
                Console.WriteLine($"  Angle          = {gradient.Angle}");

                // Sağlanan yöntemlerle degradeyi değiştir
                // Var olmayan bir üye referansından kaçınmak için varsayılan enum değerine dönüştürme kullan
                gradient.SetGradient(GradientFillType.Linear, 45.0, (GradientDirectionType)0);
                Console.WriteLine("GradientFill after SetGradient:");
                Console.WriteLine($"  Angle = {gradient.Angle}");

                // Çalışma kitabını kaydedin
                workbook.Save("LinePropertyGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [GradientFill](../../gradientfill/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


