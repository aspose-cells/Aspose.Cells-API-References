---
title: "Enum HtmlOfficeMathOutputType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlOfficeMathOutputType Enum. Gibt an, wie OfficeMath nach HTML exportiert wird"
type: docs
url: /de/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

Stellt dar, wie OfficeMath nach HTML exportiert wird.

```csharp
public enum HtmlOfficeMathOutputType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Image | `0` | Konvertiert OfficeMath nach HTML als Bild, das durch das &lt;img&gt;-Tag angegeben ist. |
| MathML | `1` | Konvertiert OfficeMath zu HTML unter Verwendung von MathML. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge OfficeMath zu Zelle A1 hinzu
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Setze den OfficeMath-Ausgabetyp auf Bild
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // Speichern mit Bild-Ausgabetyp
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // Ändere den Ausgabetyp zu MathML
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // Speichern mit MathML-Ausgabetyp
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


