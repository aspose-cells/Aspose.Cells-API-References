---
title: "FormulaSettings.PrecisionAsDisplayed"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. تشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب الصيغ"
type: docs
url: /ar/net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

يشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب الصيغ.

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // اضبط PrecisionAsDisplayed على true
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // حدد تنسيق العرض للخلية A1 لعرض منزلتين عشريتين
            cells["A1"].PutValue(1.23456);
            Style style = cells["A1"].GetStyle();
            style.Number = 2; // Format: 0.00
            cells["A1"].SetStyle(style);
            
            // ضع صيغة في الخلية B1 تشير إلى A1
            cells["B1"].Formula = "=A1";
            
            // احسب الصيغ مع تمكين PrecisionAsDisplayed
            workbook.CalculateFormula();
            
            // إخراج النتائج
            Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
            Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
        }
    }
}
```

### انظر أيضًا

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


