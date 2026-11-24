---
title: "ShapeCollection.AddButton"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt einen Button zum Arbeitsblatt hinzu."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection.AddButton method

Fügt einen Button zum Arbeitsblatt hinzu.

```csharp
public Button AddButton(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Repräsentiert den vertikalen Versatz von Button von seiner linken Zeile, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Repräsentiert den horizontalen Versatz von Button von seiner linken Spalte, in Pixel. |
| Höhe | Int32 | Repräsentiert die Höhe von Button, in Pixel. |
| Breite | Int32 | Repräsentiert die Breite von Button, in Pixel. |

### Rückgabewert

Ein Button-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen Button mit den angegebenen Parametern hinzu
            Aspose.Cells.Drawing.Button button = worksheet.Shapes.AddButton(1, 0, 1, 0, 100, 50);
            button.Text = "Click Me";

            // Speichere die Arbeitsmappe
            workbook.Save("ButtonDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Button](../../button/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


