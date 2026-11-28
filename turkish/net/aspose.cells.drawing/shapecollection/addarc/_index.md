---
title: "ShapeCollection.AddArc"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir ArcShape ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Çalışma sayfasına bir ArcShape ekler.

```csharp
public ArcShape AddArc(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | ArcShape'in sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | ArcShape'in sol sütunundan yatay ofseti, piksel biriminde temsil eder. |
| yükseklik | Int32 | ArcShape'in yüksekliğini, piksel biriminde temsil eder. |
| genişlik | Int32 | ArcShape'in genişliğini, piksel biriminde temsil eder. |

### Dönüş Değeri

Bir ArcShape nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddArcWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            ArcShape arcShape = shapes.AddArc(10, 10, 100, 50, 45, 180);
            
            workbook.Save("AddArcDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


