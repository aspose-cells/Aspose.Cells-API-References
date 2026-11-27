---
title: "TxtLoadOptions.SeparatorString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-egenskap. Hämtar och sätter ett strängvärde som separator"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/separatorstring/
---
## TxtLoadOptions.SeparatorString property

Hämtar och anger ett strängvärde som avgränsare.

```csharp
public string SeparatorString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempeldata med anpassad separator
            worksheet.Cells["A1"].PutValue("John&Doe");
            worksheet.Cells["B1"].PutValue("30");
            worksheet.Cells["A2"].PutValue("Jane&Smith");
            worksheet.Cells["B2"].PutValue("25");

            // Spara med anpassad separator
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = "&";
            workbook.Save("output.csv", saveOptions);

            // Läs in med samma separator
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = "&";
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // Verifiera den inlästa datan
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


