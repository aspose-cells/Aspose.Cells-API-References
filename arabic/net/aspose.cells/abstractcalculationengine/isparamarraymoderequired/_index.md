---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractCalculationEngine. تشير إلى ما إذا كان هذا المحرك يحتاج إلى حساب المعامل في وضع المصفوفة. القيمة الافتراضية هي false. إذا كان GetParamValueInArrayMode مطلوبًا عند حساب الدوال المخصصة ولم يقم المستخدم بتحديث التعريف لها عبر UpdateCustomFunctionDefinition، يجب تعيين هذه الخاصية إلى true."
type: docs
url: /ar/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

تشير إلى ما إذا كان هذا المحرك يحتاج إلى حساب المعامل في وضع المصفوفة. القيمة الافتراضية هي false. إذا كان [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) مطلوبًا عند حساب الدوال المخصصة ولم يقم المستخدم بتحديث التعريف لها (عن طريق [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/))، يجب تعيين هذه الخاصية إلى true.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### ملاحظات

إذا كان محرك الحساب المخصص هذا يحتاج إلى حساب المعامل في وضع المصفوفة، سيتطلب المزيد من المكدسات لتخزين شجرة المعاملات وقد يتم استدعاء طريقة Calculate() بشكل متكرر لحساب قيمة المعامل. لأسباب تتعلق بالأداء، يرجى إبقاء هذه الخاصية على القيمة الافتراضية (false) إذا لم يكن هناك أي متطلبات خاصة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamArrayModeRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomCalculationEngine engine = new CustomCalculationEngine();
            Console.WriteLine("IsParamArrayModeRequired: " + engine.IsParamArrayModeRequired);

            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].Formula = "=SUMARRAY(A1,A2)";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            Console.WriteLine("SUMARRAY result: " + worksheet.Cells["A3"].Value);

            workbook.Save("IsParamArrayModeRequiredDemo.xlsx");
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override bool IsParamArrayModeRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUMARRAY")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(i);

                    double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));

                    sum += param1;
                }
                data.CalculatedValue = sum;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            return false;
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


