---
title: "ShapeCollection.AddScrollBar"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge una ScrollBar al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addscrollbar/
---
## ShapeCollection.AddScrollBar method

Aggiunge una ScrollBar al foglio di lavoro.

```csharp
public ScrollBar AddScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale della ScrollBar dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale della ScrollBar dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza della ScrollBar, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza della ScrollBar, in unità di pixel. |

### Valore di ritorno

Un oggetto ScrollBar.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddScrollBarWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            ScrollBar scrollBar = shapes.AddScrollBar(1, 0, 100, 20, 0, 100);
            scrollBar.CurrentValue = 50;
            scrollBar.Width = 200;
            scrollBar.Height = 30;

            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScrollBar](../../scrollbar/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


