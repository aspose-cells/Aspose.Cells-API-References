---
title: "Enum HtmlHiddenColDisplayType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlHiddenColDisplayType enum. Representerar två typer av att visa de dolda kolumnerna i HTML"
type: docs
url: /sv/net/aspose.cells/htmlhiddencoldisplaytype/
---
## HtmlHiddenColDisplayType enumeration

Representerar två typer av att visa dolda kolumner i HTML.

```csharp
public enum HtmlHiddenColDisplayType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Hidden | `0` | Döljer de dolda kolumnerna på HTML-sidan. |
| Remove | `1` | Tar bort de dolda kolumnerna på HTML-sidan. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenColDisplayTypeDemo
    {
        public static void HtmlHiddenColDisplayTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Dölj den andra kolumnen
            worksheet.Cells.HideColumn(1);

            // Skapa HtmlSaveOptions och sätt HiddenColDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;

            // Spara arbetsboken i HTML-format
            workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


