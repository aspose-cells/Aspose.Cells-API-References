---
title: "ShapeCollection.AddCopy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt eine Form hinzu und kopiert sie zum Arbeitsblatt"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addcopy/
---
## AddCopy(Shape, int, int, int, int) {#addcopy}

Fügt eine Form zum Arbeitsblatt hinzu und kopiert sie.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceShape | Form | Quellform. |
| topRow | Int32 | Der Index der obersten Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz von seiner oberen Zeile dar, in Pixel. |
| leftColumn | Int32 | Der Index der linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz von seiner linken Spalte dar, in Pixel. |

### Rückgabewert

Das neue [`Shape`](../../shape/) Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Rechteckform hinzufügen
            RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Füge eine Kopie der Rechteckform mit neuer Position hinzu
            shapes.AddCopy(rectangle, 7, 0, 7, 0);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Shape, int, int, int, int, CopyOptions) {#addcopy_1}

Fügt eine Form zum Arbeitsblatt hinzu und kopiert sie.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, 
    CopyOptions copyOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceShape | Form | Quellform. |
| topRow | Int32 | Der Index der obersten Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz von seiner oberen Zeile dar, in Pixel. |
| leftColumn | Int32 | Der Index der linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz von seiner linken Spalte dar, in Pixel. |
| copyOptions | CopyOptions | Die Optionen zum Kopieren von Formen. |

### Rückgabewert

Das neue [`Shape`](../../shape/) Objekt.

### Beispiele

```csharp

[C#]
//Form hinzufügen
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Fügt eine Form hinzu und kopiert sie.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### Siehe auch

* class [Shape](../../shape/)
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


