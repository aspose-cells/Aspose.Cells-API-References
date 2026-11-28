---
title: "Shape.SetLockedProperty"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Kilitli özelliği ayarlayın"
type: docs
url: /tr/net/aspose.cells.drawing/shape/setlockedproperty/
---
## Shape.SetLockedProperty method

Kilitli özelliğini ayarla.

```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ShapeLockType | Kilitli tür. |
| değer | Boolean | Özelliğin değeri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLockedPropertyWithShapeLockTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // SetLockedProperty kullanımını gösterin
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
            shape.SetLockedProperty(ShapeLockType.Selection, false);

            Console.WriteLine("Shape locked properties set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


