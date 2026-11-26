---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de AbstractCalculationEngine. Indica si se debe forzar que la función dada se recalcule siempre al calcular fórmulas compartidas"
type: docs
url: /es/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

Si se debe forzar que la función dada se recalcule siempre al calcular fórmulas compartidas.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionName | String | nombre de la función. Generalmente es el nombre de la función personalizada. Si [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) es verdadero, entonces también se comprobarán las funciones incorporadas aquí. |

### Valor de retorno

verdadero si la función especificada necesita recalcularse siempre.

### Observaciones

Para fórmulas compartidas, varias celdas comparten la misma función. Si los parámetros de la función permanecen iguales para esas celdas también, entonces generalmente esta función solo necesita calcularse una vez. Por lo tanto, por razones de rendimiento solo calculamos este tipo de función una vez también ([`Calculate`](../calculate/) se llama solo una vez, en lugar de llamarse repetidamente para cada celda). Sin embargo, para la implementación personalizada del usuario, puede que la función, especialmente la función personalizada, necesite calcularse de manera diferente para distintas celdas. En ese caso, el usuario debe sobrescribir este método para que devuelva verdadero para la función. Y para [`Calculate`](../calculate/), el [`CalculatedValue`](../../calculationdata/calculatedvalue/) proporcionado puede haber sido inicializado con el valor en caché del cálculo anterior.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;


    public class AbstractCalculationEngineMethodForceRecalculateWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            MyCustomEngine engine = new MyCustomEngine();
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;

            worksheet.Cells["A1"].Formula = "MYVOLATILEFUNC()";

            try
            {
                bool result = engine.ForceRecalculate("MYVOLATILEFUNC");
                Console.WriteLine($"ForceRecalculate returned: {result} for 'MYVOLATILEFUNC'");

                workbook.CalculateFormula(options);
                Console.WriteLine($"First calculation result: {worksheet.Cells["A1"].Value}");

                System.Threading.Thread.Sleep(1000);
                workbook.CalculateFormula(options);
                Console.WriteLine($"Second calculation result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ForceRecalculate: {ex.Message}");
            }

            workbook.Save("ForceRecalculateDemo.xlsx");
        }
    }


    public class MyCustomEngine : AbstractCalculationEngine
    {
        private int calculationCount = 0;

        public override bool ForceRecalculate(string functionName)
        {
            return functionName == "MYVOLATILEFUNC";
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYVOLATILEFUNC")
            {
                calculationCount++;
                data.CalculatedValue = calculationCount;
            }
        }
    }
}
```

### Ver también

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


