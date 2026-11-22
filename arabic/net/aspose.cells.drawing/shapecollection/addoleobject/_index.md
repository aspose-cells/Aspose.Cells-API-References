---
title: "ShapeCollection.AddOleObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تُضيف كائن OleObject"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addoleobject/
---
## ShapeCollection.AddOleObject method

يضيف OleObject.

```csharp
public OleObject AddOleObject(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 |  |
| أعلى | Int32 |  |
| العمود الأيسر | Int32 |  |
| يسار | Int32 |  |
| الارتفاع | Int32 |  |
| العرض | Int32 |  |
| imageData | Byte[] |  |

### أمثلة

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

### انظر أيضًا

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


