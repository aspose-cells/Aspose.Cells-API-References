---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractCalculationEngine özelliği. Bu motorun parametrenin dizi modunda hesaplanması gerekip gerekmediğini gösterir. Varsayılan değer false. Özel işlevler hesaplanırken GetParamValueInArrayMode gerekli ise ve kullanıcı bunlar için tanımı UpdateCustomFunctionDefinition ile güncellememişse bu özellik true olarak ayarlanmalıdır."
type: docs
url: /tr/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Bu motorun parametrenin dizi modunda hesaplanması gerekip gerekmediğini gösterir. Varsayılan değer false. Özel işlevler hesaplanırken [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) gerekli ise ve kullanıcı bunların tanımını ([`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) ile) güncellememişse, bu özellik true olarak ayarlanmalıdır.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Açıklamalar

Bu özel hesaplama motoru parametrenin dizi modunda hesaplanması gerekiyorsa, parametreler için ağacı önbelleğe almak üzere daha fazla yığın gerekecek ve Calculate() yöntemi parametrenin değerini hesaplamak için özyinelemeli olarak çağrılabilir. Performans düşünülerek, özel bir gereklilik yoksa lütfen bu özelliği varsayılan değer (false) olarak tutun.

### Örnekler

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

### Ayrıca Bakınız

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


