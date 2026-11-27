---
title: "Klass MsoFillFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoFillFormat-klass. Representerar fyllningsformatering för en form"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformat/
---
## MsoFillFormat class

Representerar fyllningsformat för en form.

```csharp
public class MsoFillFormat
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | Hämtar och anger filens bakgrundsfärg. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | Hämtar och anger fyllningens förgrundsfärg. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | Hämtar och anger textur‑ och bildfyllnadsdata. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | Indikerar om det finns fyllning. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | Hämtar typen av texturfyllning. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | Returnerar eller anger graden av transparens för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (klar). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en enfärgsgradient. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatDemo
    {
        public static void MsoFillFormatExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bågform till kalkylbladet
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Åtkomst till fyllningsformatet för formen
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Ställ in fyllningens förgrundsfärg
            fillFormat.ForeColor = Color.Blue;

            // Ställ in fyllningens bakgrundsfärg
            fillFormat.BackColor = Color.LightBlue;

            // Ställ in transparensen
            fillFormat.Transparency = 0.5;

            // Kontrollera om fyllningen är synlig
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // Ställ in en enfärgsgradientfyllning
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Spara arbetsboken
            workbook.Save("MsoFillFormatExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


