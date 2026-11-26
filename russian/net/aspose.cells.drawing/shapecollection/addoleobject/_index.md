---
title: "ShapeCollection.AddOleObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет OleObject"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addoleobject/
---
## ShapeCollection.AddOleObject method

Добавляет OleObject.

```csharp
public OleObject AddOleObject(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 |  |
| верх | Int32 |  |
| leftColumn | Int32 |  |
| влево | Int32 |  |
| высота | Int32 |  |
| ширина | Int32 |  |
| imageData | Byte[] |  |

### Примеры

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

### См. также

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


