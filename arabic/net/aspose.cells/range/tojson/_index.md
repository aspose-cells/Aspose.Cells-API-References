---
title: "Range.ToJson"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تحويل النطاق إلى قيمة JSON"
type: docs
url: /ar/net/aspose.cells/range/tojson/
---
## Range.ToJson method

تحويل النطاق إلى قيمة JSON.

```csharp
public string ToJson(JsonSaveOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | JsonSaveOptions | خيارات التحويل |

### أمثلة

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
            
            // بيانات عينة
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

### انظر أيضًا

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


