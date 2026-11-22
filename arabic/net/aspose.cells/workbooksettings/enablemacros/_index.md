---
title: "WorkbookSettings.EnableMacros"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تمكين الماكرو"
type: docs
url: /ar/net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

تمكين الماكرو؛

```csharp
public bool EnableMacros { get; set; }
```

### ملاحظات

الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyEnableMacrosDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = wb.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Macro Test");
            
            // عرض خاصية EnableMacros
            Console.WriteLine("Initial EnableMacros value: " + wb.Settings.EnableMacros);
            
            // تعطيل الماكرو
            wb.Settings.EnableMacros = false;
            Console.WriteLine("After disabling macros: " + wb.Settings.EnableMacros);
            
            // تمكين الماكرو
            wb.Settings.EnableMacros = true;
            Console.WriteLine("After enabling macros: " + wb.Settings.EnableMacros);
            
            // احفظ المصنف
            wb.Save("EnableMacrosDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


