---
title: "TextOptions.LanguageCode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextOptions egenskap. Hämtar och anger språket för användargränssnittet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

Hämtar och anger språket för användargränssnittet.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form och ange dess text
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // Ställ in språkkoden för formens textalternativ
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // Verifiera och skriv ut språkkoden
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // Spara arbetsboken
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


