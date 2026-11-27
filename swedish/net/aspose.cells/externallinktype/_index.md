---
title: "Enum ExternalLinkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalLinkType enum. Representerar typen av extern länk"
type: docs
url: /sv/net/aspose.cells/externallinktype/
---
## ExternalLinkType enumeration

Representerar typen av extern länk.

```csharp
public enum ExternalLinkType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DDELink | `0` | Representerar DDE-länken. |
| External | `1` | Representerar extern länk. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkTypeDemo
    {
        public static void ExternalLinkTypeExample()
        {
            // Öppna en fil med externa länkar
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // Hämta extern länk 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Visa typen av extern länk
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // Ändra extern länks datakälla
            externalLink.DataSource = "d:\\link.xls";

            // Spara arbetsboken
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }

    // Enum som representerar typen av extern länk
    public enum ExternalLinkType
    {
        DDELink = 0, // Represents the DDE link
        External = 1 // Represents external link
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


