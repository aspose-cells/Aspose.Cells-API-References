---
title: "JsonUtility.ExportRangeToJson"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة JsonUtility. تصدير النطاق إلى ملف json"
type: docs
url: /ar/net/aspose.cells.utility/jsonutility/exportrangetojson/
---
## ExportRangeToJson(Range, ExportRangeToJsonOptions) {#exportrangetojson_1}

تصدير النطاق إلى ملف json.

```csharp
[Obsolete("Use ExportRangeToJson(Range range, JsonSaveOptions options) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ExportRangeToJson(Range range, ExportRangeToJsonOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | النطاق. |
| خيارات | ExportRangeToJsonOptions | خيارات التصدير. |

### قيمة الإرجاع

قيمة سلسلة json.

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة ExportRangeToJson(Range range, JsonSaveOptions options). سيتم إزالة هذه الخاصية بعد 6 أشهر منذ نوفمبر 2022. تقدم Aspose اعتذارها عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء نطاق يغطي البيانات
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // إنشاء خيارات التصدير
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.ExportAsString = true;

            // تصدير النطاق إلى JSON
            string json = JsonUtility.ExportRangeToJson(range, options);
            
            Console.WriteLine(json);
        }
    }
}
```

### انظر أيضًا

* class [Range](../../../aspose.cells/range/)
* class [ExportRangeToJsonOptions](../../exportrangetojsonoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## ExportRangeToJson(Range, JsonSaveOptions) {#exportrangetojson}

تصدير النطاق إلى ملف json.

```csharp
public static string ExportRangeToJson(Range range, JsonSaveOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | النطاق. |
| خيارات | JsonSaveOptions | خيارات التصدير. |

### قيمة الإرجاع

قيمة سلسلة json.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeJsonSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["C2"].PutValue("New York");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["C3"].PutValue("London");

            // إنشاء نطاق (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 3);
            
            // تكوين خيارات تصدير JSON
            JsonSaveOptions options = new JsonSaveOptions();
            options.ExportEmptyCells = true;
            options.HasHeaderRow = true;
            options.ExportNestedStructure = false;

            // تصدير النطاق إلى JSON
            string jsonOutput = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
            
            // إخراج نتيجة JSON
            Console.WriteLine(jsonOutput);
        }
    }
}
```

### انظر أيضًا

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


