---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractCalculationEngine. Указывает, требуется ли этому движку вычислять параметр в режиме массива. Значение по умолчанию — false. Если при расчёте пользовательских функций требуется GetParamValueInArrayMode, а пользователь не обновил их определение с помощью UpdateCustomFunctionDefinition, это свойство должно быть установлено в true."
type: docs
url: /ru/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Указывает, требуется ли этому движку вычислять параметр в режиме массива. Значение по умолчанию — false. Если [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) требуется при расчёте пользовательских функций, а пользователь не обновил их определение (с помощью [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/)), это свойство должно быть установлено в true.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Примечания

Если этому пользовательскому движку расчёта требуется вычислять параметр в режиме массива, понадобится больше стеков для кэширования дерева параметров, и метод Calculate() может вызываться рекурсивно для вычисления значения параметра. С учётом производительности, пожалуйста, оставьте это свойство со значением по умолчанию (false), если нет особых требований.

### Примеры

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

### См. также

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


