---
title: "Enum JsonExportHyperlinkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Json.JsonExportHyperlinkType enum. Stellt den Typ dar, wie Hyperlinks nach JSON exportiert werden."
type: docs
url: /de/net/aspose.cells.json/jsonexporthyperlinktype/
---
## JsonExportHyperlinkType enumeration

Stellt den Typ dar, wie Hyperlinks in JSON exportiert werden.

```csharp
public enum JsonExportHyperlinkType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DisplayString | `0` | Anzeigestring exportieren |
| Address | `1` | URL exportieren |
| HtmlString | `2` | Als HTML-String exportieren. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten mit Hyperlinks hinzu
            worksheet.Cells["A1"].PutValue("Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");

            worksheet.Cells["A2"].PutValue("Aspose");
            worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");

            // Erstelle JsonSaveOptions und setze ExportHyperlinkType
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;

            // Speichere das Arbeitsbuch im JSON-Format
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);

            // Ändere ExportHyperlinkType zu Address und speichere erneut
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);

            // Ändere ExportHyperlinkType zu HtmlString und speichere erneut
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);

            Console.WriteLine("Workbooks saved with different hyperlink export types.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)


