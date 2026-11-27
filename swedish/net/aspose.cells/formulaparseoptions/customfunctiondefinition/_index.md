---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaParseOptions-egenskap. Definition för att tolka anpassade funktioner"
type: docs
url: /sv/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

Definition för att analysera anpassade funktioner.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### Anmärkningar

För vissa speciella krav, såsom när en anpassad funktion beräknas i användarens egna motor, måste vissa parametrar beräknas i arrayläge; med den här egenskapen kan dessa parametrar markeras som arrayläge vid parsning av formeln. Annars måste användaren uppdatera dessa anpassade funktioner senare via [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) för att få samma resultat.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa definition för anpassad funktion
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // Ställ in formelparsningalternativ med anpassad funktion
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // Ange exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // Använd anpassad funktion i formeln
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // Beräkna arbetsbok för att demonstrera bearbetning av anpassad funktion
            workbook.CalculateFormula();

            // Spara resultatet
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


