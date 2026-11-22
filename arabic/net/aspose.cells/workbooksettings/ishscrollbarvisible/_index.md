---
title: "WorkbookSettings.IsHScrollBarVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. يحصل أو يضبط قيمة تشير إلى ما إذا كان جدول البيانات المُنشأ سيحتوي على شريط تمرير أفقي"
type: docs
url: /ar/net/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings.IsHScrollBarVisible property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان الجدول الإلكتروني المُنشأ سيحتوي على شريط تمرير أفقي.

```csharp
public bool IsHScrollBarVisible { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;
            
            // إخفاء شريط التمرير الأفقي
            settings.IsHScrollBarVisible = false;
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


