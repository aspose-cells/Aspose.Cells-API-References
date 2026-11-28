---
title: "FillFormat.FillType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. Doldurma tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Dolgu tipini alır ve ayarlar.

```csharp
public FillType FillType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Renkli katı doldurma ayarlayın
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Red;

            // Doldurma tipini çıktı olarak alın
            Console.WriteLine("Shape fill type: " + shape.Fill.FillType);

            // Gradyan doldurmaya değiştirin
            shape.Fill.FillType = FillType.Gradient;
            Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);

            // Çalışma kitabını kaydedin
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


