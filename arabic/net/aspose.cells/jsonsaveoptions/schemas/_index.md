---
title: "JsonSaveOptions.Schemas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. مخطط json الأصلي لكل ورقة عمل"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/schemas/
---
## JsonSaveOptions.Schemas property

مخطط JSON الأصلي لكل ورقة عمل.

```csharp
public string[] Schemas { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertySchemasDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // بيانات JSON عينة للاستيراد
            string jsonData = @"{
                ""Products"": [
                    {
                        ""ID"": 101,
                        ""Name"": ""Product A"",
                        ""Price"": 99.99
                    }
                ]
            }";

            // استيراد بيانات JSON إلى ورقة العمل
            JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, new JsonLayoutOptions());

            // مخطط عينة للتحقق
            string schema = @"{
                ""$schema"": ""http://json-schema.org/draft-07/schema#"",
                ""type"": ""object"",
                ""properties"": {
                    ""Products"": {
                        ""type"": ""array"",
                        ""items"": {
                            ""type"": ""object"",
                            ""properties"": {
                                ""ID"": { ""type"": ""integer"" },
                                ""Name"": { ""type"": ""string"" },
                                ""Price"": { ""type"": ""number"" }
                            },
                            ""required"": [""ID"", ""Name"", ""Price""]
                        }
                    }
                },
                ""required"": [""Products""]
            }";

            // تكوين خيارات حفظ JSON مع المخطط
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.Schemas = new string[] { schema };
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // حفظ دفتر العمل باستخدام خيارات JSON
            string outputPath = "output_with_schema.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook saved with JSON schema validation.");
        }
    }
}
```

### انظر أيضًا

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


