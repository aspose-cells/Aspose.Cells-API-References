---
title: "Enumeración CalculationPrecisionStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.CalculationPrecisionStrategy enum. Enumera estrategias para manejar la precisión de cálculo. Debido al problema de precisión de la aritmética de punto flotante IEEE 754, algunas fórmulas aparentemente simples pueden no calcularse con el resultado esperado. Por ejemplo, la fórmula 0.450.430.02 al calcular los operandos mediante el operador directamente el resultado no es cero. Para este tipo de problema de precisión, algunas estrategias especiales pueden proporcionar el resultado esperado."
type: docs
url: /es/net/aspose.cells/calculationprecisionstrategy/
---
## CalculationPrecisionStrategy enumeration

Enumera estrategias para manejar la precisión de cálculo. Debido al problema de precisión de la aritmética de punto flotante IEEE 754, algunas fórmulas \"aparentemente simples\" pueden no calcularse con el resultado esperado. Por ejemplo, la fórmula \"=-0.45+0.43+0.02\", al calcular los operandos con el operador '+' directamente, el resultado no es cero. Para este tipo de problema de precisión, algunas estrategias especiales pueden proporcionar el resultado esperado.

```csharp
public enum CalculationPrecisionStrategy
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | No se aplica ninguna estrategia en el cálculo. Al calcular, simplemente use el valor double original como operando y devuelva el resultado directamente. Es lo más eficiente en rendimiento y aplicable a la mayoría de los casos. |
| Round | `1` | Redondea el resultado del cálculo de acuerdo con los dígitos significativos. |
| Decimal | `2` | Utiliza decimal como operandos cuando sea posible. Es lo menos eficiente en rendimiento. |

### Ejemplos

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CalculationPrecisionStrategyDemo
    {
        public static void CalculationPrecisionStrategyExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Formula");
            worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0

            // Establecer opciones de cálculo
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
            };

            // Calcular las fórmulas en la hoja de cálculo
            workbook.CalculateFormula(calcOptions);

            // Obtener el resultado de la fórmula
            double result = worksheet.Cells["A2"].DoubleValue;

            // Mostrar el resultado
            Console.WriteLine("Calculated Result: " + result);

            // Guarda el libro de trabajo
            workbook.Save("CalculationPrecisionStrategyExample.xlsx");
            workbook.Save("CalculationPrecisionStrategyExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


