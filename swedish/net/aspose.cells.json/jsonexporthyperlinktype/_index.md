---
title: "Enum JsonExportHyperlinkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Json.JsonExportHyperlinkType enum. Representerar typen hur hyperlänkar exporteras till json"
type: docs
url: /sv/net/aspose.cells.json/jsonexporthyperlinktype/
---
## JsonExportHyperlinkType enumeration

Representerar typen hur hyperlänkar exporteras till JSON.

```csharp
public enum JsonExportHyperlinkType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DisplayString | `0` | Exportera visningssträng |
| Address | `1` | Exportera URL |
| HtmlString | `2` | Exportera som HTML-sträng. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonExportHyperlinkTypeDemo
    {
        public static void JsonExportHyperlinkTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med hyperlänkar
            worksheet.Cells["A1"].PutValue("Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");

            worksheet.Cells["A2"].PutValue("Aspose");
            worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");

            // Skapa JsonSaveOptions och ställ in ExportHyperlinkType
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;

            // Spara arbetsboken i JSON-format
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);

            // Ändra ExportHyperlinkType till Address och spara igen
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);

            // Ändra ExportHyperlinkType till HtmlString och spara igen
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);

            Console.WriteLine("Workbooks saved with different hyperlink export types.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)


