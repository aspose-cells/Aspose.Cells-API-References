---
title: "Workbook.HasExernalLinks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Anger om denna arbetsbok innehåller externa länkar till andra datakällor"
type: docs
url: /sv/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Anger om denna arbetsbok innehåller externa länkar till andra datakällor.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Returvärde

Om denna arbetsbok innehåller externa länkar till andra datakällor.

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället ExternalLinkCollection.Count för att kontrollera om det finns externa länkar i denna arbetsbok. Denna metod kommer att tas bort 12 månader senare sedan december 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med externa länkar
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // Lägg till en extern länk
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // Kontrollera om arbetsboken har externa länkar
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


