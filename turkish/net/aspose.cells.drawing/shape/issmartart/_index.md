---
title: "Shape.IsSmartArt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin smart art olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/issmartart/
---
## Shape.IsSmartArt property

Şeklin akıllı sanat olup olmadığını gösterir.

```csharp
public bool IsSmartArt { get; }
```

### Açıklamalar

Yalnızca ooxml dosyası için.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsSmartArtDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir SmartArt şekli ekle (Not: Aspose.Cells mevcut sürümlerde SmartArt oluşturmayı doğrudan sunmaz)
            // Demonstrasyon için mevcut şekilleri kontrol edeceğiz
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Şeklin SmartArt olup olmadığını kontrol et
            if (shape.IsSmartArt)
            {
                Console.WriteLine("The shape is a SmartArt object");
            }
            else
            {
                Console.WriteLine("The shape is not a SmartArt object");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


