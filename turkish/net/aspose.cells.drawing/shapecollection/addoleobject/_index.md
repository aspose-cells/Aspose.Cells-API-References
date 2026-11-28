---
title: "ShapeCollection.AddOleObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bir OleObject ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addoleobject/
---
## ShapeCollection.AddOleObject method

Bir OleObject ekler.

```csharp
public OleObject AddOleObject(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 |  |
| üst | Int32 |  |
| leftColumn | Int32 |  |
| sol | Int32 |  |
| yükseklik | Int32 |  |
| genişlik | Int32 |  |
| imageData | Byte[] |  |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOleObjectWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            byte[] imageData = File.ReadAllBytes("image.jpg");
            shapes.AddOleObject(4, 0, 5, 0, 300, 500, imageData);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


