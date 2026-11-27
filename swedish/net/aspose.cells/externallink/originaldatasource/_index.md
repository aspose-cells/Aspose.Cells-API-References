---
title: "ExternalLink.OriginalDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLink-egenskap. Representerar lagrad datakälla för den externa länken"
type: docs
url: /sv/net/aspose.cells/externallink/originaldatasource/
---
## ExternalLink.OriginalDataSource property

Representerar lagrad datakälla för den externa länken.

```csharp
public string OriginalDataSource { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyOriginalDataSourceDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med externa länkar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till extern länk
            worksheet.Cells["A1"].Formula = "='https://arcusventures.sharepoint.com/Fund II/[example.xlsx]Sheet1'!A1";
            
            // Ändra sökvägar för extern länk
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                string originalLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
                string modifiedLink = originalLink.Replace(
                    @"https://arcusventures.sharepoint.com/Fund II/", 
                    @"/sites/shared/shared documents/Fund II/");
                
                workbook.Worksheets.ExternalLinks[i].OriginalDataSource = modifiedLink;
            }
            
            // Verifiera ändringarna
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine("Modified Link: " + link.OriginalDataSource);
            }
        }
    }
}
```

### Se även

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


