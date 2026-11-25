---
title: "Validation.GetFormula1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di convalida. Ottiene il valore o l'espressione associata a questa convalida"
type: docs
url: /it/net/aspose.cells/validation/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Ottiene il valore o l'espressione associati a questa convalida.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Valore di ritorno

Il valore o l'espressione associata a questa convalida.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula1WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una convalida alla prima cella
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Applica la convalida alla cella A1
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Chiama GetFormula1 con i parametri (false, false) per ottenere la formula nella notazione A1
                string formula1 = validation.GetFormula1(false, false);
                
                Console.WriteLine("Formula1 in A1 notation: " + formula1);
                
                // Chiama GetFormula1 con i parametri (true, false) per ottenere la formula nella notazione R1C1
                string formula1R1C1 = validation.GetFormula1(true, false);
                
                Console.WriteLine("Formula1 in R1C1 notation: " + formula1R1C1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ValidationMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Ottiene il valore o l'espressione associati a questa convalida per una cella specifica.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |

### Valore di ritorno

Il valore o l'espressione associata a questa convalida.

### Esempi

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

            // Crea una convalida nella cella B5 (riga 4, colonna 1)
            CellArea area = CellArea.CreateCellArea(4, 1, 4, 1); // Use static method via type name
            int validationIndex = worksheet.Validations.Add(area); // Get validation index
            Validation validation = worksheet.Validations[validationIndex]; // Retrieve validation object
            validation.Type = ValidationType.Custom;
            validation.Formula1 = "=A5"; // Relative reference to cell A5

            try
            {
                // Chiama GetFormula1 con il formato R1C1 per la cella B5
                string formulaR1C1 = validation.GetFormula1(true, false, 4, 1);
                Console.WriteLine($"R1C1 Formula: {formulaR1C1}");

                // Chiama GetFormula1 con il formato A1 per la cella B5
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

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


