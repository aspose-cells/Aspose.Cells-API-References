---
title: "Shape.AddHyperlink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Lägger till en hyperlänk till formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/addhyperlink/
---
## Shape.AddHyperlink method

Lägger till en hyperlänk till formen.

```csharp
public Hyperlink AddHyperlink(string address)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | String | Adress för hyperlänken. |

### Returvärde

Returnerar det nya hyperlänkobjektet.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Lägg till en hyperlänk till formen med sträng-URL
            Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");

            // Spara arbetsboken
            workbook.Save("ShapeWithHyperlink.xlsx");
        }
    }
}
```

### Se även

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


