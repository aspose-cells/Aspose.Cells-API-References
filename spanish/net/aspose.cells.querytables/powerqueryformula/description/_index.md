---
title: "PowerQueryFormula.Description"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormula. Obtiene y establece la descripción de la fórmula Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

Obtiene y establece la descripción de la fórmula de Power Query.

```csharp
public string Description { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaPropertyDescriptionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Cargar un archivo existente con fórmulas Power Query
                workbook = new Workbook("example.xlsx");

                // Acceder a fórmulas Power Query existentes
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // Mostrar el valor actual de Description
                    Console.WriteLine("Current Description: " + formula.Description);

                    // Establecer una nueva descripción
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // Guarda el libro de trabajo
                    workbook.Save("PowerQueryFormulaDescriptionDemo.xlsx");
                    Console.WriteLine("Description property demonstrated successfully.");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### Ver también

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


