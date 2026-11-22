---
title: "ExportTableOptions.SkipErrorValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportTableOptions. تشير إلى ما إذا كان سيتم تخطي القيمة غير الصالحة للعمود. على سبيل المثال إذا كان نوع العمود decimal وكانت القيمة أكبر من decimal.MaxValue وكانت هذه الخاصية true فلن نرمي استثناءً مرة أخرى. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/skiperrorvalue/
---
## ExportTableOptions.SkipErrorValue property

يشير إلى ما إذا كان يتم تخطي القيمة غير الصالحة للعمود. على سبيل المثال، إذا كان نوع العمود decimal والقيمة أكبر من decimal.MaxValue وهذه الخاصية true، لن نرمي استثناءً مرة أخرى. القيمة الافتراضية هي false.

```csharp
public bool SkipErrorValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertySkipErrorValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;

            Worksheet ws = wb.Worksheets[0];

            // حالة الاختبار الأولى - القيم الرقمية
            ws.Cells["A1"].Value = "Double";
            ws.Cells["A2"].Value = 1.56;

            ExportTableOptions eto = new ExportTableOptions();
            eto.ExportColumnName = true;
            eto.SkipErrorValue = true;
            eto.CheckMixedValueType = true;

            DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[0][0] is string)); // Should be False
            Console.WriteLine("Value: " + data.Rows[0][0]); // Should be 1.56

            // حالة الاختبار الثانية - القيم المختلطة
            ws.Cells["A2"].Value = "dummy";
            ws.Cells["A3"].Value = 1.56;

            data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"

            // حالة الاختبار الثالثة - تصدير كسلسلة
            data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
        }
    }
}
```

### انظر أيضًا

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


