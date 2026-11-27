---
title: "PictureCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PictureCollection metod. Lägger till en bild i samlingen"
type: docs
url: /sv/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Lägger till en bild i samlingen.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| bottomRow | Int32 | Index för nedre högra rad |
| rightColumn | Int32 | Index för nedre högra kolumnen |
| ström | Ström | Strömobjekt som innehåller bilddata. |

### Returvärde

[`Picture`](../../picture/) object index.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild från ström
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(10, 10, 200, 200, fs);
            }

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Lägger till en bild i samlingen.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| bottomRow | Int32 | Index för nedre högra rad |
| rightColumn | Int32 | Index för nedre högra kolumnen |
| fileName | String | Bildfilnamn. |

### Returvärde

[`Picture`](../../picture/) object index.

### Exempel

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

### Se även

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Lägger till en bild i samlingen.

```csharp
public int Add(int topRow, int leftColumn, Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| ström | Ström | Strömobjekt som innehåller bilddata. |

### Returvärde

[`Picture`](../../picture/) object index.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild från ström
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(1, 1, fs);
            }

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Lägger till en bild i samlingen.

```csharp
public int Add(int topRow, int leftColumn, string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| fileName | String | Bildfilnamn. |

### Returvärde

[`Picture`](../../picture/) object index.

### Exempel

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

### Se även

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Lägger till en bild i samlingen.

```csharp
public int Add(int topRow, int leftColumn, Stream stream, int widthScale, int heightScale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| ström | Ström | Strömobjekt som innehåller bilddata. |
| widthScale | Int32 | Skala för bildbredd, i procent. |
| heightScale | Int32 | Skala för bildhöjd, i procent. |

### Returvärde

[`Picture`](../../picture/) object index.

### Exempel

```csharp

[C#]
//lägg till en bild
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Se även

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Lägger till en bild i samlingen.

```csharp
public int Add(int topRow, int leftColumn, string fileName, int widthScale, int heightScale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| fileName | String | Bildfilnamn. |
| widthScale | Int32 | Skala för bildbredd, i procent. |
| heightScale | Int32 | Skala för bildhöjd, i procent. |

### Returvärde

[`Picture`](../../picture/) object index.

### Exempel

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

### Se även

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


