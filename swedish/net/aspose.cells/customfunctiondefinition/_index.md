---
title: "Klass CustomFunctionDefinition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CustomFunctionDefinition klass. Definition av anpassad funktion för beräkning med användarens egna motor"
type: docs
url: /sv/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

Definition av anpassad funktion för beräkning med användarens anpassade motor.

```csharp
public class CustomFunctionDefinition
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | Hämtar indexen för den angivna anpassade funktionens parametrar som måste beräknas i arrayläge. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa en ny CustomFunctionDefinition-instans
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // Skapa en ny FormulaParseOptions-instans och ange CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // Lägg till ett kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Definiera en anpassad formel
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // Analysera den anpassade formeln med hjälp av FormulaParseOptions
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // Spara arbetsboken
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


