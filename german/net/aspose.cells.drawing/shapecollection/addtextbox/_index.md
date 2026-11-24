---
title: "ShapeCollection.AddTextBox"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein Textfeld zum Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Fügt ein Textfeld zum Arbeitsblatt hinzu.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Abstand des Textfelds von seiner oberen Zeile in Pixeln dar. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Abstand des Textfelds von seiner linken Spalte in Pixeln dar. |
| Höhe | Int32 | Stellt die Höhe des Textfelds in Pixeln dar. |
| Breite | Int32 | Stellt die Breite des Textfelds in Pixeln dar. |

### Rückgabewert

Ein [`TextBox`](../../textbox/) Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Fügen Sie ein TextBox mit angegebener Position und Größe hinzu.
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


