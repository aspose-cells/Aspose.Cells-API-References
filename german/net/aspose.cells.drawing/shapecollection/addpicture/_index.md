---
title: "ShapeCollection.AddPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein Bild zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addpicture/
---
## AddPicture(int, int, int, int, Stream) {#addpicture}

Fügt ein Bild zur Sammlung hinzu.

```csharp
public Picture AddPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| bottomRow | Int32 | Index der unteren rechten Zeile |
| rightColumn | Int32 | Index der unteren rechten Spalte |
| Stream | Stream | Stream-Objekt, das die Bilddaten enthält. |

### Rückgabewert

[`Picture`](../../picture/) Picture object.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Ein Bild aus einem Dateistream hinzufügen
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddPicture(int, int, Stream, int, int) {#addpicture_1}

Fügt ein Bild zur Sammlung hinzu.

```csharp
public Picture AddPicture(int topRow, int leftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| Stream | Stream | Stream-Objekt, das die Bilddaten enthält. |
| widthScale | Int32 | Skalierung der Bildbreite, ein Prozentsatz. |
| heightScale | Int32 | Skalierung der Bildhöhe, ein Prozentsatz. |

### Rückgabewert

[`Picture`](../../picture/) Picture object.

### Beispiele

```csharp

[C#]
//ein Bild hinzufügen
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
}
```

### Siehe auch

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


