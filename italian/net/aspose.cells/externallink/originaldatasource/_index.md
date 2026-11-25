---
title: "ExternalLink.OriginalDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExternalLink property. Rappresenta la fonte dati memorizzata del collegamento esterno"
type: docs
url: /it/net/aspose.cells/externallink/originaldatasource/
---
## ExternalLink.OriginalDataSource property

Rappresenta la fonte dati memorizzata del collegamento esterno.

```csharp
public string OriginalDataSource { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyOriginalDataSourceDemo
    {
        public static void Run()
        {
            // Crea un workbook con collegamenti esterni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi collegamento esterno
            worksheet.Cells["A1"].Formula = "='https://arcusventures.sharepoint.com/Fund II/[example.xlsx]Sheet1'!A1";
            
            // Modifica i percorsi dei collegamenti esterni
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                string originalLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
                string modifiedLink = originalLink.Replace(
                    @"https://arcusventures.sharepoint.com/Fund II/", 
                    @"/sites/shared/shared documents/Fund II/");
                
                workbook.Worksheets.ExternalLinks[i].OriginalDataSource = modifiedLink;
            }
            
            // Verifica le modifiche
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine("Modified Link: " + link.OriginalDataSource);
            }
        }
    }
}
```

### Vedi anche

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


