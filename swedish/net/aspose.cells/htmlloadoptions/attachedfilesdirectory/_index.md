---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions-egenskap. Katalogen som de bifogade filerna kommer att sparas i"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

Katalogen som de bifogade filerna kommer att sparas i.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället HtmlLoadOptions.StreamProvider‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med december 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Skapa en instans av HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Ställ in katalogen för bifogade filer
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // Läs in en HTML-fil i en arbetsbok med de angivna alternativen
            Workbook workbook = new Workbook("input.html", options);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


