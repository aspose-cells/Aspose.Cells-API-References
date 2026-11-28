---
title: "Shape.GetLockedProperty"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Kilitli özelliğin değerini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

Kilitli özelliğinin değerini alır.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ShapeLockType | Şeklin kilitli özelliğinin türü. |

### Dönüş Değeri

Kilitli özelliğin değerini döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLockedPropertyWithShapeLockTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // AdjustHandles için kilitli özelliği ayarla
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);

            // AdjustHandles'ın kilitli olup olmadığını kontrol et
            int noAdjustHandles = 0;
            if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
                noAdjustHandles = 1;

            Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
        }
    }
}
```

### Ayrıca Bakınız

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


