---
title: "Validation.SetFormula2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di convalida. Imposta il valore o l'espressione associata a questa convalida"
type: docs
url: /it/net/aspose.cells/validation/setformula2/
---
## Validation.SetFormula2 method

Imposta il valore o l'espressione associati a questa convalida.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class ValidationMethodSetFormula2WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola i valori di riferimento di esempio
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["B1"].PutValue(200);

            // Crea la convalida dei dati per la cella C1
            ValidationCollection validations = worksheet.Validations;
            Validation validation = validations[validations.Add()];
            validation.AddArea(CellArea.CreateCellArea(0, 0, 2, 2)); // Applies to cell C1

            // Configura i parametri di convalida
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.ShowError = true;
            validation.ErrorTitle = "Range Error";
            validation.ErrorMessage = "Value must be between A1 (100) and B1 (200)";

            try
            {
                // Imposta le formule di convalida utilizzando i tipi di parametro richiesti
                validation.SetFormula1("=A1", false, false);
                validation.SetFormula2("=B1", false, false); // Demonstrate (String, Boolean, Boolean)

                Console.WriteLine("SetFormula2 executed successfully with formula '=B1'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("ValidationSetFormula2Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


