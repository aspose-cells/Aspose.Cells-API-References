---
title: "PowerQueryFormulaParameter.ParameterDefinition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaParameter. Obtiene la definición del parámetro"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/
---
## PowerQueryFormulaParameter.ParameterDefinition property

Obtiene la definición del parámetro.

```csharp
[Obsolete("Use PowerQueryFormulaParameter.FormulaDefinition property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ParameterDefinition { get; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PowerQueryFormulaParameter.FormulaDefinition. Esta propiedad será eliminada dentro de 12 meses a partir de noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyParameterDefinitionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder a la propiedad DataMashup del libro de trabajo
                DataMashup dataMashup = workbook.DataMashup;

                if (dataMashup != null)
                {
                    // Acceda a la colección PowerQueryFormulaParameters
                    PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                    // Itere a través de los parámetros para demostrar ParameterDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Muestre el valor de la propiedad ParameterDefinition (propiedad de solo lectura)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Parameter Definition: {parameter.ParameterDefinition}");
                        Console.WriteLine($"Formula Definition: {parameter.FormulaDefinition}");
                        Console.WriteLine($"Parameter Value: {parameter.Value}");
                        Console.WriteLine("----------------------------------------");
                    }

                    if (parameters.Count == 0)
                    {
                        Console.WriteLine("No PowerQueryFormulaParameter instances found in the workbook.");
                    }
                }
                else
                {
                    Console.WriteLine("No DataMashup available in the workbook.");
                }

                // Guarda el libro de trabajo
                workbook.Save("ParameterDefinitionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


