---
title: "Shape.GetActualBox"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Dönme, çevirme vb. uygulandıktan sonra şeklin gerçek konumunu ve boyutunu al"
type: docs
url: /tr/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

Şeklin gerçek konumunu ve boyutunu al (dönme, çevirme vb. uygulandıktan sonra).

```csharp
public float[] GetActualBox()
```

### Dönüş Değeri

Pozisyonu ve boyutu x, y, w, h sırasıyla döndürür

### Açıklamalar

Not: Arayüz tam olarak işlevsel değil, özellikle konum bilgileri doğru değil. İşlev tamamlanana kadar bu arayüzü kullanmamanız önerilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // Şeklin gerçek kutu boyutlarını al
            float[] box = rectangle.GetActualBox();

            // Kutu boyutlarını çıktıya ver
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


