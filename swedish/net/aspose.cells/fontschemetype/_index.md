---
title: "Enum FontSchemeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FontSchemeType enum. Representerar schematypen för teckensnittet."
type: docs
url: /sv/net/aspose.cells/fontschemetype/
---
## FontSchemeType enumeration

Representerar schematypen för typsnittet.

```csharp
public enum FontSchemeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen |
| Major | `1` | Större schema. |
| Minor | `2` | Mindre schema. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSchemeTypeDemo
    {
        public static void FontSchemeTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Hämta referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            // Åtkomst till cellen "A1" från kalkylbladet
            Cell cell = worksheet.Cells["A1"];
            // Lägger till ett värde i cellen "A1"
            cell.PutValue("Hello Aspose!");

            // Åtkomst till teckensnittet i cellstilen
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Ställer in teckensnittsschematyp till Större
            font.SchemeType = FontSchemeType.Major;

            // Ställer in andra teckensnittsegenskaper för demonstration
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // Spara arbetsboken
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


