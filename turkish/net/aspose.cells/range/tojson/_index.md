---
title: "Range.ToJson"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Aralığı JSON değerine dönüştür."
type: docs
url: /tr/net/aspose.cells/range/tojson/
---
## Range.ToJson method

Aralığı JSON değerine dönüştür.

```csharp
public string ToJson(JsonSaveOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | JsonSaveOptions | Dönüştürme seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToJsonWithJsonSaveOptionsDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            
            // Örnek veri
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);

            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:B2");

            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;
            
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


