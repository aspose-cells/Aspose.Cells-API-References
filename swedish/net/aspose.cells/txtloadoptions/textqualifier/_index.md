---
title: "TxtLoadOptions.TextQualifier"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions egenskap. Anger textavgränsaren för cellvärden. Standardavgränsare är"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

Anger textavgränsaren för cellvärden. Standardavgränsaren är '\"'.

```csharp
public char TextQualifier { get; set; }
```

### Anmärkningar

När du ställer in denna egenskap blir [`HasTextQualifier`](../hastextqualifier/) automatiskt sann.

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTextQualifierDemo
    {
        public static void Run()
        {
            // Skapa en instans av TxtLoadOptions för CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Skapa exempel på CSV-data med textavgränsare
            string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
            
            // Spara exempeldata till en temporär fil
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvData);

            // Läs in CSV-filen med de angivna alternativen
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("TextQualifierDemo.xlsx");

            // Rensa upp temporär fil
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


