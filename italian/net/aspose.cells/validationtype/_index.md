---
title: "Enum ValidationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.ValidationType. Rappresenta il tipo di convalida dei dati"
type: docs
url: /it/net/aspose.cells/validationtype/
---
## ValidationType enumeration

Rappresenta il tipo di convalida dei dati.

```csharp
public enum ValidationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| AnyValue | `0` | Tipo di convalida per qualsiasi valore. |
| WholeNumber | `1` | Tipo di convalida per numeri interi. |
| Decimal | `2` | Tipo di convalida per decimali. |
| List | `3` | Tipo di convalida per elenco. |
| Date | `4` | Tipo di convalida per data. |
| Time | `5` | Tipo di convalida per ora. |
| TextLength | `6` | Tipo di convalida per lunghezza del testo. |
| Custom | `7` | Tipo di convalida personalizzato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationTypeDemo
    {
        public static void ValidationTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una convalida al foglio di lavoro
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // Imposta il tipo di convalida su WholeNumber
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // Imposta proprietà aggiuntive per la convalida
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // Salva la cartella di lavoro
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


