---
title: "WorkbookSettings.CultureInfo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. يحصل أو يضبط معلومات الثقافة للنظام"
type: docs
url: /ar/net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

يحصل أو يعيّن معلومات الثقافة للنظام.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### ملاحظات

يعيد null إذا لم يتم تعيين معلومات الثقافة ولم يتم تعيين [`Region`](../region/).

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            
            // ضبط المنطقة إلى فرنسا لعرض تغييرات CultureInfo
            wb.Settings.Region = CountryCode.France;
            
            // الحصول على فاصل المجموعات من الثقافة الفرنسية
            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            Console.WriteLine($"French group separator: '{groupSep}'");
            
            // إنشاء نمط بتنسيق مخصص وعرض التنسيق المعدل وفق الثقافة
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00_ ;-#,##0.00";
            Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
            
            // عرض تنسيق الأرقام مع الثقافة الفرنسية
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells["A1"];
            cell.PutValue(123456.78);
            cell.SetStyle(style);
            style.Custom = "# ###,00 €";
            
            Console.WriteLine($"Formatted value: {cell.StringValue}");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


