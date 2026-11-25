---
title: "ShapeCollection.AddIcons"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapeCollection metodo. Aggiunge immagine svg"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

Aggiunge un'immagine svg.

```csharp
public Picture AddIcons(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageByteData, byte[] compatibleImageData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale della forma dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | L'offset orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | L'altezza della forma, in unità di pixel. |
| larghezza | Int32 | La larghezza della forma, in unità di pixel. |
| imageByteData | Byte[] | I dati byte dell'immagine. |
| compatibleImageData | Byte[] | Dati immagine convertiti da svg per essere compatibili con Excel 2016 o versioni precedenti. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Crea un file icona di esempio (in un utilizzo reale, dovresti usare un file esistente)
            string iconPath = "icon.svg";
            File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");

            // Aggiungi icona al foglio di lavoro
            using (FileStream fs = new FileStream(iconPath, FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            // Pulizia (opzionale)
            File.Delete(iconPath);
        }
    }
}
```

### Vedi anche

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


