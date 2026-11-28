---
title: "ShapeCollection.AddAutoShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir AutoShape ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

Çalışma sayfasına bir AutoShape ekler.

```csharp
public Shape AddAutoShape(AutoShapeType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | AutoShapeType | Auto şekil türü. |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Shape'in sol satırından dikey ofsetini piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Shape'in sol sütunundan yatay ofsetini piksel biriminde temsil eder. |
| yükseklik | Int32 | Shape'in yüksekliğini piksel biriminde temsil eder. |
| genişlik | Int32 | Shape'in genişliğini piksel biriminde temsil eder. |

### Dönüş Değeri

Bir Shape nesnesi.

### Açıklamalar

Tür, Chart/Comment/Picture/OleObject/Polygon/DialogBox olamaz

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddAutoShapeWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
            
            workbook.Save("AutoShapeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


