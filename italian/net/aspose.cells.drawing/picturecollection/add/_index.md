---
title: "PictureCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PictureCollection. Aggiunge un'immagine alla collezione"
type: docs
url: /it/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Aggiunge un'immagine alla collezione.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| bottomRow | Int32 | Indice della riga in basso a destra |
| rightColumn | Int32 | Indice della colonna in basso a destra |
| stream | Stream | Oggetto Stream che contiene i dati dell'immagine. |

### Valore di ritorno

[`Picture`](../../picture/) object index.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine dal flusso
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(10, 10, 200, 200, fs);
            }

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Aggiunge un'immagine alla collezione.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| bottomRow | Int32 | Indice della riga in basso a destra |
| rightColumn | Int32 | Indice della colonna in basso a destra |
| fileName | String | Nome file dell'immagine. |

### Valore di ritorno

[`Picture`](../../picture/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, 5, 5, "image.jpg");

            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Aggiunge un'immagine alla collezione.

```csharp
public int Add(int topRow, int leftColumn, Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| stream | Stream | Oggetto Stream che contiene i dati dell'immagine. |

### Valore di ritorno

[`Picture`](../../picture/) object index.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine dal flusso
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(1, 1, fs);
            }

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Aggiunge un'immagine alla collezione.

```csharp
public int Add(int topRow, int leftColumn, string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| fileName | String | Nome file dell'immagine. |

### Valore di ritorno

[`Picture`](../../picture/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, "image.jpg");

            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Aggiunge un'immagine alla collezione.

```csharp
public int Add(int topRow, int leftColumn, Stream stream, int widthScale, int heightScale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| stream | Stream | Oggetto Stream che contiene i dati dell'immagine. |
| widthScale | Int32 | Scala della larghezza dell'immagine, in percentuale. |
| heightScale | Int32 | Scala dell'altezza dell'immagine, in percentuale. |

### Valore di ritorno

[`Picture`](../../picture/) object index.

### Esempi

```csharp

[C#]
//aggiungi un'immagine
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Vedi anche

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Aggiunge un'immagine alla collezione.

```csharp
public int Add(int topRow, int leftColumn, string fileName, int widthScale, int heightScale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| fileName | String | Nome file dell'immagine. |
| widthScale | Int32 | Scala della larghezza dell'immagine, in percentuale. |
| heightScale | Int32 | Scala dell'altezza dell'immagine, in percentuale. |

### Valore di ritorno

[`Picture`](../../picture/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodAddWithInt32Int32StringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            PictureCollection pictures = worksheet.Pictures;
            pictures.Add(1, 1, "image.jpg", 50, 50);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


