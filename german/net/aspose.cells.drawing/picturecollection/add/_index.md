---
title: "PictureCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PictureCollection method. Fügt ein Bild zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Fügt ein Bild zur Sammlung hinzu.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| bottomRow | Int32 | Index der unteren rechten Zeile |
| rightColumn | Int32 | Index der unteren rechten Spalte |
| Stream | Stream | Stream-Objekt, das die Bilddaten enthält. |

### Rückgabewert

[`Picture`](../../picture/) object index.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Bild aus einem Stream hinzu
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(10, 10, 200, 200, fs);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Fügt ein Bild zur Sammlung hinzu.

```csharp
public int Add(int topRow, int leftColumn, int bottomRow, int rightColumn, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| bottomRow | Int32 | Index der unteren rechten Zeile |
| rightColumn | Int32 | Index der unteren rechten Spalte |
| fileName | String | Bilddateiname. |

### Rückgabewert

[`Picture`](../../picture/) object index.

### Beispiele

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

### Siehe auch

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Fügt ein Bild zur Sammlung hinzu.

```csharp
public int Add(int topRow, int leftColumn, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| Stream | Stream | Stream-Objekt, das die Bilddaten enthält. |

### Rückgabewert

[`Picture`](../../picture/) object index.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Bild aus einem Stream hinzu
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                worksheet.Pictures.Add(1, 1, fs);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Fügt ein Bild zur Sammlung hinzu.

```csharp
public int Add(int topRow, int leftColumn, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| fileName | String | Bilddateiname. |

### Rückgabewert

[`Picture`](../../picture/) object index.

### Beispiele

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

### Siehe auch

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Fügt ein Bild zur Sammlung hinzu.

```csharp
public int Add(int topRow, int leftColumn, Stream stream, int widthScale, int heightScale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| Stream | Stream | Stream-Objekt, das die Bilddaten enthält. |
| widthScale | Int32 | Skalierung der Bildbreite, ein Prozentsatz. |
| heightScale | Int32 | Skalierung der Bildhöhe, ein Prozentsatz. |

### Rückgabewert

[`Picture`](../../picture/) object index.

### Beispiele

```csharp

[C#]
//ein Bild hinzufügen
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Siehe auch

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Fügt ein Bild zur Sammlung hinzu.

```csharp
public int Add(int topRow, int leftColumn, string fileName, int widthScale, int heightScale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| fileName | String | Bilddateiname. |
| widthScale | Int32 | Skalierung der Bildbreite, ein Prozentsatz. |
| heightScale | Int32 | Skalierung der Bildhöhe, ein Prozentsatz. |

### Rückgabewert

[`Picture`](../../picture/) object index.

### Beispiele

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

### Siehe auch

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


