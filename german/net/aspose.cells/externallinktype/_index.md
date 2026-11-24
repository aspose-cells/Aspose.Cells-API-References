---
title: "Enum ExternalLinkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalLinkType Enum. Stellt den Typ eines externen Links dar"
type: docs
url: /de/net/aspose.cells/externallinktype/
---
## ExternalLinkType enumeration

Stellt den Typ des externen Links dar.

```csharp
public enum ExternalLinkType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DDELink | `0` | Stellt den DDE-Link dar. |
| External | `1` | Stellt einen externen Link dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkTypeDemo
    {
        public static void ExternalLinkTypeExample()
        {
            // Öffnen Sie eine Datei mit externen Links
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // Abrufen des externen Links 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Anzeige des Typs des externen Links
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // Ändern Sie die Datenquelle des externen Links
            externalLink.DataSource = "d:\\link.xls";

            // Speichere die Arbeitsmappe
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }

    // Enum, das den Typ eines externen Links darstellt
    public enum ExternalLinkType
    {
        DDELink = 0, // Represents the DDE link
        External = 1 // Represents external link
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


