---
title: "Enum HtmlCrossType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlCrossType enum. Representerar fem typer av HTML-korssträng"
type: docs
url: /sv/net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

Representerar fem typer av HTML-korssträng.

```csharp
public enum HtmlCrossType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Visas som i MS Excel, beror på nästa cell. Om nästa cell är null, kommer strängen att korsas, eller så trunkeras den. |
| MSExport | `1` | Visa strängen som i MS Excel vid export av HTML. |
| Cross | `2` | Visa HTML-korssträng, denna prestanda för att skapa stora HTML-filer kommer att vara mer än tio gånger snabbare än att sätta värdet till Default eller FitToCell. |
| CrossHideRight | `3` | Visa HTML-korssträng och dölj den högra strängen när texterna överlappar. |
| FitToCell | `4` | Visar endast strängen inom cellens bredd. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHtmlCrossTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);
            
            // Skapa HTML-sparalternativ
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Ange korsningstyp till MSExport
            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            
            // Spara arbetsbok med HTML-alternativ
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


