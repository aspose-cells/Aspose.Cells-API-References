---
title: "ExternalLinkCollection.GetEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ExternalLinkCollection. Ottiene un enumeratore che itera attraverso questa raccolta"
type: docs
url: /it/net/aspose.cells/externallinkcollection/getenumerator/
---
## ExternalLinkCollection.GetEnumerator method

Ottieni un enumeratore che itera attraverso questa raccolta.

```csharp
public IEnumerator GetEnumerator()
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni collegamenti esterni usando la corretta firma del metodo Add
            workbook.Worksheets.ExternalLinks.Add("externallink1.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink2.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink3.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink4.xlam", new string[] { "Sheet1!A1" });

            // Ottieni la ExternalLinkCollection
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Dimostra l'uso di GetEnumerator
            Console.WriteLine("Enumerating external links:");
            IEnumerator enumerator = externalLinks.GetEnumerator();
            int count = 0;
            while (enumerator.MoveNext())
            {
                ExternalLink link = (ExternalLink)enumerator.Current;
                Console.WriteLine($"{++count}. {link.DataSource}");
            }

            // Aggiungi formule che fanno riferimento a questi collegamenti esterni
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

### Vedi anche

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


