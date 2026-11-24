---
title: "Enum HtmlHiddenRowDisplayType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlHiddenRowDisplayType-Enum. Stellt zwei Arten dar, versteckte Zeilen in HTML anzuzeigen."
type: docs
url: /de/net/aspose.cells/htmlhiddenrowdisplaytype/
---
## HtmlHiddenRowDisplayType enumeration

Stellt zwei Arten dar, versteckte Zeilen in HTML anzuzeigen.

```csharp
public enum HtmlHiddenRowDisplayType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Hidden | `0` | Versteckt die versteckten Zeilen auf der HTML-Seite. |
| Remove | `1` | Entfernt die versteckten Zeilen auf der HTML-Seite. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenRowDisplayTypeDemo
    {
        public static void HtmlHiddenRowDisplayTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Another Visible Row");

            // Verstecke die zweite Zeile
            worksheet.Cells.HideRow(1);

            // Erstelle HtmlSaveOptions und setze den HiddenRowDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove

            // Speichere das Arbeitsbuch im HTML‑Format
            workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden row display type.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


