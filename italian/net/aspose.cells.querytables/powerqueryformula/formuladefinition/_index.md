---
title: "PowerQueryFormula.FormulaDefinition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormula. Ottiene la definizione della formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformula/formuladefinition/
---
## PowerQueryFormula.FormulaDefinition property

Ottiene la definizione della formula Power Query.

```csharp
public virtual string FormulaDefinition { get; }
```

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una tabella di esempio a cui Power Query può fare riferimento
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Test");
            
            // Recupera le formule Power Query esistenti (saranno vuote per la nuova cartella di lavoro)
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Accedi alla prima formula se esiste (dimostrando l'uso di FormulaDefinition)
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

### Vedi anche

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


