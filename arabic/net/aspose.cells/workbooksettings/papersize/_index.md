---
title: "WorkbookSettings.PaperSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل وتضبط حجم ورق الطباعة الافتراضي"
type: docs
url: /ar/net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

يحصل أو يضبط حجم ورق الطباعة الافتراضي.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### ملاحظات

إذا لم يكن هناك إعداد لحجم الورق، سيستخدم MS Excel إعداد الطابعة الافتراضية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // عيّن حجم الورق إلى A5
            workbook.Settings.PaperSize = PaperSizeType.PaperA5;
            
            // تحقق من ضبط حجم الورق بشكل صحيح في ورقة العمل الأولى
            Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


