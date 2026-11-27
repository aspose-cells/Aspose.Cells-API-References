---
title: "Validation.GetFormula1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Hämtar värdet eller uttrycket som är associerat med denna validering"
type: docs
url: /sv/net/aspose.cells/validation/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Hämtar värdet eller uttrycket som är associerat med denna validering.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
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

    public class ValidationMethodGetFormula1WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en validering i den första cellen
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Applicera validering på cell A1
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Anropa GetFormula1 med parametrarna (false, false) för att få formeln i A1-notation
                string formula1 = validation.GetFormula1(false, false);
                
                Console.WriteLine("Formula1 in A1 notation: " + formula1);
                
                // Anropa GetFormula1 med parametrarna (true, false) för att få formeln i R1C1-notation
                string formula1R1C1 = validation.GetFormula1(true, false);
                
                Console.WriteLine("Formula1 in R1C1 notation: " + formula1R1C1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("ValidationMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Hämtar värdet eller uttrycket som är associerat med denna validering för en specifik cell.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
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

    public class ValidationMethodGetFormula1WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa validering i cell B5 (rad 4, kolumn 1)
            CellArea area = CellArea.CreateCellArea(4, 1, 4, 1); // Use static method via type name
            int validationIndex = worksheet.Validations.Add(area); // Get validation index
            Validation validation = worksheet.Validations[validationIndex]; // Retrieve validation object
            validation.Type = ValidationType.Custom;
            validation.Formula1 = "=A5"; // Relative reference to cell A5

            try
            {
                // Anropa GetFormula1 med R1C1-format för cell B5
                string formulaR1C1 = validation.GetFormula1(true, false, 4, 1);
                Console.WriteLine($"R1C1 Formula: {formulaR1C1}");

                // Anropa GetFormula1 med A1-format för cell B5
                string formulaA1 = validation.GetFormula1(false, false, 4, 1);
                Console.WriteLine($"A1 Formula: {formulaA1}");

                workbook.Save("ValidationGetFormula1Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


