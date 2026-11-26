---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Actualiza la definición de funciones personalizadas"
type: docs
url: /es/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Actualiza la definición de funciones personalizadas.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| definición | CustomFunctionDefinition | Definición especial de funciones personalizadas para el requisito especial del usuario. |

### Observaciones

Este método puede usarse en algunos escenarios especiales. Por ejemplo, si el usuario necesita que algunos parámetros de ciertas funciones personalizadas se calculen en modo de matriz, entonces el usuario puede proporcionar su propia definición con la implementación de [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) para esas funciones. Después de que los datos de las fórmulas se actualicen, esos parámetros especificados se calcularán en modo de matriz automáticamente al calcular las funciones personalizadas correspondientes.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // Crear motor de cálculo personalizado
            var customEngine = new MyCustomCalculationEngine();
            
            // Establecer opciones de cálculo con motor personalizado
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // Actualice la definición de la función personalizada
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // Establezca la fórmula usando una función personalizada
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // Calcular fórmulas
            wb.CalculateFormula(options);

            // Mostrar el resultado
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // Devuelva los índices de los parámetros que deben procesarse en modo de matriz
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### Ver también

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


