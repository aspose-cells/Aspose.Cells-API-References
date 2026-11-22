---
title: "WorkbookSettings.IsHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان هذا المصنف مخفيًا"
type: docs
url: /ar/net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

يشير إلى ما إذا كان هذا المصنف مخفيًا.

```csharp
public bool IsHidden { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // عيّن خاصية IsHidden إلى true
            settings.IsHidden = true;
            Console.WriteLine("Workbook is hidden: " + settings.IsHidden);

            // احفظ المصنف
            workbook.Save("WorkbookSettings_IsHidden_True.xlsx");

            // أنشئ مصنفًا آخر
            Workbook workbook2 = new Workbook();

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings2 = workbook2.Settings;

            // عيّن خاصية IsHidden إلى false (الافتراضي)
            settings2.IsHidden = false;
            Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);

            // احفظ المصنف
            workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");

            // حمّل وتحقق من المصنفات المحفوظة
            Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
            Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);

            Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
            Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


