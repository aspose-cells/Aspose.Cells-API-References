---
title: "PatternFill.ForegroundCellsColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PatternFill özelliği. Ön plan CellsColor nesnesini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

Ön plan [`CellsColor`](../../../aspose.cells/cellscolor/) nesnesini alır ve ayarlar.

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Desen doldurmayı göstermek için bir dikdörtgen şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // Doldurma tipini desene ayarlayın
                shape.Fill.FillType = FillType.Pattern;

                // PatternFill örneğini alın
                PatternFill patternFill = shape.Fill.PatternFill;

                // Desen tipini ve renkleri ayarlayın
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // Color özelliğini kullanarak ön plan için bir CellsColor nesnesi oluşturun
                // CellsColor'ın genel bir yapıcı metodu olmadığından, mevcut ForegroundCellsColor'ı kullanacağız
                // ve özelliklerini doğrudan değiştirin
                patternFill.ForegroundCellsColor.Color = Color.Blue;
                patternFill.ForegroundCellsColor.Argb = Color.Blue.ToArgb();

                // ForegroundCellsColor özelliklerini gösterin
                Console.WriteLine("ForegroundCellsColor Type: " + patternFill.ForegroundCellsColor.Type);
                Console.WriteLine("ForegroundCellsColor Color: " + patternFill.ForegroundCellsColor.Color);
                Console.WriteLine("ForegroundCellsColor ARGB: " + patternFill.ForegroundCellsColor.Argb);

                // Çalışma kitabını kaydedin
                workbook.Save("ForegroundCellsColorDemo.xlsx");
                Console.WriteLine("ForegroundCellsColor demonstration completed successfully.");
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
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


