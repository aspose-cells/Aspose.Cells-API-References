---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractCalculationEngine. Omite el cálculo de toda la fórmula que hace referencia a la función que se está evaluando actualmente"
type: docs
url: /es/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

Omite el cálculo de toda la fórmula que hace referencia a la función que se está evaluando actualmente.

```csharp
public void SkipCalculation()
```

### Observaciones

Este método puede invocarse en la implementación de [`Calculate`](../calculate/) para omitir el cálculo de toda la fórmula y el valor original de la fórmula se mantendrá sin cambios.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // Crear motor de cálculo personalizado
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // Calcular el libro de trabajo que activará nuestro motor personalizado
                workbook.CalculateFormula(options);

                // Mostrar el resultado (debería omitirse)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // Guarda el libro de trabajo
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
                // Omitir el cálculo de esta fórmula
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### Ver también

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


