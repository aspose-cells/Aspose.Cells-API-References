---
title: "WorkbookSettings.DataExtractLoad"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان التطبيق قد فتح الدفتر مؤخرًا لاستعادة البيانات"
type: docs
url: /ar/net/aspose.cells/workbooksettings/dataextractload/
---
## WorkbookSettings.DataExtractLoad property

يشير إلى ما إذا كان التطبيق قد فتح المصنف آخر مرة لاستعادة البيانات.

```csharp
public bool DataExtractLoad { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDataExtractLoadDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تكوين إعدادات الدفتر
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;
            
            // احفظ المصنف
            string destPath = "output.xlsx";
            workbook.Save(destPath);
            
            // إعادة تحميل الدفتر للتحقق من الإعدادات
            Workbook loadedWorkbook = new Workbook(destPath);
            
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


