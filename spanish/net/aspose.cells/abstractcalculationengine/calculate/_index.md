---
title: "AbstractCalculationEngine.Calculate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de AbstractCalculationEngine. Calcula una función con los datos proporcionados"
type: docs
url: /es/net/aspose.cells/abstractcalculationengine/calculate/
---
## AbstractCalculationEngine.Calculate method

Calcula una función con los datos proporcionados.

```csharp
public abstract void Calculate(CalculationData data)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| datos | CalculationData | los datos requeridos para calcular la función, como el nombre de la función, los parámetros, ...etc. |

### Observaciones

El usuario debe establecer el valor calculado para los datos dados para todas las funciones (incluyendo funciones nativas de Excel) que desea calcular por sí mismo en esta implementación.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodCalculateWithCalculationDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].Formula = "=CUSTOMSUM(A1,A2)";
            
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();
            
            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Custom calculation result: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Calculate method: {ex.Message}");
            }
            
            workbook.Save("AbstractCalculationEngineDemo.xlsx");
        }

        class CustomCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName.ToUpper() == "CUSTOMSUM")
                {
                    if (data.ParamCount == 2)
                    {
                        try
                        {
                            Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                            Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                            double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                            double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));

                            data.CalculatedValue = param1 + param2;
                        }
                        catch
                        {
                            data.CalculatedValue = "#VALUE!";
                        }
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [CalculationData](../../calculationdata/)
* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


