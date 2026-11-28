---
title: "ShapeTextAlignment.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment yöntemi. Bu örneğin, belirtilen başka bir ShapeTextAlignment nesnesiyle aynı değere sahip olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

Bu örneğin, belirtilen başka bir [`ShapeTextAlignment`](../) nesnesiyle aynı değere sahip olup olmadığını belirler.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnek ile karşılaştırılacak [`ShapeTextAlignment`](../) nesnesi. |

### Dönüş Değeri

obj parametresinin değeri bu örnekle aynıysa true; aksi takdirde false. obj null ise, bu metod false döner.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Metin hizalamasını karşılaştırmak için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            
            // Karşılaştırma için başka bir şeklin metin hizalamasını al
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 0, 100, 100);
            ShapeTextAlignment obj = shape2.TextBody.TextAlignment;

            if (shapeTextAlignment.Equals((object)obj))
            {
                Console.WriteLine("Text alignments are equal");
            }
            else
            {
                Console.WriteLine("Text alignments are not equal");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


