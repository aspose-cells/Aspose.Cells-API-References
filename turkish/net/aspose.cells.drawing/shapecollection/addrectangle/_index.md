---
title: "ShapeCollection.AddRectangle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir RectangleShape ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

Çalışma sayfasına bir RectangleShape ekler.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | RectangleShape'in sol satırından dikey ofsetini, piksel birimi cinsinden temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | RectangleShape'in sol sütunundan yatay kaymasını piksel biriminde temsil eder. |
| yükseklik | Int32 | RectangleShape'in yüksekliğini piksel biriminde temsil eder. |
| genişlik | Int32 | RectangleShape'in genişliğini piksel biriminde temsil eder. |

### Dönüş Değeri

Bir RectangleShape nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Belirtilen parametreleri kullanarak bir dikdörtgen ekle
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Çalışma kitabını kaydedin
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


