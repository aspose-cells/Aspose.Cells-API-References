---
title: "TxtSaveOptions.ExportAllSheets"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions‑egenskap. Anger om alla blad ska exporteras till textfilen. Om den är falsk exporteras endast det aktiva bladet, precis som i MS Excel"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

Anger om alla blad ska exporteras till textfilen. Om falskt exporteras endast det aktiva bladet, precis som i MS Excel.

```csharp
public bool ExportAllSheets { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAllSheetsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med två blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Lägg till exempeldata i båda bladen
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[0].Cells["A2"].PutValue(1);
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
            workbook.Worksheets[1].Cells["A2"].PutValue(2);

            // Spara med ExportAllSheets=false (standard)
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save("output_single_sheet.csv", saveOptions);

            // Spara med ExportAllSheets=true
            saveOptions.ExportAllSheets = true;
            workbook.Save("output_all_sheets.csv", saveOptions);
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


