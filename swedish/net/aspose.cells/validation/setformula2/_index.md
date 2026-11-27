---
title: "Validation.SetFormula2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Anger värdet eller uttrycket som är associerat med denna validering"
type: docs
url: /sv/net/aspose.cells/validation/setformula2/
---
## Validation.SetFormula2 method

Ställer in värdet eller uttrycket som är associerat med denna validering.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class ValidationMethodSetFormula2WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempelreferensvärden
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["B1"].PutValue(200);

            // Skapa datavalidering för cell C1
            ValidationCollection validations = worksheet.Validations;
            Validation validation = validations[validations.Add()];
            validation.AddArea(CellArea.CreateCellArea(0, 0, 2, 2)); // Applies to cell C1

            // Konfigurera valideringsparametrar
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.ShowError = true;
            validation.ErrorTitle = "Range Error";
            validation.ErrorMessage = "Value must be between A1 (100) and B1 (200)";

            try
            {
                // Ange valideringsformler med nödvändiga parametertyper
                validation.SetFormula1("=A1", false, false);
                validation.SetFormula2("=B1", false, false); // Demonstrate (String, Boolean, Boolean)

                Console.WriteLine("SetFormula2 executed successfully with formula '=B1'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("ValidationSetFormula2Demo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


