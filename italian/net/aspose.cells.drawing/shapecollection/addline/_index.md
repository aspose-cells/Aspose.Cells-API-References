---
title: "ShapeCollection.AddLine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un LineShape al foglio di lavoro."
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addline/
---
## ShapeCollection.AddLine method

Aggiunge un LineShape al foglio di lavoro.

```csharp
public LineShape AddLine(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale di LineShape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale di LineShape dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza di LineShape, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza di LineShape, in unità di pixel. |

### Valore di ritorno

Un oggetto LineShape.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLineWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            LineShape lineShape = shapes.AddLine(1, 0, 1, 0, 100, 50);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [LineShape](../../lineshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


