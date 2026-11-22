---
title: "WorkbookSettings.ShowTabs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. الحصول أو تعيين قيمة ما إذا كانت علامات تبويب المصنف معروضة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/showtabs/
---
## WorkbookSettings.ShowTabs property

يحصل أو يضبط قيمة ما إذا كانت علامات تبويب Workbook معروضة.

```csharp
public bool ShowTabs { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyShowTabsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إخفاء علامات تبويب الجدول
            workbook.Settings.ShowTabs = false;
            
            // احفظ المصنف
            workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
            
            // إنشاء مصنف آخر لإظهار علامات التبويب
            Workbook workbook2 = new Workbook();
            
            // تأكد من أن علامات التبويب مرئية (القيمة الافتراضية صحيحة)
            workbook2.Settings.ShowTabs = true;
            
            // احفظ المصنف
            workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


