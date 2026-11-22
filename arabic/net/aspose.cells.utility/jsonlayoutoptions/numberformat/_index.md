---
title: "JsonLayoutOptions.NumberFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLayoutOptions. تحصل وتضبط تنسيق القيمة الرقمية"
type: docs
url: /ar/net/aspose.cells.utility/jsonlayoutoptions/numberformat/
---
## JsonLayoutOptions.NumberFormat property

يحصل ويضبط تنسيق القيمة الرقمية.

```csharp
public string NumberFormat { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // إنشاء سلسلة بيانات JSON
            string jsonData = @"{
                ""Products"": [
                    { ""ID"": 101, ""Price"": 19.95, ""Date"": ""2023-05-15"" },
                    { ""ID"": 102, ""Price"": 29.99, ""Date"": ""2023-06-20"" }
                ]
            }";

            // إنشاء JsonLayoutOptions مع NumberFormat
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                NumberFormat = "0.00",
                DateFormat = "yyyy-MM-dd"
            };

            // إنشاء دفتر عمل من JSON
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(jsonData);
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, layoutOptions);

            // حفظ إلى Excel
            workbook.Save("JsonNumberFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


