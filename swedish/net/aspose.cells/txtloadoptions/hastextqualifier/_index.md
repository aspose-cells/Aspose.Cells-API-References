---
title: "TxtLoadOptions.HasTextQualifier"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-egenskap. Om det finns textavgränsare för cellvärde. Standard är true"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

Om det finns textavgränsare för cellvärde. Standard är sant.

```csharp
public bool HasTextQualifier { get; set; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasTextQualifierDemo
    {
        public static void Run()
        {
            // Skapa CSV-innehåll med textavgränsare
            string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
            
            // Spara CSV-innehåll till en temporär fil
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);

            // Skapa TxtLoadOptions med HasTextQualifier satt till true
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Läs in CSV-filen med textavgränsare
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Spara arbetsboken för att demonstrera lyckad inläsning
            workbook.Save("Output.xlsx");

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


