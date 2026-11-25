---
title: "Validation.SetFormula1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di convalida. Imposta il valore o l'espressione associata a questa convalida"
type: docs
url: /it/net/aspose.cells/validation/setformula1/
---
## Validation.SetFormula1 method

Imposta il valore o l'espressione associati a questa convalida.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | Il valore o l'espressione associata a questa condizione di formattazione. |
| isR1C1 | Booleano | Indica se la formula è una formula R1C1. |
| isLocal | Booleano | Se la formula è formattata secondo la locale. |

### Esempi

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

            // Prepara dati di esempio nella cella B1
            worksheet.Cells["B1"].PutValue(100);

            // Crea la convalida dei dati per la cella A1
            int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.Decimal;
            validation.Operator = OperatorType.GreaterOrEqual;
            validation.ShowError = true;
            validation.ErrorTitle = "Validation Error";
            validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";

            try
            {
                // Imposta la formula che fa riferimento a B1 usando la notazione A1 (non R1C1, non locale)
                validation.SetFormula1("=B1", false, false);
                Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
            }

            // Salva la cartella di lavoro con la convalida
            workbook.Save("ValidationSetFormula1Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


