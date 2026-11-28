---
title: "FillFormat.SolidFill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. SolidFill nesnesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

`SolidFill` nesnesini alır.

```csharp
public SolidFill SolidFill { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertySolidFillDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Şekil için katı dolgu rengini ayarla
            shape.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(135, 222, 255);
            
            // Katı dolgu rengini al ve göster
            System.Drawing.Color fillColor = shape.Fill.SolidFill.Color;
            Console.WriteLine("Solid Fill Color - R:{0}, G:{1}, B:{2}", 
                fillColor.R, fillColor.G, fillColor.B);
            
            // Çalışma kitabını kaydedin
            workbook.Save("SolidFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


