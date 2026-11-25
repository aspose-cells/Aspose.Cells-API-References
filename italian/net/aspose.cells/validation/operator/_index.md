---
title: "Validation.Operator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Validation. Rappresenta l'operatore per la convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/operator/
---
## Validation.Operator property

Rappresenta l'operatore per la convalida dei dati.

```csharp
public OperatorType Operator { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyOperatorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la convalida
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Crea un intervallo di convalida
            CellArea area = CellArea.CreateCellArea("B1", "B5");
            int validationIndex = worksheet.Validations.Add(area);
            Validation validation = worksheet.Validations[validationIndex];

            // Imposta le proprietà di convalida con la dimostrazione di Operator
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "30";
            validation.ShowError = true;
            validation.ErrorMessage = "Value must be between 10 and 30";

            // Salva la cartella di lavoro
            workbook.Save("ValidationOperatorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


