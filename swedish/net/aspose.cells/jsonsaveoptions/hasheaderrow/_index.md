---
title: "JsonSaveOptions.HasHeaderRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Anger om området innehåller en rubrikrad"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/hasheaderrow/
---
## JsonSaveOptions.HasHeaderRow property

Anger om intervallet innehåller en rubrikrad.

```csharp
public bool HasHeaderRow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till rubrikrad
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            
            // Lägg till datarader
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa område (A1:B3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);

            // Exportera till JSON med HasHeaderRow = true (standard)
            JsonSaveOptions options1 = new JsonSaveOptions();
            options1.HasHeaderRow = true;
            string jsonWithHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options1);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Exportera till JSON med HasHeaderRow = false
            JsonSaveOptions options2 = new JsonSaveOptions();
            options2.HasHeaderRow = false;
            string jsonWithoutHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options2);
            Console.WriteLine("\nJSON without headers:\n" + jsonWithoutHeaders);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


