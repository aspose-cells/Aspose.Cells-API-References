---
title: "PowerQueryFormulaFunction.F"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaFunction. Obtiene y establece la definición de la función"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

Obtiene y establece la definición de la función.

```csharp
public string F { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaFunctionPropertyFDemo
    {
        public static void Run()
        {
            // Cargar un libro de trabajo que contiene fórmulas de Power Query existentes
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la colección de fórmulas de Power Query
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Recuperar una fórmula de función existente por nombre
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // Convertir a PowerQueryFormulaFunction para acceder a la propiedad F
            if (formula is PowerQueryFormulaFunction function)
            {
                // Demostrar la obtención de la propiedad F
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // Demostrar la asignación de la propiedad F
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


