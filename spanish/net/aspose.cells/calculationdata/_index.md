---
title: "Clase CalculationData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CalculationData. Representa los datos requeridos al calcular una función, como el nombre de la función, parámetros ...etc"
type: docs
url: /es/net/aspose.cells/calculationdata/
---
## CalculationData class

Representa los datos requeridos al calcular una función, como el nombre de la función, los parámetros, ...etc.

```csharp
public class CalculationData
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Obtiene o establece el valor calculado para esta función. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Obtiene el objeto Cell donde está la función. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Obtiene el índice de columna de la celda donde está la función. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Obtiene el índice de fila de la celda donde está la función. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Obtiene el nombre de la función a calcular. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Obtiene la cantidad de parámetros |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Obtiene el objeto Workbook donde está la función. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Obtiene el objeto Worksheet donde está la función. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Obtiene el texto literal del parámetro en el índice dado. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Obtiene el objeto de valor representado del parámetro en un índice dado. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Obtiene el(los) valor(es) del parámetro en un índice dado. Si el parámetro es algún tipo de expresión que necesita ser calculada, entonces se calculará en modo de matriz. |

### Observaciones

Todos los objetos proporcionados por esta clase son solo para fines de "lectura". El usuario no debe cambiar ningún dato en el Workbook durante el proceso de cálculo de la fórmula, de lo contrario se pueden causar resultados inesperados o una Exception.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // Prepare un libro de trabajo y una hoja de cálculo simples
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // Coloque algunos valores que se usarán como parámetros en una función personalizada
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // Establezca una fórmula que invoque la función personalizada
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // Configure las opciones de cálculo para usar un motor personalizado
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // Ejecute el cálculo – el motor personalizado recibirá una instancia de CalculationData
                workbook.CalculateFormula(options);

                // Mostrar el resultado de la función personalizada
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // Guarde el libro de trabajo para completitud
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // Motor de cálculo personalizado que demuestra el acceso a los miembros de CalculationData
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Asegúrese de que estamos manejando la función personalizada esperada
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // Recupere los valores de los parámetros (se devuelven como objetos)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // Convierta los parámetros a double para el cálculo
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // Asigne el resultado calculado
                    data.CalculatedValue = result;

                    // Demostrar la lectura de propiedades de solo lectura
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


