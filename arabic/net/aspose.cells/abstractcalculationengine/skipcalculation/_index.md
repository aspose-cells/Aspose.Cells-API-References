---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractCalculationEngine. تتخطى الحساب للمعادلة بأكملها التي تشير إلى الدالة الحالية قيد التقييم"
type: docs
url: /ar/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

يتخطى الحساب للمعادلة بالكامل التي تشير إلى الدالة التي يتم تقييمها حاليًا.

```csharp
public void SkipCalculation()
```

### ملاحظات

يمكن استدعاء هذه الطريقة في تنفيذ [`Calculate`](../calculate/) لتخطي الحساب للمعادلة بأكملها وسيتم الحفاظ على القيمة الأصلية للمعادلة دون تغيير.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // أنشئ محرك حساب مخصص
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // احسب المصنف الذي سيُشغّل محركنا المخصص
                workbook.CalculateFormula(options);

                // اعرض النتيجة (يجب تخطيها)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // احفظ المصنف
                workbook.Save("SkipCalculationDemo.xlsx");
                Console.WriteLine("SkipCalculation method demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SkipCalculation: {ex.Message}");
            }
        }
    }

    public class CustomSkipEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "SKIPFUNC")
            {
                // تخطي الحساب لهذه المعادلة
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


