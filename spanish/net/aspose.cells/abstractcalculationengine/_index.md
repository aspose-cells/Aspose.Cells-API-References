---
title: "Clase AbstractCalculationEngine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AbstractCalculationEngine. Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells"
type: docs
url: /es/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells.

```csharp
public abstract class AbstractCalculationEngine
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Indica si este motor necesita que el parámetro se calcule en modo de matriz. El valor predeterminado es false. Si se requiere [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) al calcular funciones personalizadas y el usuario no ha actualizado la definición de las mismas (mediante [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/)), esta propiedad debe establecerse en true. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Indica si este motor necesita el texto literal del parámetro durante un cálculo. El valor predeterminado es false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Si las funciones incorporadas que han sido soportadas por el motor interno deben ser verificadas y procesadas por esta implementación. El valor predeterminado es false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Calcula una función con los datos proporcionados. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | Si se debe forzar que la función dada se recalcule siempre al calcular fórmulas compartidas. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | Omite el cálculo de toda la fórmula que hace referencia a la función que se está evaluando actualmente. |

### Observaciones

El usuario no debe modificar ninguna parte del Workbook directamente en esta implementación (excepto el resultado calculado de la función personalizada, que puede establecerse mediante la propiedad CalculationData.CalculatedValue). De lo contrario, pueden producirse resultados inesperados o una excepción. Si el usuario necesita cambiar datos diferentes al resultado calculado en la implementación para algunas funciones personalizadas, por ejemplo, modificar la fórmula de una celda, el estilo, etc., debe recopilar esos datos en esta implementación y modificarlos fuera del ámbito del cálculo de la fórmula.

### Ejemplos

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Ejemplo: Implementación personalizada para una función llamada "MYFUNC"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // Suponiendo que MYFUNC toma dos parámetros y devuelve su suma
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // Forzar recalculación para la función personalizada "MYFUNC"
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Introduzca algunos valores en las celdas
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // Agregue una fórmula que utilice la función personalizada
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // Establezca las opciones de cálculo con el motor personalizado
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // Calcule fórmulas con el motor personalizado
            workbook.CalculateFormula(options);

            // Imprima el resultado de la función personalizada
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // Guarda el libro de trabajo
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


