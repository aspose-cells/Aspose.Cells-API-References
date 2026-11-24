---
title: "ExternalLinkCollection.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLinkCollection-Methode. Gibt einen Enumerator zurück, der diese Sammlung durchläuft"
type: docs
url: /de/net/aspose.cells/externallinkcollection/getenumerator/
---
## ExternalLinkCollection.GetEnumerator method

Holen Sie einen Enumerator, der durch diese Sammlung iteriert.

```csharp
public IEnumerator GetEnumerator()
```

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Füge einige externe Links hinzu, indem du die korrekte Add-Methodensignatur verwendest
            workbook.Worksheets.ExternalLinks.Add("externallink1.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink2.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink3.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink4.xlam", new string[] { "Sheet1!A1" });

            // Hole die ExternalLinkCollection
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Demonstriere die Verwendung von GetEnumerator
            Console.WriteLine("Enumerating external links:");
            IEnumerator enumerator = externalLinks.GetEnumerator();
            int count = 0;
            while (enumerator.MoveNext())
            {
                ExternalLink link = (ExternalLink)enumerator.Current;
                Console.WriteLine($"{++count}. {link.DataSource}");
            }

            // Füge Formeln hinzu, die auf diese externen Links verweisen.
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

### Siehe auch

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


