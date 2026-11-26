---
title: "CalculationData.ParamCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationData. Obtiene el recuento de parámetros"
type: docs
url: /es/net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Obtiene la cantidad de parámetros

```csharp
public int ParamCount { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Poblar algunas celdas que se usarán como parámetros
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // Establecer una fórmula que llame a una función personalizada con tres argumentos
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // Configure las opciones de cálculo para usar un motor personalizado
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // Realizar cálculo
                workbook.CalculateFormula(options);

                // El motor personalizado devuelve ParamCount como el valor calculado
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // Opcionalmente guardar el libro de trabajo
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Motor de cálculo personalizado que demuestra la lectura de la propiedad ParamCount
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Identificar la función personalizada por nombre
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // Leer la propiedad de solo lectura ParamCount
                    int count = data.ParamCount;

                    // Usar el recuento como el resultado de la función
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### Ver también

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


