---
title: "ShapeCollection.AddRectangle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un RectangleShape al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

Aggiunge un RectangleShape al foglio di lavoro.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale del RectangleShape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale di RectangleShape dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza di RectangleShape, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza di RectangleShape, in unità di pixel. |

### Valore di ritorno

Un oggetto RectangleShape.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un rettangolo usando i parametri specificati
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Salva la cartella di lavoro
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


