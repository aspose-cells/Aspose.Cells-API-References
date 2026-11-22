---
title: "FormulaSettings.EnableCalculationChain"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. تشير إلى ما إذا كان يجب تمكين سلسلة الحساب للصيغ. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

يشير إلى ما إذا كان يجب تمكين سلسلة الحساب للصيغ. القيمة الافتراضية هي false.

```csharp
public bool EnableCalculationChain { get; set; }
```

### ملاحظات

عندما يكون هناك الكثير من الصيغ في المصنف ويحتاج المستخدم إلى حسابها بشكل متكرر مع تعديل جزء صغير فقط منها، قد يكون تمكين سلسلة الحساب مفيدًا للأداء. من ناحية أخرى، إذا تم تمكين السلسلة، فإن صيانة نموذج السلسلة تتطلب ذاكرة إضافية، كما أنها تتطلب وقت CPU أكثر قليلًا لبعض العمليات الأخرى مثل تغيير قيمة الخلية أو الصيغ. بعد تغيير هذه الخاصية من false إلى true، سيتم تحليل وبناء سلسلة الحساب في وقت أول حساب للمصنف، لذا قد يكون الوقت المطلوب لأول حساب أكثر من الحساب العادي بدون سلسلة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableCalculationChainDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة صيغ نموذجية
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
            
            // تعطيل سلسلة الحساب
            workbook.Settings.FormulaSettings.EnableCalculationChain = false;
            
            // حساب الصيغ
            workbook.CalculateFormula();
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with calculation chain disabled.");
        }
    }
}
```

### انظر أيضًا

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


