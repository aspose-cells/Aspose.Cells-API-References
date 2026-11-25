---
title: "ShapeCollection.AddShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge una Shape al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addshape/
---
## ShapeCollection.AddShape method

Aggiunge una Shape al foglio di lavoro.

```csharp
public Shape AddShape(MsoDrawingType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | MsoDrawingType | Tipo di disegno Mso. |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale della Shape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale della Shape dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza della Shape, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza della Shape, in unità di pixel. |

### Valore di ritorno

Un oggetto Shape.

### Osservazioni

Il tipo non può essere Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Esempi

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

### Vedi anche

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


