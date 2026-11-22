---
title: "JsonLoadOptions.LayoutOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLoadOptions. خيارات استيراد json"
type: docs
url: /ar/net/aspose.cells/jsonloadoptions/layoutoptions/
---
## JsonLoadOptions.LayoutOptions property

خيارات استيراد json.

```csharp
public JsonLayoutOptions LayoutOptions { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyLayoutOptionsDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل JSON باستخدام LayoutOptions
            JsonLoadOptions options = new JsonLoadOptions
            {
                LayoutOptions = new JsonLayoutOptions
                {
                    ArrayAsTable = true,
                    IgnoreNull = false,
                    ConvertNumericOrDate = true,
                    NumberFormat = "0.00",
                    DateFormat = "yyyy-MM-dd"
                }
            };

            // إنشاء دفتر عمل جديد ببيانات JSON
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عينة بيانات JSON
            string json = @"{
                ""Products"": [
                    { ""ID"": 1, ""Name"": ""Product A"", ""Price"": 19.99, ""Date"": ""2023-05-15"" },
                    { ""ID"": 2, ""Name"": ""Product B"", ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // استيراد JSON إلى ورقة العمل
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options.LayoutOptions);

            // احفظ المصنف
            workbook.Save("JsonWithLayoutOptions.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


