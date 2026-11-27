---
title: "SaveOptions.ClearData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Gör arbetsboken tom efter att filen har sparats"
type: docs
url: /sv/net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Gör arbetsboken tom efter att filen har sparats.

```csharp
public bool ClearData { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyClearDataDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till testdata
            worksheet.Cells["A1"].PutValue("Tabelle1");
            worksheet.Cells["B3"].PutValue(3);

            // Konfigurera sparalternativ med ClearData = false
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.ClearData = false;
            saveOptions.Separator = ',';

            // Spara arbetsboken
            string outputPath = "output_with_cleardata_false.csv";
            workbook.Save(outputPath, saveOptions);

            // Läs in igen för att verifiera att data bevarades
            Workbook loadedWorkbook = new Workbook(outputPath);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;
            
            Console.WriteLine("A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("B3 value: " + cells["B3"].IntValue);
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


