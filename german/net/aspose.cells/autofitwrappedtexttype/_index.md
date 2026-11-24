---
title: "Enum AutoFitWrappedTextType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AutoFitWrappedTextType Enum. Stellt den Typ des automatischen Anpassens von umgebrochenem Text dar"
type: docs
url: /de/net/aspose.cells/autofitwrappedtexttype/
---
## AutoFitWrappedTextType enumeration

Stellt den Typ des automatischen Anpassens von umgebrochenem Text dar.

```csharp
public enum AutoFitWrappedTextType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Funktioniert wie MS Excel. |
| Paragraph | `1` | Automatisches Anpassen der Breite an den längsten Absatz. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitWrappedTextTypeDemo
    {
        public static void AutoFitWrappedTextTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
            worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");

            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            Style style2 = worksheet.Cells["A5"].GetStyle();
            style2.IsTextWrapped = true;
            worksheet.Cells["A5"].SetStyle(style);

            // Erstelle einen Bereich A1:F3
            Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
            // Zellen zusammenführen
            range.Merge();

            // Erstelle einen Bereich A4:F6
            Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
            // Zellen zusammenführen
            range2.Merge();

            // Erstelle AutoFitterOptions und setze AutoFitWrappedTextType
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            // Zeilen automatisch anpassen mit den angegebenen Optionen
            worksheet.AutoFitRows(options);

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
            workbook.Save("AutoFitWrappedTextTypeExample.pdf");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


