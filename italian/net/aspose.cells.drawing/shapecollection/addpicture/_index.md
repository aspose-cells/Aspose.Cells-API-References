---
title: "ShapeCollection.AddPicture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un'immagine alla raccolta"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addpicture/
---
## AddPicture(int, int, int, int, Stream) {#addpicture}

Aggiunge un'immagine alla collezione.

```csharp
public Picture AddPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| bottomRow | Int32 | Indice della riga in basso a destra |
| rightColumn | Int32 | Indice della colonna in basso a destra |
| stream | Stream | Oggetto Stream che contiene i dati dell'immagine. |

### Valore di ritorno

[`Picture`](../../picture/) Picture object.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddPictureWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi un'immagine da un flusso di file
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
            }

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddPicture(int, int, Stream, int, int) {#addpicture_1}

Aggiunge un'immagine alla collezione.

```csharp
public Picture AddPicture(int topRow, int leftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| stream | Stream | Oggetto Stream che contiene i dati dell'immagine. |
| widthScale | Int32 | Scala della larghezza dell'immagine, in percentuale. |
| heightScale | Int32 | Scala dell'altezza dell'immagine, in percentuale. |

### Valore di ritorno

[`Picture`](../../picture/) Picture object.

### Esempi

```csharp

[C#]
//aggiungi un'immagine
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
}
```

### Vedi anche

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


