---
title: "Enum HtmlVersion"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlVersion enum. Gibt an, welche HTML-Version beim Speichern in HTML-Formaten verwendet wird."
type: docs
url: /de/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

Gibt an, welche HTML‑Version beim Speichern in HTML‑Formaten verwendet wird.

```csharp
public enum HtmlVersion
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Speichern Sie das Dokument gemäß dem von MS Excel exportierten HTML. |
| XHtml | `1` | Speichert das Dokument gemäß dem XHTML 1.0 Transitional-Standard. |
| Html5 | `2` | Speichert das Dokument gemäß dem HTML 5‑Standard. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Setzen Sie die HTML-Version auf HTML5
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // Speichern Sie die Arbeitsmappe mit der HTML5-Version
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // Ändern Sie die HTML-Version zu XHTML
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // Speichern Sie die Arbeitsmappe mit der XHTML-Version
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // Setzen Sie die HTML-Version auf Standard (MS Excel‑kompatibel)
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // Speichern Sie die Arbeitsmappe mit der Standardversion
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


