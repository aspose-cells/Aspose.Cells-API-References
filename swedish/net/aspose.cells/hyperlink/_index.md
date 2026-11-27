---
title: "Klass Hyperlink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Hyperlink-klass. Inkapslar objektet som representerar en hyperlänk"
type: docs
url: /sv/net/aspose.cells/hyperlink/
---
## Hyperlink class

Inkapslar objektet som representerar en hyperlänk.

```csharp
public class Hyperlink
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | Representerar adressen för en hyperlänk. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | Hämtar intervallet för hyperlänken. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | Hämtar länktypen. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | Returnerar eller anger ScreenTip‑texten för den angivna hyperlänken. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | Representerar texten som ska visas för den angivna hyperlänken. Standardvärdet är hyperlänkens adress. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | Tar bort denna hyperlänk |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkDemo
    {
        public static void HyperlinkExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Lägga till ett nytt kalkylblad i Workbook-objektet
            workbook.Worksheets.Add();
            
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägger till en hyperlänk till en URL i cellen "A1"
            int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
            
            // Hämtar en hyperlänk efter index
            Hyperlink hyperlink = worksheet.Hyperlinks[index];
            
            // Ställer in visningstexten för denna hyperlänk
            hyperlink.TextToDisplay = "Aspose";
            
            // Ställer in ScreenTip‑texten för hyperlänken
            hyperlink.ScreenTip = "Visit Aspose Website";
            
            // Sparar Excel-filen
            workbook.Save("HyperlinkExample.xlsx");
            workbook.Save("HyperlinkExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


