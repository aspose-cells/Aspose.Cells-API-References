---
title: "JsonLayoutOptions.IgnoreNull"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLayoutOptions. تشير إلى ما إذا كان يتم تجاهل القيمة الفارغة"
type: docs
url: /ar/net/aspose.cells.utility/jsonlayoutoptions/ignorenull/
---
## JsonLayoutOptions.IgnoreNull property

يشير إلى ما إذا كان يتم تجاهل القيمة الفارغة.

```csharp
public bool IgnoreNull { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreNullDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // عينة JSON مع قيم فارغة
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": null,
                ""Salary"": 500.00
            }";

            // تكوين خيارات استيراد JSON مع تعيين IgnoreNull إلى true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreNull = true;
            options.NumberFormat = "$0.00";

            // استيراد بيانات JSON إلى ورقة العمل
            JsonUtility.ImportData(json, cells, 0, 0, options);

            // تحقق من البيانات المستوردة (يجب تجاهل العنوان الفارغ)
            Console.WriteLine("Name: " + cells["A2"].StringValue);    // John
            Console.WriteLine("Age: " + cells["B2"].IntValue);        // 30
            Console.WriteLine("Address exists: " + (cells["C2"].Value != null)); // False
            Console.WriteLine("Salary: " + cells["D2"].StringValue);  // $500.00

            // احفظ المصنف
            workbook.Save("JsonIgnoreNullDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


