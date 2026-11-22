---
title: "Workbook.IsLicensed"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تشير إلى ما إذا تم تعيين الترخيص"
type: docs
url: /ar/net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

يشير إلى ما إذا تم ضبط الترخيص.

```csharp
public bool IsLicensed { get; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsLicensedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // عيّن بعض الخصائص الأساسية لتوضيح استخدام دفتر العمل
            wb.Worksheets[0].Name = "Sheet1";
            wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
            
            // تحقق مما إذا كان المصنف مرخصًا
            Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
            
            // توضيح سلوك مختلف بناءً على حالة الترخيص
            if (wb.IsLicensed)
            {
                Console.WriteLine("Running in licensed mode - full features available");
            }
            else
            {
                Console.WriteLine("Running in evaluation mode - watermarks will appear");
            }

            // احفظ إلى تدفق الذاكرة لتوضيح الوظيفة
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


