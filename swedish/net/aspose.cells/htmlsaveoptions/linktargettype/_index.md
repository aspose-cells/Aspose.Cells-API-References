---
title: "HtmlSaveOptions.LinkTargetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions property. Anger typen av target‑attribut i en länk. Standardvärdet är HtmlLinkTargetType.Parent."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/linktargettype/
---
## HtmlSaveOptions.LinkTargetType property

Anger typen av target-attribut i `<a>`-länk. Standardvärdet är HtmlLinkTargetType.Parent.

```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyLinkTargetTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Link to Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.google.com");

            // Ställ in HTML‑sparalternativ med LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            // Spara arbetsboken som HTML
            workbook.Save("output.html", saveOptions);
        }
    }
}
```

### Se även

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


