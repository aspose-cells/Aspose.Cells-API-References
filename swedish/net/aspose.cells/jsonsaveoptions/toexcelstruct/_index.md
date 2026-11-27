---
title: "JsonSaveOptions.ToExcelStruct"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Anger om konvertering till JSON‑struktur för Excel‑filen"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

Indikerar om konvertering till json-struktur för Excel-filen.

```csharp
public bool ToExcelStruct { get; set; }
```

### Anmärkningar

Endast för konvertering av område till JSON.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyToExcelStructDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Skapa ett område att exportera
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            // Konfigurera JSON‑sparalternativ med ToExcelStruct
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;

            // Exportera område till JSON
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


