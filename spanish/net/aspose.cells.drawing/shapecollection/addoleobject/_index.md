---
title: "ShapeCollection.AddOleObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega un OleObject"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addoleobject/
---
## ShapeCollection.AddOleObject method

Agrega un OleObject.

```csharp
public OleObject AddOleObject(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 |  |
| superior | Int32 |  |
| leftColumn | Int32 |  |
| izquierda | Int32 |  |
| altura | Int32 |  |
| ancho | Int32 |  |
| imageData | Byte[] |  |

### Ejemplos

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

### Ver también

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


