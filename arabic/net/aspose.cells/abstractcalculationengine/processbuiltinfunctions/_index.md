---
title: "AbstractCalculationEngine.ProcessBuiltInFunctions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractCalculationEngine. ما إذا كان يجب فحص ومعالجة الدوال المدمجة التي يدعمها المحرك المدمج من قبل هذا التنفيذ. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/abstractcalculationengine/processbuiltinfunctions/
---
## AbstractCalculationEngine.ProcessBuiltInFunctions property

ما إذا كان يجب فحص ومعالجة الدوال المدمجة التي يدعمها المحرك المدمج بواسطة هذا التنفيذ. القيمة الافتراضية هي false.

```csharp
public virtual bool ProcessBuiltInFunctions { get; }
```

### ملاحظات

إذا كان المستخدم يحتاج إلى تغيير منطق الحساب لبعض الدوال المدمجة، يجب تعيين هذه الخاصية إلى true. وإلا يرجى ترك هذه الخاصية كـ false لأسباب تتعلق بالأداء.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyProcessBuiltInFunctionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ بيانات الاختبار
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // أنشئ محركات حساب مخصصة بقيم مختلفة لخاصية ProcessBuiltInFunctions
            CustomEngine engineProcessEnabled = new CustomEngine(true);
            CustomEngine engineProcessDisabled = new CustomEngine(false);

            // اعرض قيم الخاصية
            Console.WriteLine("Engine1 ProcessBuiltInFunctions: " + engineProcessEnabled.ProcessBuiltInFunctions);
            Console.WriteLine("Engine2 ProcessBuiltInFunctions: " + engineProcessDisabled.ProcessBuiltInFunctions);

            // احسب باستخدام محرك مخصص (ProcessBuiltInFunctions = true)
            CalculationOptions optionsEnabled = new CalculationOptions { CustomEngine = engineProcessEnabled };
            workbook.CalculateFormula(optionsEnabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=true: " + worksheet.Cells["A4"].Value);

            // احسب باستخدام محرك مخصص (ProcessBuiltInFunctions = false)
            CalculationOptions optionsDisabled = new CalculationOptions { CustomEngine = engineProcessDisabled };
            workbook.CalculateFormula(optionsDisabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=false: " + worksheet.Cells["A4"].Value);

            workbook.Save("ProcessBuiltInFunctionsDemo.xlsx");
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        private readonly bool _processBuiltIn;

        public CustomEngine(bool processBuiltIn)
        {
            _processBuiltIn = processBuiltIn;
        }

        public override bool ProcessBuiltInFunctions => _processBuiltIn;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("SUM", StringComparison.OrdinalIgnoreCase) && ProcessBuiltInFunctions)
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object param = data.GetParamValue(i);
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);

                    for (int r = paramArea1.StartRow; r <= paramArea1.EndRow; r++)
                    {
                        for (int c = paramArea1.StartColumn; c <= paramArea1.EndColumn; c++)
                        {
                            object cellValue = paramArea1.GetValue(r, c);
                            sum += Convert.ToDouble(cellValue);
                        }
                    }
                    
                }
                data.CalculatedValue = sum * 2; // Custom SUM implementation doubles the result
            }
            // تتم معالجة الدوال الأخرى بواسطة المحرك الافتراضي
        }

        public override bool ForceRecalculate(string functionName) => false;
    }
}
```

### انظر أيضًا

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


