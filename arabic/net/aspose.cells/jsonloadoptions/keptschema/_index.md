---
title: "JsonLoadOptions.KeptSchema"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLoadOptions. تشير إلى ما إذا كان يتم الحفاظ على مخطط هذا json"
type: docs
url: /ar/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

يشير إلى ما إذا كان يتم الاحتفاظ بمخطط هذا json.

```csharp
public bool KeptSchema { get; set; }
```

### ملاحظات

أحيانًا نقوم بحفظ الملف إلى JSON بعد تحميل ملف JSON.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل JSON
            JsonLoadOptions options = new JsonLoadOptions();

            // عرض القيمة الافتراضية لخاصية KeptSchema
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // تعيين KeptSchema إلى true
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // إنشاء ملف JSON تجريبي
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // تحميل JSON مع تمكين KeptSchema
                Workbook workbook = new Workbook("sample.json", options);

                // عرض معلومات حول دفتر العمل المحمّل
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // احفظ المصنف
                workbook.Save("KeptSchemaOutput.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


