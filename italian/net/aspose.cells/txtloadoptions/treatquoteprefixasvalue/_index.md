---
title: "TxtLoadOptions.TreatQuotePrefixAsValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale verrà rimosso dal valore della cella corrispondente e QuotePrefix sarà impostato a true per la cella."
type: docs
url: /it/net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale verrà rimosso dal valore della cella corrispondente e [`QuotePrefix`](../../style/quoteprefix/) sarà impostato a true per la cella.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Esempi

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
            // Crea dati CSV di esempio con prefissi di virgolette
            string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
            string filePath = "test.csv";

            // Salva i dati CSV in un file
            File.WriteAllText(filePath, csvData);

            // Scenario 1: TreatQuotePrefixAsValue = false (predefinito)
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

            // Pulisci
            File.Delete(filePath);
        }
    }
}
```

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


