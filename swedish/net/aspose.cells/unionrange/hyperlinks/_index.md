---
title: "UnionRange.Hyperlinks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑egenskap. Hämtar alla hyperlänkar i området"
type: docs
url: /sv/net/aspose.cells/unionrange/hyperlinks/
---
## UnionRange.Hyperlinks property

Hämtar alla hyperlänkar i området.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några hyperlänkar i celler
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://products.aspose.com/cells");
            worksheet.Hyperlinks.Add("C3", 1, 1, "https://docs.aspose.com/cells/net");

            // Skapa ett intervall
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            UnionRange unionRange = range.UnionRanges(new Aspose.Cells.Range[] { range });

            // Hämta hyperlänkar i området
            Hyperlink[] hyperlinks = unionRange.Hyperlinks;
            Console.WriteLine("Hyperlinks count in range: " + hyperlinks.Length);

            // Visa information om varje hyperlänk
            foreach (Hyperlink link in hyperlinks)
            {
                Console.WriteLine("Address: " + link.Address + ", Text: " + link.TextToDisplay);
            }

            // Spara arbetsboken
            workbook.Save("HyperlinksDemo.xlsx");
        }
    }
}
```

### Se även

* class [Hyperlink](../../hyperlink/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


