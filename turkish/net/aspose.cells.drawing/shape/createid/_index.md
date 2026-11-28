---
title: "Shape.CreateId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bu şekil için oluşturma kimliğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

Bu şekil için oluşturma kimliğini alır ve ayarlar.

```csharp
public Guid CreateId { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCreateIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
            
            // Yeni bir GUID oluştur ve CreateId olarak ata
            Guid createId = Guid.NewGuid();
            shape.CreateId = createId;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShapeCreateIdDemo.xlsx");
            
            // CreateId'in kalıcı olduğunu doğrulamak için çalışma kitabını yeniden yükle
            Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Doğrulama için CreateId'i çıktılayın
            Console.WriteLine("Original CreateId: " + createId);
            Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


