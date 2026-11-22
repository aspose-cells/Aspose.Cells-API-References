---
title: "تعداد TxtLoadStyleStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.TxtLoadStyleStrategy. يحدد كيفية تطبيق النمط على القيم المُحلَّلة عند تحويل القيمة النصية إلى رقم أو تاريخ/وقت"
type: docs
url: /ar/net/aspose.cells/txtloadstylestrategy/
---
## TxtLoadStyleStrategy enumeration

يحدد كيفية تطبيق النمط للقيم المُحللة عند تحويل قيمة نصية إلى رقم أو تاريخ/وقت.

```csharp
public enum TxtLoadStyleStrategy
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لا يحدد نمطًا للقيمة المُحلَّلة. |
| BuiltIn | `1` | تعيين النمط كرقم/تاريخ مدمج عندما تكون القيمة المُحلَّلة قيمًا رقمية/تاريخية بسيطة. |
| ExactFormat | `2` | تعيين التنسيق المخصص الدقيق للقيمة المُحلَّلة لجعل القيمة المُنسقة مطابقة للقيمة الأصلية المدخلة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtLoadStyleStrategyDemo
    {
        public static void TxtLoadStyleStrategyExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعريف محتوى CSV نموذجي
            string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";

            // حفظ محتوى CSV إلى ملف مؤقت
            string tempCsvFilePath = "sample.csv";
            System.IO.File.WriteAllText(tempCsvFilePath, csvContent);

            // إنشاء TxtLoadOptions وتعيين LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;

            // تحميل ملف CSV إلى المصنف
            workbook = new Workbook(tempCsvFilePath, loadOptions);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("TxtLoadStyleStrategyExample.xlsx");

            // تنظيف ملف CSV المؤقت
            System.IO.File.Delete(tempCsvFilePath);

            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


