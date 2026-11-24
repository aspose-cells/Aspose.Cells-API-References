---
title: "TextOptions.LanguageCode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions property. Gibt die Sprache der Benutzeroberfläche zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

Liest und setzt die Sprache der Benutzeroberfläche.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu und setze ihren Text
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // Lege den Sprachcode für die Textoptionen der Form fest
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // Überprüfe und gib den Sprachcode aus
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // Speichere die Arbeitsmappe
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


