---
title: "Klass ExternalLink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalLink class. Representerar en extern länk i en arbetsbok"
type: docs
url: /sv/net/aspose.cells/externallink/
---
## ExternalLink class

Representerar en extern länk i en arbetsbok.

```csharp
public class ExternalLink
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Representerar datakällan för den externa länken. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Indikerar om denna externa länk refereras av andra. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Indikerar om denna externa länk är synlig i MS Excel. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Representerar lagrad datakälla för den externa länken. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | Hämta sökvägstypen för denna externa länk |
| [Type](../../aspose.cells/externallink/type/) { get; } | Hämtar typen av extern länk. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Lägger till ett externt namn. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkDemo
    {
        public static void ExternalLinkExample()
        {
            // Öppna en fil med externa länkar
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // Hämta extern länk 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Visa egenskaper för den externa länken
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // Ändra extern länks datakälla
            externalLink.DataSource = "d:\\linktest.xls";

            // Lägg till ett externt namn till den externa länken
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // Spara arbetsboken
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


