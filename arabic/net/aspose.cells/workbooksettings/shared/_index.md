---
title: "WorkbookSettings.Shared"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل أو تعين قيمة تشير إلى ما إذا كان المصنف مشتركًا"
type: docs
url: /ar/net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

يحصل أو يضبط قيمة تشير إلى ما إذا كان Workbook مشتركًا.

```csharp
public bool Shared { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySharedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook book = new Workbook();
            
            // تعيين خاصية Shared إلى true
            book.Settings.Shared = true;
            
            // احفظ المصنف
            string outputPath = "output_shared.xlsx";
            book.Save(outputPath);
            
            // تحميل المصنف المحفوظ للتحقق من خاصية Shared
            Workbook loadedBook = new Workbook(outputPath);
            Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


