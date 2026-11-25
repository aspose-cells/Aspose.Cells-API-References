---
title: "ShapeCollection.AddActiveXControl"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Crea un controllo Activex"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addactivexcontrol/
---
## ShapeCollection.AddActiveXControl method

Crea un controllo Activex.

```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left, 
    int width, int height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ControlType | Il tipo del controllo. |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale della Shape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale della Shape dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza della Shape, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza della Shape, in unità di pixel. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddActiveXControlWithControlTypeInt32Int32Int32Int3Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape activeXControl = shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 
                1,  // upperLeftRow
                0,  // top
                1,  // upperLeftColumn
                0,  // left
                100,  // width
                50   // height
            );

            workbook.Save("AddActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


