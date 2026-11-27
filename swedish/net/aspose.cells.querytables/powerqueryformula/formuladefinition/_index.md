---
title: "PowerQueryFormula.FormulaDefinition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormula egenskap. Hämtar definitionen av Power Query-formeln"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformula/formuladefinition/
---
## PowerQueryFormula.FormulaDefinition property

Hämtar definitionen av Power Query-formeln.

```csharp
public virtual string FormulaDefinition { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeltabell som Power Query kan referera till
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Test");
            
            // Hämta befintliga Power Query-formler (kommer att vara tomt för ny arbetsbok)
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Åtkomst till första formeln om den finns (demonstrerar användning av FormulaDefinition)
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

### Se även

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


