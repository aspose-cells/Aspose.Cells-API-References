---
title: "WorkbookSettings.IsProtected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل على قيمة تشير إلى ما إذا كان هيكل أو نافذة المصنف محمية"
type: docs
url: /ar/net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

يحصل على قيمة تشير إلى ما إذا كانت بنية أو نافذة المصنف محمية.

```csharp
public bool IsProtected { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;
            
            // تحقق مما إذا كان المصنف محميًا
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // حماية المصنف باستخدام كلمة مرور
            settings.Password = "password123";
            
            // التحقق من حالة الحماية
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // حفظ دفتر العمل المحمي
            workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
            
            // فتح المصنف المحمي
            Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            
            // تحقق من حالة الحماية للمصنف المحمَّل
            Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


