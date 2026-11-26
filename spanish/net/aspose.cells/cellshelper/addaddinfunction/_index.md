---
title: "CellsHelper.AddAddInFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Agregar función addin"
type: docs
url: /es/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

Agregar función addin.

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| función | String | El nombre de la función. |
| minCountOfParameters | Int32 | Número mínimo de parámetros que requiere esta función |
| maxCountOfParameters | Int32 | Número máximo de parámetros que permite esta función. |
| paramersType | ParameterType[] | El tipo de parámetros esperado de la función |
| functionValueType | ParameterType | El tipo de valor de la función. |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use los métodos WorksheetCollection.RegisterAddInFunction(). Este método será eliminado 12 meses después desde enero de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Definir parámetros para AddAddInFunction
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // Llamar al método AddAddInFunction
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // Usar la función personalizada en una celda
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // Calcular fórmulas
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


