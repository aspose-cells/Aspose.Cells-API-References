---
title: "ShapeCollection.AddOleObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un OleObject"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addoleobject/
---
## ShapeCollection.AddOleObject method

Aggiunge un OleObject.

```csharp
public OleObject AddOleObject(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 |  |
| alto | Int32 |  |
| leftColumn | Int32 |  |
| sinistra | Int32 |  |
| altezza | Int32 |  |
| larghezza | Int32 |  |
| imageData | Byte[] |  |

### Esempi

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

### Vedi anche

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


