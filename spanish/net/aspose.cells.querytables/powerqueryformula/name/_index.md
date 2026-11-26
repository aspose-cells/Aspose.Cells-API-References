---
title: "PowerQueryFormula.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormula. Obtiene y establece el nombre de la fórmula Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Obtiene y establece el nombre de la fórmula de Power Query.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Cargar un archivo existente con fórmulas Power Query
            workbook = new Workbook("example.xlsx");
            
            // Acceder a fórmulas Power Query existentes
            if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
            {
                PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
                
                // Demostrar el uso de la propiedad Name
                Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
                
                // Cambiar el nombre
                formula.Name = "UpdatedSalesFilter";
                Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
                
                // Guarda el libro de trabajo
                workbook.Save("PowerQueryFormulaDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### Ver también

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


