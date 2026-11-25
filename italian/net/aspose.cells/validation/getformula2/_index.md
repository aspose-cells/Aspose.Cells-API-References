---
title: "Validation.GetFormula2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di convalida. Ottiene il valore o l'espressione associata a questa convalida"
type: docs
url: /it/net/aspose.cells/validation/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Ottiene il valore o l'espressione associati a questa convalida.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
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

    public class ValidationMethodGetFormula2WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una convalida a un intervallo di celle
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Aggiungi area di convalida
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Chiama GetFormula2 con i parametri (isR1C1: false, isLocal: false)
                string formula2 = validation.GetFormula2(false, false);
                
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // Visualizza le impostazioni di convalida
                Console.WriteLine("Validation Type: " + validation.Type);
                Console.WriteLine("Validation Operator: " + validation.Operator);
                Console.WriteLine("Validation Formula1: " + validation.Formula1);
                Console.WriteLine("Validation Formula2: " + validation.Formula2);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ValidationMethodGetFormula2Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Ottiene il valore o l'espressione associati a questa convalida per una cella specifica.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
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

    public class ValidationMethodGetFormula2WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea la convalida dei dati nella cella A1
            worksheet.Validations.Add();
            Validation validation = worksheet.Validations[worksheet.Validations.Count - 1];
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.Formula2 = "=B1"; // A1-style formula
            validation.AddArea(CellArea.CreateCellArea(0, 0, 0, 0)); // Apply to cell A1 (row 0, column 0)

            try
            {
                // Ottieni Formula2 in formato R1C1 per la cella A1
                string formulaR1C1 = validation.GetFormula2(true, false, 0, 0);
                Console.WriteLine($"Formula2 (R1C1 format): {formulaR1C1}");

                // Dimostra che la formula originale rimane invariata
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

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


