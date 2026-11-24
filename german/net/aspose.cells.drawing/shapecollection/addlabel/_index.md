---
title: "ShapeCollection.AddLabel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein Label zum Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Fügt ein Label zum Arbeitsblatt hinzu.

```csharp
public Label AddLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz von Label von seiner linken Zeile dar, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz von Label von seiner linken Spalte dar, in Pixel. |
| Höhe | Int32 | Stellt die Höhe von Label dar, in Pixel. |
| Breite | Int32 | Stellt die Breite von Label dar, in Pixel. |

### Rückgabewert

Ein Label-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLabelWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Fügt ein Label zum Arbeitsblatt hinzu
            Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
            label.Text = "Sample Label";

            // Speichere die Arbeitsmappe
            workbook.Save("AddLabelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


