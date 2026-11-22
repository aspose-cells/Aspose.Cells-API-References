---
title: "Row.IsHeightMatched"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الصف. تشير إلى ما إذا كان ارتفاع الصف يطابق إعداد الخط الافتراضي الحالي لدفتر العمل. قيمة true لهذه الخاصية تعني أيضًا أن ارتفاع الصف تلقائي دون قيمة ارتفاع مخصصة يحددها المستخدم."
type: docs
url: /ar/net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

يشير إلى ما إذا كان ارتفاع الصف يتطابق مع إعداد الخط الافتراضي الحالي لدفتر العمل. قيمة true لهذه الخاصية تعني أيضًا أن ارتفاع الصف "تلقائي" دون قيمة ارتفاع مخصصة تم تعيينها من قبل المستخدم.

```csharp
public bool IsHeightMatched { get; set; }
```

### ملاحظات

عندما تكون هذه الخاصية true، إذا تغير المحتوى في هذا الصف، عادةً ما يحتاج ارتفاع الصف إلى إعادة حسابه (مثلًا باستخدام [`AutoFitRows`](../../worksheet/autofitrows/)) للحصول على نفس النتيجة كما هو معروض في مايكروسوفت إكسل عند فتح دفتر العمل فيه.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHeightMatchedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين بيانات وعينة ونمط لتوضيح مطابقة ارتفاع الصف
            worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
            worksheet.Cells["B1"].PutValue("Another cell in the same row");
            
            // تطبيق التفاف النص لإجبار تعديل الارتفاع
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            
            // ضبط الصف تلقائيًا لمطابقة ارتفاع المحتوى
            worksheet.AutoFitRow(0);
            
            // تحقق مما إذا كان ارتفاع الصف يطابق محتواه
            Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


