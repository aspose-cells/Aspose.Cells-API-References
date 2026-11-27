---
title: "TxtLoadOptions.TreatQuotePrefixAsValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions‑egenskap. Anger om det inledande enkelfnuttstecknet ska tas som en del av värdet i en cell. Standard är true. Om den är false tas det inledande enkelfnuttstecknet bort från motsvarande cells värde och QuotePrefix sätts till true för cellen."
type: docs
url: /sv/net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Anger om det inledande enkelfnuttstecknet ska tas som en del av värdet i en cell. Standard är true. Om den är false tas det inledande enkelfnuttstecknet bort från motsvarande cells värde och [`QuotePrefix`](../../style/quoteprefix/) sätts till true för cellen.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTreatQuotePrefixAsValueDemo
    {
        public static void Run()
        {
            // Skapa exempel‑CSV‑data med citatprefix
            string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
            string filePath = "test.csv";

            // Spara CSV‑data till en fil
            File.WriteAllText(filePath, csvData);

            // Scenario 1: TreatQuotePrefixAsValue = false (standard)
            var loadOptions1 = new TxtLoadOptions();
            loadOptions1.TreatQuotePrefixAsValue = false;
            
            var workbook1 = new Workbook(filePath, loadOptions1);
            var worksheet1 = workbook1.Worksheets[0];
            Console.WriteLine("TreatQuotePrefixAsValue = false:");
            Console.WriteLine("Cell B2 value: " + worksheet1.Cells["B2"].Value); // Will show 'Apple (quote treated as formatting)

            // Scenario 2: TreatQuotePrefixAsValue = true
            var loadOptions2 = new TxtLoadOptions();
            loadOptions2.TreatQuotePrefixAsValue = true;
            
            var workbook2 = new Workbook(filePath, loadOptions2);
            var worksheet2 = workbook2.Worksheets[0];
            Console.WriteLine("\nTreatQuotePrefixAsValue = true:");
            Console.WriteLine("Cell B2 value: " + worksheet2.Cells["B2"].Value); // Will show 'Apple (quote treated as value)

            // Rensa upp
            File.Delete(filePath);
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


