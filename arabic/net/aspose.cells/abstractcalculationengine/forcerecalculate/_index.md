---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractCalculationEngine. ما إذا كان يجب إجبار الدالة المعطاة على إعادة الحساب دائمًا عند حساب الصيغ المشتركة"
type: docs
url: /ar/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

ما إذا كان يجب إجبار الدالة المعطاة على إعادة حسابها دائمًا عند حساب الصيغ المشتركة.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| functionName | String | اسم الدالة. عادةً ما يكون اسم الدالة المخصصة. إذا كان [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) صحيحًا، فسيتم أيضًا فحص الدوال المدمجة هنا. |

### قيمة الإرجاع

صحيح إذا كانت الدالة المحددة تحتاج إلى إعادة الحساب دائمًا.

### ملاحظات

بالنسبة للصيغ المشتركة، تشترك عدة خلايا في نفس الدالة. إذا كانت معلمات الدالة تبقى نفسها لتلك الخلايا أيضًا، فعمومًا تحتاج هذه الدالة إلى حساب مرة واحدة فقط. لذلك، لأسباب الأداء، نحسب هذا النوع من الدوال مرة واحدة فقط أيضًا (يتم استدعاء [`Calculate`](../calculate/) مرة واحدة فقط، بدلاً من استدعائه بشكل متكرر لكل خلية). ومع ذلك، في تنفيذ المستخدم المخصص، قد تحتاج الدالة، خاصة الدالة المخصصة، إلى حساب مختلف لخلايا مختلفة. إذا كان الأمر كذلك، يجب على المستخدم تجاوز هذه الطريقة لجعلها تُعيد true لهذه الدالة. ولـ [`Calculate`](../calculate/)، قد يكون [`CalculatedValue`](../../calculationdata/calculatedvalue/) المُعطى قد تم تهيئته بقيمة مخزنة من الحساب السابق.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;


    public class AbstractCalculationEngineMethodForceRecalculateWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            MyCustomEngine engine = new MyCustomEngine();
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;

            worksheet.Cells["A1"].Formula = "MYVOLATILEFUNC()";

            try
            {
                bool result = engine.ForceRecalculate("MYVOLATILEFUNC");
                Console.WriteLine($"ForceRecalculate returned: {result} for 'MYVOLATILEFUNC'");

                workbook.CalculateFormula(options);
                Console.WriteLine($"First calculation result: {worksheet.Cells["A1"].Value}");

                System.Threading.Thread.Sleep(1000);
                workbook.CalculateFormula(options);
                Console.WriteLine($"Second calculation result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ForceRecalculate: {ex.Message}");
            }

            workbook.Save("ForceRecalculateDemo.xlsx");
        }
    }


    public class MyCustomEngine : AbstractCalculationEngine
    {
        private int calculationCount = 0;

        public override bool ForceRecalculate(string functionName)
        {
            return functionName == "MYVOLATILEFUNC";
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYVOLATILEFUNC")
            {
                calculationCount++;
                data.CalculatedValue = calculationCount;
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


