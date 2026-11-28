---
title: "Shape.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bu şeklin tanımlayıcısını alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/id/
---
## Shape.Id property

Bu şeklin tanımlayıcısını alır.

```csharp
public int Id { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Şeklin kimliğini al ve göster
            int id = shape.Id;
            Console.WriteLine("Shape ID: " + id);

            // Şeklin özelliklerini değiştir
            shape.Name = "Rectangle1";
            shape.Text = "Shape with ID: " + id;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePropertyIdDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


