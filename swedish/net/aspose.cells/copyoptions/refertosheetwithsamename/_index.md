---
title: "CopyOptions.ReferToSheetWithSameName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CopyOptions property. I ms excel, när du kopierar formler som refererar till andra kalkylblad medan du kopierar ett kalkylblad till ett annat, bör de kopierade formlerna referera till källarboken. Men i vissa situationer kan användaren behöva att de kopierade formlerna refererar till kalkylblad med samma namn i samma arbetsbok, till exempel när dessa kalkylblad har kopierats tidigare innan denna kopieringsoperation, då bör denna egenskap vara sann."
type: docs
url: /sv/net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

I MS Excel, när formler som refererar till andra kalkylblad kopieras samtidigt som ett kalkylblad kopieras till ett annat, bör de kopierade formlerna referera till källarboken. I vissa situationer kan användaren dock behöva att de kopierade formlerna refererar till kalkylblad med samma namn i samma arbetsbok, till exempel när dessa kalkylblad redan har kopierats innan denna kopieringsåtgärd, då bör denna egenskap vara sann.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToSheetWithSameNameDemo
    {
        public static void Run()
        {
            // Skapa en mallarbok med exempeldata
            Workbook templateWorkbook = new Workbook();
            Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
            templateSheet1.Name = "Data";
            templateSheet1.Cells["A1"].PutValue("Value");
            templateSheet1.Cells["A2"].PutValue(10);
            templateSheet1.Cells["A3"].PutValue(20);
            
            Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
            templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";

            // Skapa utdataarbok
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            // Kopiera kalkylblad med ReferToSheetWithSameName aktiverat
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                outputWorkbook.Worksheets.Add(sheet.Name);
                CopyOptions options = new CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
            }

            // Verifiera att formeln refererar till rätt blad
            Console.WriteLine("Formula in output workbook: " + 
                outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
        }
    }
}
```

### Se även

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


