---
title: "ShapeCollection.AddLine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein LineShape zum Arbeitsblatt hinzu."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addline/
---
## ShapeCollection.AddLine method

Fügt ein LineShape zum Arbeitsblatt hinzu.

```csharp
public LineShape AddLine(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Repräsentiert den vertikalen Versatz von LineShape von seiner linken Zeile, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Repräsentiert den horizontalen Versatz von LineShape von seiner linken Spalte, in Pixel. |
| Höhe | Int32 | Repräsentiert die Höhe von LineShape, in Pixel. |
| Breite | Int32 | Repräsentiert die Breite von LineShape, in Pixel. |

### Rückgabewert

Ein LineShape-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLineWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            LineShape lineShape = shapes.AddLine(1, 0, 1, 0, 100, 50);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [LineShape](../../lineshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


