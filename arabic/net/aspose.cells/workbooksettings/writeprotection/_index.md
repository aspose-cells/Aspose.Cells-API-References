---
title: "WorkbookSettings.WriteProtection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. توفر الوصول إلى خيارات حماية الكتابة للدفتر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

يوفر الوصول إلى خيارات حماية الكتابة لدفتر العمل.

```csharp
public WriteProtection WriteProtection { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWriteProtectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // ضبط خصائص حماية الكتابة
            workbook.Settings.WriteProtection.Password = "test123";
            workbook.Settings.WriteProtection.Author = "John Doe";
            workbook.Settings.WriteProtection.RecommendReadOnly = true;

            // احفظ المصنف
            string outputPath = "WriteProtectionDemo.xlsx";
            workbook.Save(outputPath);

            // تحميل المصنف المحفوظ للتحقق من الخصائص
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // إخراج خصائص حماية الكتابة
            Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
            Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
        }
    }
}
```

### انظر أيضًا

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


