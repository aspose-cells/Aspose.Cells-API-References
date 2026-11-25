---
title: "Validation.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Validation. Rappresenta il tipo di convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/type/
---
## Validation.Type property

Rappresenta il tipo di convalida dei dati.

```csharp
public ValidationType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una convalida alla cella A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.ErrorTitle = "Number Validation";
            validation.ErrorMessage = "Please enter a whole number";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });

            // Dimostra la proprietà Type
            Console.WriteLine("Validation Type: " + validation.Type);
            
            // Salva la cartella di lavoro
            workbook.Save("ValidationExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


