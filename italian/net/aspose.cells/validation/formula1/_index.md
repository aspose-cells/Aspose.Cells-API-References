---
title: "Validation.Formula1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di convalida. Rappresenta il valore o l'espressione associata alla convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/formula1/
---
## Validation.Formula1 property

Rappresenta il valore o l'espressione associati alla convalida dei dati.

```csharp
public string Formula1 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula1Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi la convalida dell'elenco con Formula1 come valori separati da virgola
            Validation validation1 = worksheet.Validations[worksheet.Validations.Add()];
            validation1.Type = ValidationType.List;
            validation1.AlertStyle = ValidationAlertType.Stop;
            validation1.Formula1 = "A,B,C";
            validation1.AddArea(new CellArea() { StartRow = 0, StartColumn = 0, EndRow = 5, EndColumn = 0 });

            // Aggiungi la convalida della formula con Formula1 come riferimento di cella
            Validation validation2 = worksheet.Validations[worksheet.Validations.Add()];
            validation2.Type = ValidationType.Custom;
            validation2.AlertStyle = ValidationAlertType.Stop;
            validation2.Formula1 = "=A5";
            validation2.AddArea(new CellArea() { StartRow = 0, StartColumn = 1, EndRow = 5, EndColumn = 1 });

            // Salva e ricarica per verificare la persistenza
            string outputPath = "output_validation_formula1.xlsx";
            workbook.Save(outputPath);

            // Ricarica per verificare
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            Console.WriteLine("Validation 1 Formula1: " + loadedSheet.Validations[0].Formula1);
            Console.WriteLine("Validation 2 Formula1: " + loadedSheet.Validations[1].Formula1);
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


