---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractCalculationEngine. Indica si este motor necesita que el parámetro se calcule en modo de matriz. El valor predeterminado es false. Si GetParamValueInArrayMode es necesario al calcular funciones personalizadas y el usuario no ha actualizado la definición de ellas mediante UpdateCustomFunctionDefinition, esta propiedad debe establecerse en true"
type: docs
url: /es/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Indica si este motor necesita que el parámetro se calcule en modo de matriz. El valor predeterminado es false. Si [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) es necesario al calcular funciones personalizadas y el usuario no ha actualizado la definición de ellas (mediante [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/)), esta propiedad debe establecerse en true.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Observaciones

Si este motor de cálculo personalizado necesita que el parámetro se calcule en modo de matriz, se requerirán más pilas para almacenar en caché el árbol de parámetros y el método Calculate() puede llamarse recursivamente para calcular el valor del parámetro. Por consideraciones de rendimiento, mantenga esta propiedad con el valor predeterminado (false) si no hay requisitos especiales.

### Ejemplos

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

### Ver también

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


