---
title: "Clase PowerQueryFormulaItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.QueryTables.PowerQueryFormulaItem. Representa el elemento de la fórmula de Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Representa el elemento de la fórmula Power Query.

```csharp
public class PowerQueryFormulaItem
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ItemType](../../aspose.cells.querytables/powerqueryformulaitem/itemtype/) { get; } | Obtiene el tipo de este elemento (Function, Parameter, List, Literal o Unknown). |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Obtiene el nombre del elemento. |
| [TextValue](../../aspose.cells.querytables/powerqueryformulaitem/textvalue/) { get; } | Obtiene el valor de texto del elemento. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Obtiene el valor del elemento. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;

    public class QueryTablesClassPowerQueryFormulaItemDemo
    {
        public static void Run()
        {
            try
            {
                // Cree un nuevo libro de trabajo (puede ser un archivo existente si tiene datos de Power Query)
                Workbook workbook = new Workbook();

                // Acceda al objeto DataMashup que contiene fórmulas PowerQuery
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // Itere a través de todas las fórmulas PowerQuery y sus elementos
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // Demostrar la propiedad Name de solo lectura
                        Console.WriteLine($"Item Name: {item.Name}");

                        // Demostrar la propiedad Value de lectura/escritura
                        Console.WriteLine($"Original Value: {item.Value}");
                        item.Value = "SampleValue";
                        Console.WriteLine($"Modified Value: {item.Value}");

                        itemFound = true;
                    }
                }

                if (!itemFound)
                {
                    Console.WriteLine("No PowerQueryFormulaItem instances were found in the workbook.");
                }

                Console.WriteLine("PowerQueryFormulaItem demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaItem: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


