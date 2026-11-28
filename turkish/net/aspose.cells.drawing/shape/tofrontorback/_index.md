---
title: "Shape.ToFrontOrBack"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Şekli öne getirir veya arkaya gönderir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/tofrontorback/
---
## Shape.ToFrontOrBack method

Şekli öne getirir veya arkaya gönderir.

```csharp
public void ToFrontOrBack(int orders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sıralamalar | Int32 | Sıfırdan küçükse, şekli arkaya ayarlar. Sıfırdan büyükse, şekli öne getirir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToFrontOrBackWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // z-sırasını göstermek için iki şekil ekleyin
            Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // shape2'yi z-sırasında 2 konum ileri taşıyın
            shape2.ToFrontOrBack(2);

            // shape1'i z-sırasında 1 konum geri taşıyın
            shape1.ToFrontOrBack(-1);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


