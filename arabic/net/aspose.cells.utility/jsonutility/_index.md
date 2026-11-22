---
title: "الفئة JsonUtility"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Utility.JsonUtility. تمثل الفئة المساعدة لمعالجة json"
type: docs
url: /ar/net/aspose.cells.utility/jsonutility/
---
## JsonUtility class

يمثل فئة المساعدة لمعالجة json.

```csharp
public class JsonUtility
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [JsonUtility](jsonutility/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Obsolete.**) تصدير النطاق إلى ملف json. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | تصدير النطاق إلى ملف json. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | استيراد سلسلة json. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Utility;
    using System;

    public class JsonUtilityDemo
    {
        public static void JsonUtilityExample()
        {
            // إنشاء مثيل من JsonUtility
            JsonUtility jsonUtility = new JsonUtility();

            // نظرًا لأن الفئة JsonUtility لا تحتوي على أي خصائص أو طرق معرفة في JSON،
            // سنوضح إنشاءها واستخدامها المحتمل في السياق.

            // مثال: بافتراض أن JsonUtility قد تُستخدم لمعالجة بيانات JSON بطريقة ما.
            // ملاحظة: الاستخدام الفعلي سيعتمد على الطرق والخصائص المتاحة في الفئة الحقيقية.
            // هنا، نحن فقط نوضح إنشاء الكائن لأنه لا توجد طرق أو خصائص متوفرة.

            Console.WriteLine("JsonUtility instance created successfully.");

            // كود إضافي لتوضيح الاستخدام المحتمل
            // على سبيل المثال، إذا كان لدى JsonUtility طريقة لمعالجة JSON، فقد تبدو هكذا:
            // string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
            // var result = jsonUtility.ProcessJson(jsonString);
            // Console.WriteLine("Processed JSON: " + result);

            // نظرًا لعدم توفر أي طرق، سننهي المثال هنا.
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


