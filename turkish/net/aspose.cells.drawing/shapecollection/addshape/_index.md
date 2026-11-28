---
title: "ShapeCollection.AddShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir Shape ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addshape/
---
## ShapeCollection.AddShape method

Çalışma sayfasına bir Shape ekler.

```csharp
public Shape AddShape(MsoDrawingType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | MsoDrawingType | Mso çizim türü. |
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
    public class ShapeCollectionMethodAddShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 200, 50);
            
            Console.WriteLine("Shape added successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


