---
title: "WorkbookSettings.FirstVisibleTab"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل أو تعين علامة تبويب ورقة العمل الأولى الظاهرة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/firstvisibletab/
---
## WorkbookSettings.FirstVisibleTab property

يحصل أو يعيّن أول تبويب ورقة عمل مرئي.

```csharp
public int FirstVisibleTab { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFirstVisibleTabDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض أوراق العمل
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // عيّن فهرس علامة التبويب الأولى الظاهرة (0-قائم على)
            workbook.Settings.FirstVisibleTab = 1;
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // تحقق من الإعداد
            Console.WriteLine("First visible tab index: " + workbook.Settings.FirstVisibleTab);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


