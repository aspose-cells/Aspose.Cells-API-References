---
title: "ShapeCollection.AddFreeform"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge una forma libera al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

Aggiunge una forma libera al foglio di lavoro.

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale della forma libera dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale della forma libera dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza della forma libera, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza della forma libera, in unità di pixel. |
| paths | ShapePath[] | Rappresenta un percorso definito dall'utente |

### Valore di ritorno

Una forma libera.

### Osservazioni

Nota: la larghezza e l'altezza nei parametri possono essere qualsiasi valore intero positivo, non la larghezza e l'altezza totali dell'array ShapePath specificato da ’paths'. La relazione tra di esse è una relazione di scala-riempimento, cioè ogni oggetto ShapePath verrà scalato in base alla larghezza e all'altezza. Pertanto, quando ci sono più oggetti in 'paths', ogni oggetto ShapePath deve essere progettato in modo ragionevole per soddisfare le aspettative. Quando c'è un solo oggetto ShapePath e non ci sono altri requisiti, passare la larghezza e l'altezza dell'oggetto come valori dei parametri è una buona soluzione.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Crea percorsi di figure personalizzate
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // Aggiungi forma libera al foglio di lavoro
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // Salva la cartella di lavoro
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


