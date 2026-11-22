---
title: "تعداد FormatConditionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.FormatConditionType. نوع قاعدة التنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

نوع قاعدة التنسيق الشرطي.

```csharp
public enum FormatConditionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| CellValue | `1` | قواعد التنسيق الشرطي هذه تقارن قيمة خلية بنتيجة معادلة محسوبة، باستخدام عامل. |
| Expression | `2` | قواعد التنسيق الشرطي هذه تحتوي على معادلة للتقييم. عندما تكون نتيجة المعادلة صحيحة، يتم تمييز الخلية. |
| Top10 | `4` | قواعد التنسيق الشرطي هذه تبرز الخلايا التي تقع قيمها في الفئة العليا N أو الفئة السفلى N، حسب التحديد. |
| UniqueValues | `8` | قواعد التنسيق الشرطي هذه تبرز القيم الفريدة في النطاق. |
| DuplicateValues | `16` | قواعد التنسيق الشرطي هذه تبرز القيم المكررة. |
| ContainsText | `32` | قواعد التنسيق الشرطي هذه تبرز الخلايا التي تحتوي على النص المحدد. يعادل استخدام دالة SEARCH() في الورقة لتحديد ما إذا كانت الخلية تحتوي على النص. |
| NotContainsText | `64` | قواعد التنسيق الشرطي هذه تبرز الخلايا التي لا تحتوي على النص المحدد. يعادل استخدام دالة SEARCH() في الورقة لتحديد ما إذا كانت الخلية تحتوي على النص أم لا. |
| BeginsWith | `128` | قواعد التنسيق الشرطي هذه تبرز الخلايا في النطاق التي تبدأ بالنص المحدد. يعادل استخدام دالة LEFT() في الورقة ومقارنة القيم. |
| EndsWith | `256` | قواعد التنسيق الشرطي هذه تبرز الخلايا التي تنتهي بالنص المحدد. يعادل استخدام دالة RIGHT() في الورقة ومقارنة القيم. |
| ContainsBlanks | `512` | قواعد التنسيق الشرطي هذه تبرز الخلايا التي تكون فارغة تمامًا. يعادل استخدام LEN(TRIM()). هذا يعني أنه إذا كانت الخلية تحتوي فقط على أحرف سيزيلها TRIM()، فإنها تُعتبر فارغة. الخلية الفارغة أيضًا تُعتبر فارغة. |
| NotContainsBlanks | `1024` | قواعد التنسيق الشرطي هذه تبرز الخلايا التي ليست فارغة. يعادل استخدام LEN(TRIM()). هذا يعني أنه إذا كانت الخلية تحتوي فقط على أحرف سيزيلها TRIM()، فإنها تُعتبر فارغة. الخلية الفارغة أيضًا تُعتبر فارغة. |
| ContainsErrors | `2048` | قواعد التنسيق الشرطي هذه تبرز الخلايا التي تحتوي على أخطاء في الصيغة. يعادل استخدام دالة ISERROR() في الورقة لتحديد ما إذا كان هناك خطأ في الصيغة. |
| NotContainsErrors | `4096` | قواعد التنسيق الشرطي هذه تبرز الخلايا التي لا تحتوي على أخطاء في الصيغة. يعادل استخدام دالة ISERROR() في الورقة لتحديد ما إذا كان هناك خطأ في الصيغة. |
| TimePeriod | `8192` | تُبرز قاعدة التنسيق الشرطي هذه الخلايا التي تحتوي على تواريخ في الفترة الزمنية المحددة. يتم تقييم القيمة الأساسية للخلية، وبالتالي لا تحتاج الخلية إلى أن تكون مُنسقة كتاريخ لتُقيم. على سبيل المثال، مع خلية تحتوي على القيمة 38913 سيتم تطبيق التنسيق الشرطي إذا كانت القاعدة تتطلب قيمة 7/14/2006. |
| AboveAverage | `16384` | تُبرز قاعدة التنسيق الشرطي هذه الخلايا التي تكون أعلى أو أقل من المتوسط لجميع القيم في النطاق. |
| ColorScale | `32768` | تنشئ قاعدة التنسيق الشرطي هذه مقياس ألوان متدرج على الخلايا. |
| DataBar | `65536` | تعرض قاعدة التنسيق الشرطي هذه شريط بيانات متدرج في نطاق الخلايا. |
| IconSet | `131072` | تطبق قاعدة التنسيق الشرطي هذه أيقونات على الخلايا وفقًا لقيمها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionTypeDemo
    {
        public static void FormatConditionTypeExample()
        {
            // إنشاء مصنف جديد.
            Workbook workbook = new Workbook();

            // احصل على ورقة العمل الأولى.
            Worksheet worksheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // يحدد نطاق التنسيق الشرطي.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // يضيف شرطًا لـ AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // تعيين الخصائص لـ AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // يضيف شرطًا لـ CellValue
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // يضيف شرطًا لـ ContainsText
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // احفظ ملف Excel
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


