---
title: "Shape.AddHyperlink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Fügt der Form einen Hyperlink hinzu."
type: docs
url: /de/net/aspose.cells.drawing/shape/addhyperlink/
---
## Shape.AddHyperlink method

Fügt der Form einen Hyperlink hinzu.

```csharp
public Hyperlink AddHyperlink(string address)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| address | String | Adresse des Hyperlinks. |

### Rückgabewert

Gibt das neue Hyperlink-Objekt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAddHyperlinkWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Füge der Form einen Hyperlink mit einer Zeichenketten-URL hinzu.
            Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeWithHyperlink.xlsx");
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


