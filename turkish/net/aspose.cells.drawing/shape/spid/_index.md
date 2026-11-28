---
title: "Shape.Spid"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bir uygulamanın belirli şekli tanımlamak için kullanabileceği isteğe bağlı bir dize tanımlayıcısını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/spid/
---
## Shape.Spid property

Bir uygulamanın belirli şekli tanımlamak için kullanabileceği isteğe bağlı bir dize tanımlayıcısını belirtir.

```csharp
public string Spid { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySpidDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle çalışma sayfasına bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Şeklin Spid özelliğini al ve göster
            string spid = shape.Spid;
            Console.WriteLine("Shape SPID: " + spid);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePropertySpidDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


