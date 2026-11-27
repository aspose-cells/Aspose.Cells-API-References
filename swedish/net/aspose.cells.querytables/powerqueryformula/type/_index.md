---
title: "PowerQueryFormula.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormula property. Hämtar typen av denna Power Query-formel"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

Hämtar typen av denna Power Query-formel.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta befintliga formler (inga i ny arbetsbok) för att demonstrera Type‑egenskapen
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // I ett verkligt scenario med befintliga formler skulle vi kontrollera deras typer
            Console.WriteLine("Power Query Formula Types:");
            
            // Detta demonstrerar kontroll av Type‑egenskapen
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // För demonstrationsändamål, lägg till output när inga formler finns
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // Spara arbetsboken
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### Se även

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


