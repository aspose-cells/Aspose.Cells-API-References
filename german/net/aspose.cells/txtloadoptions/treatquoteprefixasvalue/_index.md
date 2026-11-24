---
title: "TxtLoadOptions.TreatQuotePrefixAsValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions‑Eigenschaft. Gibt an, ob das führende einfache Anführungszeichen als Teil des Zellwertes betrachtet werden soll. Standard ist true. Ist es false, wird das führende einfache Anführungszeichen aus dem Wert der entsprechenden Zelle entfernt und QuotePrefix wird für die Zelle auf true gesetzt."
type: docs
url: /de/net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Gibt an, ob das führende einfache Anführungszeichen als Teil des Zellwertes betrachtet werden soll. Standard ist true. Ist es false, wird das führende einfache Anführungszeichen aus dem Wert der entsprechenden Zelle entfernt und [`QuotePrefix`](../../style/quoteprefix/) wird für die Zelle auf true gesetzt.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Beispiele

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
            // Erstelle Beispieldaten im CSV-Format mit Anführungszeichen‑Präfixen
            string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
            string filePath = "test.csv";

            // Speichere die CSV‑Daten in einer Datei
            File.WriteAllText(filePath, csvData);

            // Szenario 1: TreatQuotePrefixAsValue = false (Standard)
            var loadOptions1 = new TxtLoadOptions();
            loadOptions1.TreatQuotePrefixAsValue = false;
            
            var workbook1 = new Workbook(filePath, loadOptions1);
            var worksheet1 = workbook1.Worksheets[0];
            Console.WriteLine("TreatQuotePrefixAsValue = false:");
            Console.WriteLine("Cell B2 value: " + worksheet1.Cells["B2"].Value); // Will show 'Apple (quote treated as formatting)

            // Szenario 2: TreatQuotePrefixAsValue = true
            var loadOptions2 = new TxtLoadOptions();
            loadOptions2.TreatQuotePrefixAsValue = true;
            
            var workbook2 = new Workbook(filePath, loadOptions2);
            var worksheet2 = workbook2.Worksheets[0];
            Console.WriteLine("\nTreatQuotePrefixAsValue = true:");
            Console.WriteLine("Cell B2 value: " + worksheet2.Cells["B2"].Value); // Will show 'Apple (quote treated as value)

            // Aufräumen
            File.Delete(filePath);
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


