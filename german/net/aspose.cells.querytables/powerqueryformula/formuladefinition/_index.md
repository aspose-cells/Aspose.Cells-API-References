---
title: "PowerQueryFormula.FormulaDefinition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormula-Eigenschaft. Gibt die Definition der Power Query-Formel zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformula/formuladefinition/
---
## PowerQueryFormula.FormulaDefinition property

Liest die Definition der Power-Query-Formel.

```csharp
public virtual string FormulaDefinition { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle eine Beispielstabelle, auf die Power Query verweisen kann
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Test");
            
            // Vorhandene Power Query-Formeln abrufen (ist leer für neue Arbeitsmappe)
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Zugriff auf die erste Formel, falls vorhanden (demonstriert die Verwendung von FormulaDefinition)
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

### Siehe auch

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


