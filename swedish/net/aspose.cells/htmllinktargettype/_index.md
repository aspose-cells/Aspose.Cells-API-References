---
title: "Enum HtmlLinkTargetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlLinkTargetType enum. Representerar typen av target-attribut i HTML‑taggen"
type: docs
url: /sv/net/aspose.cells/htmllinktargettype/
---
## HtmlLinkTargetType enumeration

Representerar typen av target-attribut i HTML-taggen.

```csharp
public enum HtmlLinkTargetType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Blank | `0` | Öppnar det länkade dokumentet i ett nytt fönster eller en ny flik |
| Parent | `1` | Öppnar det länkade dokumentet i föräldraramen |
| Self | `2` | Öppnar det länkade dokumentet i samma ram som det klickades på (detta är standard) |
| Top | `3` | Öppnar det länkade dokumentet i fönstrets hela område |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLinkTargetTypeDemo
    {
        public static void HtmlLinkTargetTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Skapa HtmlSaveOptions och ange LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // Spara arbetsboken i HTML-format
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


