---
title: "Aufzählung FontFileFormatType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FontFileFormatType Aufzählung. Stellt den Schriftartformattyp dar"
type: docs
url: /de/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

Stellt den Schriftartformattyp dar.

```csharp
public enum FontFileFormatType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Unknown | `0` | Unbekannter Schriftartformattyp. |
| Ttf | `1` | TTF-Schriftartformattyp. |
| Otf | `2` | OTF-Schriftartformattyp. |
| Ttc | `3` | TTC-Schriftartformattyp. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf eine Zelle zu und setzen Sie deren Stil
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // Demonstrieren Sie die Verwendung von FontFileFormatType
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // Schriftarteinstellungen anwenden
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Überprüfen Sie die Kompatibilität des Schriftartformats
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


