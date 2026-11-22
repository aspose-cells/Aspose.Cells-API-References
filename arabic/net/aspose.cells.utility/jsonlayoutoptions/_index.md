---
title: "الفئة JsonLayoutOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Utility.JsonLayoutOptions. تمثل خيارات نوع تخطيط json"
type: docs
url: /ar/net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

يمثل خيارات نوع تخطيط json.

```csharp
public class JsonLayoutOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | منشئ لتحميل خيارات تخطيط JSON. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | يعالج المصفوفة كجدول. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | يشير إلى ما إذا كان يتم تحويل السلسلة في json إلى قيمة رقمية أو تاريخية. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | يحصل على ويضبط تنسيق قيمة التاريخ. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يتم تجاهل العنوان إذا كانت المصفوفة خاصية لكائن. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | يشير إلى ما إذا كان يتم تجاهل القيمة الفارغة. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يجب تجاهل العنوان إذا كان الكائن خاصية لكائن آخر. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | يتجاهل عناوين السمات |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | يشير إلى ما إذا كان يتم الاحتفاظ بمخطط هذا json. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | يحصل ويضبط تنسيق القيمة الرقمية. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | يحصل على ويضبط نمط العنوان. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassJsonLayoutOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء JsonLayoutOptions وتعيين الخصائص
            JsonLayoutOptions options = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true,
                IgnoreArrayTitle = false,
                IgnoreObjectTitle = false
            };

            // عينة بيانات JSON
            string jsonData = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Departments"": [""HR"", ""Finance"", ""IT""]
            }";

            // استيراد بيانات JSON إلى ورقة العمل
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);

            // احفظ المصنف
            workbook.Save("JsonLayoutOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


