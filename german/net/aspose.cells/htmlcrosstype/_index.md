---
title: "Enum HtmlCrossType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlCrossType enum. Stellt fünf Typen von HTML‑Kreuz‑Zeichenketten dar"
type: docs
url: /de/net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

Stellt fünf Typen von HTML‑Cross‑Strings dar.

```csharp
public enum HtmlCrossType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Anzeige wie MS Excel, abhängig von der nächsten Zelle. Wenn die nächste Zelle null ist, wird die Zeichenkette gekreuzt, oder sie wird abgeschnitten. |
| MSExport | `1` | Die Zeichenkette wie MS Excel beim Exportieren von HTML anzeigen. |
| Cross | `2` | HTML‑Kreuz‑Zeichenkette anzeigen, diese Leistung beim Erstellen großer HTML‑Dateien ist mehr als zehnmal schneller als das Setzen des Werts auf Default oder FitToCell. |
| CrossHideRight | `3` | HTML‑Kreuz‑Zeichenkette anzeigen und die rechte Zeichenkette ausblenden, wenn sich die Texte überlappen. |
| FitToCell | `4` | Nur die Zeichenkette innerhalb der Zellenbreite anzeigen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHtmlCrossTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);
            
            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Kreuztyp auf MSExport setzen
            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            
            // Arbeitsmappe mit HTML‑Optionen speichern
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


