---
title: "ExternalLinkCollection.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLinkCollection-metoden. Hämta en enumerator som itererar genom denna samling"
type: docs
url: /sv/net/aspose.cells/externallinkcollection/getenumerator/
---
## ExternalLinkCollection.GetEnumerator method

Hämta en enumerator som itererar genom denna samling.

```csharp
public IEnumerator GetEnumerator()
```

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några externa länkar med den korrekta Add-metodsignaturen
            workbook.Worksheets.ExternalLinks.Add("externallink1.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink2.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink3.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink4.xlam", new string[] { "Sheet1!A1" });

            // Hämta ExternalLinkCollection
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Demonstrera användning av GetEnumerator
            Console.WriteLine("Enumerating external links:");
            IEnumerator enumerator = externalLinks.GetEnumerator();
            int count = 0;
            while (enumerator.MoveNext())
            {
                ExternalLink link = (ExternalLink)enumerator.Current;
                Console.WriteLine($"{++count}. {link.DataSource}");
            }

            // Lägg till formler som refererar till dessa externa länkar
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].Formula = $"=externallink{i+1}.xlam!customfunc()";
            }

            Console.WriteLine("\nFormulas referencing external links:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {worksheet.Cells[i, 0].Formula}");
            }
        }
    }
}
```

### Se även

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


