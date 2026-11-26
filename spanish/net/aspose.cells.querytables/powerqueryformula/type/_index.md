---
title: "PowerQueryFormula.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormula. Obtiene el tipo de esta fórmula Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

Obtiene el tipo de esta fórmula de Power Query.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener fórmulas existentes (ninguna en el nuevo libro) para demostrar la propiedad Type
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // En un escenario real con fórmulas existentes, verificaríamos sus tipos
            Console.WriteLine("Power Query Formula Types:");
            
            // Esto demuestra la verificación de la propiedad Type
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // Con fines de demostración, agregar salida cuando no existan fórmulas
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // Guarda el libro de trabajo
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### Ver también

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


