---
title: "WorkbookSettings.AutoRecover"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان الملف معلمًا للاستعادة التلقائية"
type: docs
url: /ar/net/aspose.cells/workbooksettings/autorecover/
---
## WorkbookSettings.AutoRecover property

يشير إلى ما إذا كان الملف معلمًا للاستعادة التلقائية.

```csharp
public bool AutoRecover { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoRecoverDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعيين AutoRecover وإعدادات أخرى
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // احفظ المصنف
            string outputPath = "WorkbookSettings_AutoRecoverDemo.xlsx";
            workbook.Save(outputPath);

            // تحميل المصنف المحفوظ للتحقق من الإعدادات
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // إخراج الإعدادات إلى وحدة التحكم
            Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
            Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
            Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
            Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


