---
title: "ShapeCollection.AddOval"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un Oval al foglio di lavoro."
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

Aggiunge un Oval al foglio di lavoro.

```csharp
public Oval AddOval(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale dell'Oval dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale dell'Oval dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza dell'Oval, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza dell'Oval, in unità di pixel. |

### Valore di ritorno

Un oggetto Oval.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOvalWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma ovale al foglio di lavoro
            ShapeCollection shapes = worksheet.Shapes;
            Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);

            // Salva la cartella di lavoro
            workbook.Save("AddOvalDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Oval](../../oval/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


