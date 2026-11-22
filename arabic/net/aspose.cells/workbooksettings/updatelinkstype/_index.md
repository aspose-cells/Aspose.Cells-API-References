---
title: "WorkbookSettings.UpdateLinksType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. يحصل ويضبط كيفية تحديث الروابط الخارجية عند فتح المصنف"
type: docs
url: /ar/net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

يحصل ويضبط كيفية تحديث الروابط الخارجية عند فتح دفتر العمل.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateLinksTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعيين UpdateLinksType إلى Never
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحميل الدفتر المحفوظ للتحقق من الإعداد
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // إخراج قيمة UpdateLinksType
            Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
        }
    }
}
```

### انظر أيضًا

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


