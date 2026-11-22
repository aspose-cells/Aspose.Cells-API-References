---
title: "WorkbookSettings.SignificantDigits"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل وتضبط عدد الأرقام ذات الدقة. القيمة الافتراضية هي SignificantDigits"
type: docs
url: /ar/net/aspose.cells/workbooksettings/significantdigits/
---
## WorkbookSettings.SignificantDigits property

تحصل وتضبط عدد الأرقام ذات الدقة. القيمة الافتراضية هي [`SignificantDigits`](../../cellshelper/significantdigits/).

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```

### ملاحظات

يمكن أن يكون الآن 15 أو 17 فقط. ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام [`SignificantDigitsType`](../significantdigitstype/). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات رقمية نموذجية لتوضيح الأرقام ذات الدقة
            sheet.Cells["A1"].PutValue(123.4567890123456789);
            sheet.Cells["A2"].PutValue(0.000000000123456789);

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // تعيين الأرقام ذات الدقة إلى 15 (أقصى دقة للنوع double)
            settings.SignificantDigits = 15;

            // حفظ المصنف لإظهار تأثير الأرقام ذات الدقة
            workbook.Save("SignificantDigitsDemo.xlsx");

            Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


