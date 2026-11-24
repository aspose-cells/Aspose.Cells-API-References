---
title: "Shape.Characters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Text darstellt."
type: docs
url: /de/net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich innerhalb des Textes darstellt.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 | Der Index des Beginns des Zeichens. |
| Länge | Int32 | Die Anzahl der Zeichen. |

### Rückgabewert

Characters-Objekt.

### Hinweise

Diese Methode funktioniert nur bei Formen mit Titel.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Form mit Text hinzu.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "Sample Text";

            // Hole Zeichen ab Index 0 mit Länge 4.
            FontSetting fontSetting = shape.Characters(0, 4);
            
            // Ändern Sie die Schriftarteinstellungen
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.Size = 14;
            fontSetting.Font.IsBold = true;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeCharactersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


