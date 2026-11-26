---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomFunctionDefinition. Obtiene los índices de los parámetros de la función personalizada que deben calcularse en modo de matriz"
type: docs
url: /es/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

Obtiene los índices de los parámetros de la función personalizada dada que deben calcularse en modo de matriz.

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionName | String | Nombre de la función personalizada. |

### Valor de retorno

Índices de los parámetros que deben calcularse en modo de matriz para la función personalizada dada. El valor predeterminado es nulo, no hay ningún parámetro que necesite calcularse en modo de matriz para la función personalizada.

### Observaciones

Para una expresión que necesita ser calculada, tomando A:A+B:B como ejemplo: Generalmente en modo valor se calculará a un solo valor según la base de la celda actual. Pero en modo matriz, todos los valores de A1+B1, A2+B2, A3+B3, ... se calcularán y se usarán para el cálculo.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de CustomFunctionDefinition
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // Llamar a GetArrayModeParameters con un parámetro de nombre de función
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // Mostrar el resultado
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


