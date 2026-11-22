---
title: "JsonLayoutOptions.JsonLayoutOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ JsonLayoutOptions. منشئ تحميل خيارات تخطيط JSON"
type: docs
url: /ar/net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

منشئ لتحميل خيارات تخطيط JSON.

```csharp
public JsonLayoutOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء بيانات JSON نموذجية
            string json = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Address"": {
                    ""Street"": ""123 Main St"",
                    ""City"": ""New York""
                }
            }";

            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تهيئة JsonLayoutOptions باستخدام المُنشئ
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // تعيين الخيارات
            options.ArrayAsTable = true;
            options.IgnoreArrayTitle = false;
            options.IgnoreObjectTitle = false;

            // استيراد بيانات JSON إلى ورقة العمل
            JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);

            // احفظ المصنف
            workbook.Save("JsonImportDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


