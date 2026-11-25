---
title: "ShapeCollection.AddFreeFloatingShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge una forma fluttuante al foglio di lavoro. Si applica solo a forme di linea/immagine"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addfreefloatingshape/
---
## ShapeCollection.AddFreeFloatingShape method

Aggiunge una forma libera fluttuante al foglio di lavoro. Si applica solo per forme di linea/immagine.

```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width, 
    byte[] imageData, bool isOriginalSize)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | MsoDrawingType | Il tipo di forma. |
| alto | Int32 | Rappresenta lo spostamento verticale della forma dalla riga superiore del foglio di lavoro, in unità di pixel. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale della forma dalla colonna sinistra del foglio di lavoro, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza di LineShape, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza di LineShape, in unità di pixel. |
| imageData | Byte[] | I dati dell'immagine, si applicano solo all'immagine. |
| isOriginalSize | Booleano | Indica se la forma utilizza le dimensioni originali se la forma è un'immagine. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi una forma linea
            Shape floatingShape_Line = shapes.AddFreeFloatingShape(
                MsoDrawingType.Line, 
                100, 100, 100, 50, 
                null, 
                false);

            // Aggiungi una forma immagine (usando dati immagine di esempio)
            byte[] imageData = null;
            try
            {
                using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
                {
                    imageData = new byte[fs.Length];
                    fs.Read(imageData, 0, (int)fs.Length);
                }
            }
            catch
            {
                // Crea dati immagine fittizi se il file non è trovato
                imageData = new byte[100];
            }

            Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
                MsoDrawingType.Picture, 
                200, 100, 100, 50, 
                imageData, 
                false);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
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


