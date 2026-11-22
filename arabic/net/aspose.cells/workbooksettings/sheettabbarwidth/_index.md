---
title: "WorkbookSettings.SheetTabBarWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. عرض شريط علامات تبويب ورقة العمل بوحدة 1/1000 من عرض النافذة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

عرض شريط علامات تبويب ورقة العمل (بـ 1/1000 من عرض النافذة).

```csharp
public int SheetTabBarWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySheetTabBarWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // ضبط خاصية SheetTabBarWidth
            workbook.Settings.SheetTabBarWidth = 1000;
            
            // احصل على قيمة SheetTabBarWidth واعرضها
            Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


