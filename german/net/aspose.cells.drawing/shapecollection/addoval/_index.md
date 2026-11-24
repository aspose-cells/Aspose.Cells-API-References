---
title: "ShapeCollection.AddOval"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein Oval zum Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

Fügt ein Oval zum Arbeitsblatt hinzu.

```csharp
public Oval AddOval(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz des Ovals von seiner linken Zeile dar, in Pixeln. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz des Ovals von seiner linken Spalte dar, in Pixeln. |
| Höhe | Int32 | Stellt die Höhe des Ovals dar, in Pixeln. |
| Breite | Int32 | Stellt die Breite des Ovals dar, in Pixeln. |

### Rückgabewert

Ein Oval-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOvalWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine ovale Form hinzu
            ShapeCollection shapes = worksheet.Shapes;
            Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);

            // Speichere die Arbeitsmappe
            workbook.Save("AddOvalDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Oval](../../oval/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


