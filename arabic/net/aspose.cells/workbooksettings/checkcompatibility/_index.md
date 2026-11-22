---
title: "WorkbookSettings.CheckCompatibility"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان يتم فحص التوافق مع الإصدارات السابقة عند حفظ المصنف"
type: docs
url: /ar/net/aspose.cells/workbooksettings/checkcompatibility/
---
## WorkbookSettings.CheckCompatibility property

يشير إلى ما إذا كان يتم فحص التوافق مع الإصدارات السابقة عند حفظ المصنف.

```csharp
public bool CheckCompatibility { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true. فقط لملفات Excel97-2003 xls أو xlt.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCompatibilityDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعيين CheckCompatibility إلى true وحفظ
            workbook.Settings.CheckCompatibility = true;
            workbook.Save("CheckCompatibilityDemo_true.xlsx");
            
            // أعد التحميل وتحقق
            workbook = new Workbook("CheckCompatibilityDemo_true.xlsx");
            Console.WriteLine("CheckCompatibility (true): " + workbook.Settings.CheckCompatibility);
            
            // تعيين CheckCompatibility إلى false وحفظ
            workbook.Settings.CheckCompatibility = false;
            workbook.Save("CheckCompatibilityDemo_false.xlsx");
            
            // أعد التحميل وتحقق
            workbook = new Workbook("CheckCompatibilityDemo_false.xlsx");
            Console.WriteLine("CheckCompatibility (false): " + workbook.Settings.CheckCompatibility);
            
            // إظهار عمليات اللون
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color customColor = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
            Console.WriteLine("Matching color R value: " + customColor.R);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


