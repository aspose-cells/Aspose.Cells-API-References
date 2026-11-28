---
title: "Shape.IsDecorative"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape property. Nesnenin dekoratif olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

Nesnenin dekoratif olup olmadığını gösterir.

```csharp
public bool IsDecorative { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsDecorativeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            
            // Şekli dekoratif olarak ayarla
            shape.IsDecorative = true;
            
            // Çalışma kitabını kaydedin
            string outputPath = "ShapeIsDecorativeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Özelliği doğrulamak için çalışma kitabını yeniden yükle
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


