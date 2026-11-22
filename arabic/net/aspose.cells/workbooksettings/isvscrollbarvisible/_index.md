---
title: "WorkbookSettings.IsVScrollBarVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. يحصل أو يضبط قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير عمودي"
type: docs
url: /ar/net/aspose.cells/workbooksettings/isvscrollbarvisible/
---
## WorkbookSettings.IsVScrollBarVisible property

يحصل أو يضبط قيمة تشير إلى ما إذا كان جدول البيانات المُولد سيحتوي على شريط تمرير عمودي.

```csharp
public bool IsVScrollBarVisible { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;
            
            // إخفاء شريط التمرير العمودي
            settings.IsVScrollBarVisible = false;
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


