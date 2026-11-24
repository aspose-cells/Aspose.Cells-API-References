---
title: "Aufzählung HtmlLinkTargetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlLinkTargetType Aufzählung. Stellt den Typ des target-Attributs im HTML‑Tag dar"
type: docs
url: /de/net/aspose.cells/htmllinktargettype/
---
## HtmlLinkTargetType enumeration

Stellt den Typ des target‑Attributs im HTML‑Tag dar.

```csharp
public enum HtmlLinkTargetType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Blank | `0` | Öffnet das verknüpfte Dokument in einem neuen Fenster oder Tab |
| Parent | `1` | Öffnet das verknüpfte Dokument im übergeordneten Frame |
| Self | `2` | Öffnet das verknüpfte Dokument im selben Frame, in dem es angeklickt wurde (dies ist die Vorgabe) |
| Top | `3` | Öffnet das verknüpfte Dokument im gesamten Fensterinhalt |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLinkTargetTypeDemo
    {
        public static void HtmlLinkTargetTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Erstellen Sie HtmlSaveOptions und setzen Sie den LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // Speichere das Arbeitsbuch im HTML‑Format
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


