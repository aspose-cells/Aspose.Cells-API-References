---
title: "Validation.SetFormula1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Anger värdet eller uttrycket som är associerat med denna validering"
type: docs
url: /sv/net/aspose.cells/validation/setformula1/
---
## Validation.SetFormula1 method

Ställer in värdet eller uttrycket som är associerat med denna validering.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Värdet eller uttrycket som är associerat med detta formatvillkor. |
| isR1C1 | Boolean | Om formeln är en R1C1-formel. |
| isLocal | Boolean | Om formeln är lokalt formaterad. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered exempeldata i cell B1
            worksheet.Cells["B1"].PutValue(100);

            // Skapa datavalidering för cell A1
            int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.Decimal;
            validation.Operator = OperatorType.GreaterOrEqual;
            validation.ShowError = true;
            validation.ErrorTitle = "Validation Error";
            validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";

            try
            {
                // Ange formel som refererar till B1 med A1-notation (icke-R1C1, icke-lokal)
                validation.SetFormula1("=B1", false, false);
                Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
            }

            // Spara arbetsboken med validering
            workbook.Save("ValidationSetFormula1Demo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


