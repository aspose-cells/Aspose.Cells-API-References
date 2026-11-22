---
title: "CalculationData.GetParamValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CalculationData. تحصل على كائن القيمة الممثلة للمعامل عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

يحصل على كائن القيمة الممثلة للمعامل عند فهرس معين.

```csharp
public object GetParamValue(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس المعامل (بدءًا من 0) |

### قيمة الإرجاع

القيمة المحسوبة للمعامل.

### ملاحظات

لمعامل واحد:

إذا كان قيمة عادية، فستُعيد القيمة العادية نفسها؛

إذا كان إشارة، فستُعيد كائن ReferredArea؛

إذا كان يشير إلى مجموعة بيانات (مجموعات بيانات) ذات قيم متعددة، فستُعيد مصفوفة من الكائنات؛

إذا كان نوعًا من التعبير يحتاج إلى حساب، فسيتم حسابه في وضع القيمة وعادةً ما يتم إرجاع قيمة واحدة وفقًا لقاعدة الخلية الحالية. على سبيل المثال، إذا كان أحد معاملات صيغة D2 هو A:A+B:B، فسيتم حساب A2+B2 وإرجاعه. ومع ذلك، إذا تم تحديد هذا المعامل في وضع المصفوفة (عن طريق [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) أو [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/))، فستُرجع مصفوفة (object[][]) تحتوي على العناصر A1+B1،A2+B2،....

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://localhost:9090\", \"Target\")";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new HyperlinkCalculationEngine();
            workbook.CalculateFormula(options);
        }

        class HyperlinkCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName.Equals("HYPERLINK", StringComparison.OrdinalIgnoreCase))
                {
                    Console.WriteLine("URL Parameter: " + data.GetParamValue(0));
                    Console.WriteLine("Display Text: " + data.GetParamValue(1));
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


