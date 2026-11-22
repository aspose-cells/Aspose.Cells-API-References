---
title: "WorkbookSettings.Password"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تمثل كلمة مرور تشفير ملف دفتر العمل"
type: docs
url: /ar/net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

يمثل كلمة مرور تشفير ملف Workbook.

```csharp
public string Password { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPasswordDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى الورقة الأولى وإضافة بعض البيانات
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["C6"].PutValue("test encrypt.");
            
            // عيّن كلمة المرور لحماية دفتر العمل
            wb.Settings.Password = "xixi";
            
            // احفظ المصنف
            wb.Save("output_with_password.ods");
            
            // أنشئ خيارات التحميل مع كلمة المرور لفتح دفتر العمل المحمي
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "xixi";
            
            // افتح دفتر العمل المحمي بكلمة مرور
            Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
            
            // تحقق من البيانات
            Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


