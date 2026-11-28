---
title: "Shape.IsWordArt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bu şeklin bir kelime sanatı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/iswordart/
---
## Shape.IsWordArt property

Bu şeklin kelime sanatı olup olmadığını gösterir.

```csharp
public bool IsWordArt { get; }
```

### Açıklamalar

Yalnızca xls dosyasının Eski Şekli için.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsWordArtDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle bir WordArt şekli ekle
            Shape wordArt = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample WordArt", 0, 0, 100, 100, 100, 100);

            // Tüm gerekli parametrelerle normal bir dikdörtgen şekli ekle
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 150, 100, 100, 100);

            // Şekillerin WordArt olup olmadığını kontrol et
            Console.WriteLine("WordArt shape is WordArt: " + wordArt.IsWordArt);
            Console.WriteLine("Rectangle shape is WordArt: " + rectangle.IsWordArt);

            // IsWordArt özelliğinin örnek kullanımı
            if (wordArt.IsWordArt)
            {
                Console.WriteLine("First shape is a WordArt object");
            }

            if (!rectangle.IsWordArt)
            {
                Console.WriteLine("Second shape is not a WordArt object");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


