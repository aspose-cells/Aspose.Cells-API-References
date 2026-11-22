---
title: "FormulaSettings.MaxChange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. الحد الأقصى للتغيير لحل مرجع دائري"
type: docs
url: /ar/net/aspose.cells/formulasettings/maxchange/
---
## FormulaSettings.MaxChange property

الحد الأقصى للتغيير لحل مرجع دائري.

```csharp
public double MaxChange { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxChangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إعداد إعدادات الحساب التكراري
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001; // Set maximum change threshold
            
            // إنشاء مرجع دائري للتوضيح
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // احسب الصيغ باستخدام إعداد MaxChange المحدد
            workbook.CalculateFormula();
            
            // إخراج النتائج
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("MaxChange used: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### انظر أيضًا

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


