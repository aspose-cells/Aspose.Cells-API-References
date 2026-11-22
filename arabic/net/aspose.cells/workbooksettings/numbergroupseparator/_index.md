---
title: "WorkbookSettings.NumberGroupSeparator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل أو تعين الحرف الذي يفصل مجموعات الأرقام إلى يسار الفاصلة العشرية في القيم الرقمية. الافتراضي هو فاصل المجموعات للمنطقة الحالية"
type: docs
url: /ar/net/aspose.cells/workbooksettings/numbergroupseparator/
---
## WorkbookSettings.NumberGroupSeparator property

يحصل أو يضبط الحرف الذي يفصل مجموعات الأرقام إلى يسار الفاصل العشري في القيم الرقمية. الافتراضي هو فاصل المجموعات للمنطقة الحالية.

```csharp
public char NumberGroupSeparator { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyNumberGroupSeparatorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            wb.Settings.NumberDecimalSeparator = ',';
            wb.Settings.NumberGroupSeparator = '.';
            
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00";
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(12345.6798);
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


