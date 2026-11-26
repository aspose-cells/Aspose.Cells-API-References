---
title: "Clase PowerQueryFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.QueryTables.PowerQueryFormula. Representa la definición de la fórmula de Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Representa la definición de la fórmula Power Query.

```csharp
public class PowerQueryFormula
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Obtiene y establece la descripción de la fórmula de Power Query. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Obtiene la definición de la fórmula de Power Query. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Obtiene el nombre del grupo que contiene esta fórmula de Power Query. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Obtiene y establece el nombre de la fórmula de Power Query. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Obtiene todos los elementos de la fórmula de Power Query. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Obtiene el tipo de esta fórmula de Power Query. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Acceda a la colección PowerQueryFormulas desde DataMashup
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // Verifique si existen fórmulas
                if (formulas.Count > 0)
                {
                    // Obtenga la primera PowerQueryFormula
                    PowerQueryFormula formula = formulas[0];

                    // Mostrar propiedades de solo lectura
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // Mostrar y modificar propiedades de lectura-escritura
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // Mostrar el recuento de elementos de la fórmula
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // Guarda el libro de trabajo
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormula: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


