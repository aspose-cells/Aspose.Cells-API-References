---
title: "ShapeCollection.AddPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en bild i samlingen"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addpicture/
---
## AddPicture(int, int, int, int, Stream) {#addpicture}

Lägger till en bild i samlingen.

```csharp
public Picture AddPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| bottomRow | Int32 | Index för nedre högra rad |
| rightColumn | Int32 | Index för nedre högra kolumnen |
| ström | Ström | Strömobjekt som innehåller bilddata. |

### Returvärde

[`Picture`](../../picture/) Picture object.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en bild från en filström
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
            }

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddPicture(int, int, Stream, int, int) {#addpicture_1}

Lägger till en bild i samlingen.

```csharp
public Picture AddPicture(int topRow, int leftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| ström | Ström | Strömobjekt som innehåller bilddata. |
| widthScale | Int32 | Skala för bildbredd, i procent. |
| heightScale | Int32 | Skala för bildhöjd, i procent. |

### Returvärde

[`Picture`](../../picture/) Picture object.

### Exempel

```csharp

[C#]
//lägg till en bild
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
}
```

### Se även

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


