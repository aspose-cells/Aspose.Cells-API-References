---
title: "ShapeCollection.AddOval"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir Oval ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

Çalışma sayfasına bir Oval ekler.

```csharp
public Oval AddOval(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Oval'ın sol satırından dikey offseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Oval'ın sol sütunundan yatay offseti, piksel biriminde temsil eder. |
| yükseklik | Int32 | Oval'ın yüksekliğini, piksel biriminde temsil eder. |
| genişlik | Int32 | Oval'ın genişliğini, piksel biriminde temsil eder. |

### Dönüş Değeri

Bir Oval nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOvalWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir oval şekil ekle
            ShapeCollection shapes = worksheet.Shapes;
            Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);

            // Çalışma kitabını kaydedin
            workbook.Save("AddOvalDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Oval](../../oval/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


