---
title: "PowerQueryFormula.FormulaDefinition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormula. Obtiene la definición de la fórmula Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformula/formuladefinition/
---
## PowerQueryFormula.FormulaDefinition property

Obtiene la definición de la fórmula de Power Query.

```csharp
public virtual string FormulaDefinition { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyFormulaDefinitionDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear tabla de ejemplo que Power Query pueda referenciar
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Test");
            
            // Obtener fórmulas Power Query existentes (estarán vacías para el nuevo libro)
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Acceder a la primera fórmula si existe (demostrando el uso de FormulaDefinition)
            if (formulas.Count > 0)
            {
                PowerQueryFormula formula = formulas[0];
                Console.WriteLine("Formula Definition: " + formula.FormulaDefinition);
                Console.WriteLine("Formula Name: " + formula.Name);
                Console.WriteLine("Formula Description: " + formula.Description);
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
            
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


