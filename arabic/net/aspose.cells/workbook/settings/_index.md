---
title: "Workbook.Settings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تمثل إعدادات دفتر العمل"
type: docs
url: /ar/net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

يمثل إعدادات المصنف.

```csharp
public WorkbookSettings Settings { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertySettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول وتعديل الإعدادات
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 30;
            workbook.Settings.FormulaSettings.MaxChange = 0.1;

            // تحقق من الإعدادات
            Console.WriteLine("Iterative Calculation Enabled: " + 
                workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + 
                workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + 
                workbook.Settings.FormulaSettings.MaxChange);

            // احفظ المصنف
            workbook.Save("WorkbookSettingsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


