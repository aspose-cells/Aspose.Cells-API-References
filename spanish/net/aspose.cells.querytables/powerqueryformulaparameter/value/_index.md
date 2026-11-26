---
title: "PowerQueryFormulaParameter.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaParameter. Obtiene el valor del parámetro"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulaparameter/value/
---
## PowerQueryFormulaParameter.Value property

Obtiene el valor del parámetro.

```csharp
public string Value { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyValueDemo
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

                    // Itere a través de los parámetros para demostrar la propiedad Value
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Muestre el valor actual de la propiedad Value (operación de lectura)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Current Value: {parameter.Value}");

                        // Dado que Value es de lectura/escritura, demuestre cómo establecer un nuevo valor
                        string newValue = "UpdatedValue_" + Guid.NewGuid().ToString();
                        parameter.Value = newValue;
                        Console.WriteLine($"Updated Value: {parameter.Value}");
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
                workbook.Save("ValueDemo.xlsx");
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


