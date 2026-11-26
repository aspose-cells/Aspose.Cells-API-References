---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CalculationData. Obtiene los valores del parámetro en un índice dado. Si el parámetro es algún tipo de expresión que necesita ser calculada, entonces se calculará en modo matriz"
type: docs
url: /es/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Obtiene el(los) valor(es) del parámetro en un índice dado. Si el parámetro es algún tipo de expresión que necesita ser calculada, entonces se calculará en modo de matriz.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice del parámetro (basado en 0) |
| maxRowCount | Int32 | El límite de recuento de filas para la matriz devuelta. Si es no positivo o mayor que el recuento real de filas, se usará el recuento real de filas. |
| maxColumnCount | Int32 | El límite de recuento de columnas para la matriz devuelta. Si es no positivo o mayor que el recuento real de filas, se usará el recuento real de columnas. |

### Valor de retorno

Una matriz que contiene todos los elementos representados por el parámetro especificado.

### Observaciones

Para una expresión que necesita ser calculada, tomando A:A+B:B como ejemplo: En modo valor se calculará a un solo valor según la base de la celda actual. Pero en modo matriz, todos los valores de A1+B1, A2+B2, A3+B3, ... se calcularán y se usarán para construir la matriz devuelta. Y para este tipo de situación, es mejor especificar el límite para el recuento de filas/columnas (como según [`MaxDataRow`](../../cells/maxdatarow/) y [`MaxDataColumn`](../../cells/maxdatacolumn/)), de lo contrario la gran matriz devuelta puede aumentar el consumo de memoria con una gran cantidad de datos inútiles.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para el contexto
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // Crear opciones de cálculo con motor personalizado
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // Llame a GetParamValueInArrayMode con parámetros realistas
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
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


