---
title: "TxtSaveOptions.SeparatorString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions-egenskap. Hämtar och sätter ett strängvärde som separator"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/separatorstring/
---
## TxtSaveOptions.SeparatorString property

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
    public class TxtSaveOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till testdata
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue(2);

            // Spara med mellanslag som separator
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = " ";
            workbook.Save("output_space.txt", saveOptions);

            // Spara med lodstreck som separator
            saveOptions.SeparatorString = "|";
            workbook.Save("output_pipe.txt", saveOptions);

            // Läs in den mellanslagsskilta filen för att verifiera
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = " ";
            Workbook loadedWorkbook = new Workbook("output_space.txt", loadOptions);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;

            Console.WriteLine("Space-separated values:");
            Console.WriteLine($"{cells["A1"].StringValue} {cells["B1"].StringValue}");
            Console.WriteLine($"{cells["A2"].StringValue} {cells["B2"].StringValue}");
            Console.WriteLine($"{cells["A3"].IntValue} {cells["B3"].IntValue}");
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


