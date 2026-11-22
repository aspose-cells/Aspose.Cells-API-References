---
title: "WorkbookSettings.SignificantDigitsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل وتعيّن نوع الأرقام ذات الدقة المهمة لإخراج القيم الرقمية في هذا المصنف. القيمة الافتراضية هي SignificantDigitsType"
type: docs
url: /ar/net/aspose.cells/workbooksettings/significantdigitstype/
---
## WorkbookSettings.SignificantDigitsType property

تحصل وتعيّن نوع الأرقام ذات الدقة المهمة لإخراج القيم الرقمية في هذا المصنف. القيمة الافتراضية هي [`SignificantDigitsType`](../../cellshelper/significantdigitstype/).

```csharp
public SignificantDigitsType SignificantDigitsType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // اعرض قيمة SignificantDigitsType الحالية
            Console.WriteLine("Current SignificantDigitsType: " + settings.SignificantDigitsType);

            // أظهر تعيين قيم مختلفة لـ SignificantDigitsType
            settings.SignificantDigitsType = SignificantDigitsType.Digits15;
            Console.WriteLine("After setting to Digits15: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.G17;
            Console.WriteLine("After setting to G17: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.Rounding17;
            Console.WriteLine("After setting to Rounding17: " + settings.SignificantDigitsType);

            // أضف بعض البيانات الرقمية لتوضيح التأثير
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(123.4567890123456789);
            worksheet.Cells["A2"].PutValue(9876543210.123456789);

            // احفظ المصنف
            workbook.Save("SignificantDigitsTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with SignificantDigitsType settings.");
        }
    }
}
```

### انظر أيضًا

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


