---
title: "Clase CalculationOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CalculationOptions. Representa opciones para el cálculo"
type: docs
url: /es/net/aspose.cells/calculationoptions/
---
## CalculationOptions class

Representa opciones para el cálculo.

```csharp
public class CalculationOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | El tamaño de la pila para calcular celdas de forma recursiva. El valor predeterminado es 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | El monitor para que el usuario siga el progreso del cálculo de fórmulas. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Especifica la codificación utilizada para codificar/decodificar caracteres al calcular fórmulas. Para funciones como CHAR, CODE, el resultado calculado depende de la configuración regional y del juego de caracteres predeterminado del entorno. Con esta propiedad el usuario puede especificar la codificación adecuada para esas funciones y obtener el resultado esperado. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Indica si los errores encontrados al calcular fórmulas deben ser ignorados. El error puede ser una función no compatible, enlaces externos, etc. El valor predeterminado es true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Especifica las fuentes de datos para los enlaces externos utilizados en fórmulas. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Especifica la estrategia para procesar la precisión del cálculo. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Indica si se deben calcular recursivamente las celdas dependientes al calcular una celda que depende de otras celdas. El valor predeterminado es true. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | Indica si las fórmulas de matrices dinámicas deben actualizarse antes de calcular fórmulas. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | Indica si el usuario ha especificado explícitamente el comportamiento de actualizar las fórmulas de matrices dinámicas antes de calcular fórmulas especificadas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class CalculationOptionsDemo
    {
        public static void CalculationOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Crea una instancia de CalculationOptions
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // Opcionalmente, puedes establecer un motor de cálculo personalizado o un monitor
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // Calcula fórmulas en el libro de trabajo con las opciones especificadas
            workbook.CalculateFormula(calcOptions);

            // Guarda el libro de trabajo
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
    }

    // Ejemplo de motor de cálculo personalizado (si es necesario)
    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Lógica de cálculo personalizada
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // Ejemplo de lógica de función personalizada
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // Procesa el parámetro aquí
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
    }

    // Ejemplo de monitor de cálculo personalizado (si es necesario)
    public class MyCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Lógica antes del cálculo
            Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Lógica después del cálculo
            Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
        {
            // Manejar referencias circulares
            Console.WriteLine("Circular reference detected.");
            return true; // Continue calculation
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


