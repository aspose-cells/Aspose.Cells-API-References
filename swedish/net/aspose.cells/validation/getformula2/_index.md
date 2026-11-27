---
title: "Validation.GetFormula2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Hämtar värdet eller uttrycket som är associerat med denna validering"
type: docs
url: /sv/net/aspose.cells/validation/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Hämtar värdet eller uttrycket som är associerat med denna validering.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Returvärde

Värdet eller uttrycket som är associerat med denna validering.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula2WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en validering för ett cellområde
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Lägg till valideringsområde
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Anropa GetFormula2 med parametrarna (isR1C1: false, isLocal: false)
                string formula2 = validation.GetFormula2(false, false);
                
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // Visa valideringsinställningarna
                Console.WriteLine("Validation Type: " + validation.Type);
                Console.WriteLine("Validation Operator: " + validation.Operator);
                Console.WriteLine("Validation Formula1: " + validation.Formula1);
                Console.WriteLine("Validation Formula2: " + validation.Formula2);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("ValidationMethodGetFormula2Demo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Hämtar värdet eller uttrycket som är associerat med denna validering för en specifik cell.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Returvärde

Värdet eller uttrycket som är associerat med denna validering.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula2WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa datavalidering i cell A1
            worksheet.Validations.Add();
            Validation validation = worksheet.Validations[worksheet.Validations.Count - 1];
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.Formula2 = "=B1"; // A1-style formula
            validation.AddArea(CellArea.CreateCellArea(0, 0, 0, 0)); // Apply to cell A1 (row 0, column 0)

            try
            {
                // Hämta Formula2 i R1C1-format för cell A1
                string formulaR1C1 = validation.GetFormula2(true, false, 0, 0);
                Console.WriteLine($"Formula2 (R1C1 format): {formulaR1C1}");

                // Visa att den ursprungliga formeln förblir oförändrad
                Console.WriteLine($"Original Formula2 (A1 format): {validation.Formula2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2: {ex.Message}");
            }

            workbook.Save("ValidationGetFormula2Demo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


