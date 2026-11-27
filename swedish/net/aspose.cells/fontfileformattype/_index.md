---
title: "Enum FontFileFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FontFileFormatType enum. Representerar typsnittsformattyp"
type: docs
url: /sv/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

Representerar typsnittformattyp.

```csharp
public enum FontFileFormatType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Unknown | `0` | Okänd typsnittsformattyp. |
| Ttf | `1` | TTF-typsnittsformattyp. |
| Otf | `2` | OTF-typsnittsformattyp. |
| Ttc | `3` | TTC-typsnittsformattyp. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till en cell och ange dess stil
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // Demonstrera användning av FontFileFormatType
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // Använd teckensnittsinställningar
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Kontrollera kompatibilitet för teckensnittformat
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // Spara arbetsboken
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


