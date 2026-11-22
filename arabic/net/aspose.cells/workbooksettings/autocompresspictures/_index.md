---
title: "WorkbookSettings.AutoCompressPictures"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحدد قيمة منطقية تشير إلى أن التطبيق يضغط الصور تلقائيًا في الدفتر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

يحدد قيمة منطقية تشير إلى أن التطبيق يضغط الصور تلقائيًا في دفتر العمل.

```csharp
public bool AutoCompressPictures { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoCompressPicturesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تمكين AutoCompressPictures
            workbook.Settings.AutoCompressPictures = true;
            
            // إضافة صورة عينة لتوضيح الضغط
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحميل الدفتر المحفوظ للتحقق من الإعداد
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


