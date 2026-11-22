---
title: "WorkbookSettings.RepairLoad"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان التطبيق قد فتح المصنف في وضع آمن أو وضع إصلاح في المرة الأخيرة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

يشير إلى ما إذا كان التطبيق قد فتح المصنف آخر مرة في وضع الأمان أو الإصلاح.

```csharp
public bool RepairLoad { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRepairLoadDemo
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
            string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
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


