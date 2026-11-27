---
title: "Enum HtmlHiddenRowDisplayType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlHiddenRowDisplayType enum. Representerar två typer av att visa de dolda raderna i html"
type: docs
url: /sv/net/aspose.cells/htmlhiddenrowdisplaytype/
---
## HtmlHiddenRowDisplayType enumeration

Representerar två typer av att visa dolda rader i HTML.

```csharp
public enum HtmlHiddenRowDisplayType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Hidden | `0` | Döljer de dolda raderna på html-sidan. |
| Remove | `1` | Ta bort de dolda raderna på html-sidan. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenRowDisplayTypeDemo
    {
        public static void HtmlHiddenRowDisplayTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Another Visible Row");

            // Dölj den andra raden
            worksheet.Cells.HideRow(1);

            // Skapa HtmlSaveOptions och ställ in HiddenRowDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove

            // Spara arbetsboken i HTML-format
            workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden row display type.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


