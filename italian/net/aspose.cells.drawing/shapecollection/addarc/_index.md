---
title: "ShapeCollection.AddArc"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un ArcShape al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Aggiunge un ArcShape al foglio di lavoro.

```csharp
public ArcShape AddArc(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale di ArcShape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale di ArcShape dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza di ArcShape, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza di ArcShape, in unità di pixel. |

### Valore di ritorno

Un oggetto ArcShape.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddArcWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            ArcShape arcShape = shapes.AddArc(10, 10, 100, 50, 45, 180);
            
            workbook.Save("AddArcDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


