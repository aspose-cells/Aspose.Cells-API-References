---
title: "Enum ValidationAlertType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.ValidationAlertType. Rappresenta lo stile di avviso di convalida dei dati"
type: docs
url: /it/net/aspose.cells/validationalerttype/
---
## ValidationAlertType enumeration

Rappresenta lo stile di avviso della convalida dei dati.

```csharp
public enum ValidationAlertType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Information | `0` | Stile di avviso informativo. |
| Stop | `1` | Stile di avviso di arresto. |
| Warning | `2` | Stile di avviso di avvertimento. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationAlertTypeDemo
    {
        public static void ValidationAlertTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definisci un'area di celle per la convalida
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Aggiungi una convalida al foglio di lavoro
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Imposta le proprietà di convalida
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // Salva la cartella di lavoro
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


