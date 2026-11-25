---
title: "Classe Validation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Validation. Rappresenta le impostazioni di convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/
---
## Validation class

Rappresenta le impostazioni di convalida dei dati.

```csharp
public class Validation
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle/) { get; set; } | Rappresenta lo stile di avviso di convalida. |
| [Areas](../../aspose.cells/validation/areas/) { get; } | Ottiene tutti i [`CellArea`](../cellarea/) che contengono le impostazioni di convalida dei dati. |
| [ErrorMessage](../../aspose.cells/validation/errormessage/) { get; set; } | Rappresenta il messaggio di errore di convalida dei dati. |
| [ErrorTitle](../../aspose.cells/validation/errortitle/) { get; set; } | Rappresenta il titolo della finestra di dialogo di errore di convalida dei dati. |
| [Formula1](../../aspose.cells/validation/formula1/) { get; set; } | Rappresenta il valore o l'espressione associati alla convalida dei dati. |
| [Formula2](../../aspose.cells/validation/formula2/) { get; set; } | Rappresenta il valore o l'espressione associati alla convalida dei dati. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank/) { get; set; } | Indica se i valori vuoti sono consentiti dalla convalida dei dati dell'intervallo. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown/) { get; set; } | Indica se la convalida dei dati visualizza un elenco a discesa che contiene valori accettabili. |
| [InputMessage](../../aspose.cells/validation/inputmessage/) { get; set; } | Rappresenta il messaggio di input della convalida dei dati. |
| [InputTitle](../../aspose.cells/validation/inputtitle/) { get; set; } | Rappresenta il titolo della finestra di dialogo di input della convalida dei dati. |
| [Operator](../../aspose.cells/validation/operator/) { get; set; } | Rappresenta l'operatore per la convalida dei dati. |
| [ShowError](../../aspose.cells/validation/showerror/) { get; set; } | Indica se il messaggio di errore di convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi. |
| [ShowInput](../../aspose.cells/validation/showinput/) { get; set; } | Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida dei dati. |
| [Type](../../aspose.cells/validation/type/) { get; set; } | Rappresenta il tipo di convalida dei dati. |
| [Value1](../../aspose.cells/validation/value1/) { get; set; } | Rappresenta il primo valore associato alla convalida dei dati. |
| [Value2](../../aspose.cells/validation/value2/) { get; set; } | Rappresenta il secondo valore associato alla convalida dei dati. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea/#addarea)(CellArea) | Applica la convalida all'area. |
| [AddArea](../../aspose.cells/validation/addarea/#addarea_1)(CellArea, bool, bool) | Applica la convalida all'area. |
| [AddAreas](../../aspose.cells/validation/addareas/)(CellArea[], bool, bool) | Applica la convalida alle aree specificate. |
| [Copy](../../aspose.cells/validation/copy/)(Validation, CopyOptions) | Copia la convalida. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1)(bool, bool) | Ottiene il valore o l'espressione associati a questa convalida. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1_1)(bool, bool, int, int) | Ottiene il valore o l'espressione associati a questa convalida per una cella specifica. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2)(bool, bool) | Ottiene il valore o l'espressione associati a questa convalida. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2_1)(bool, bool, int, int) | Ottiene il valore o l'espressione associati a questa convalida per una cella specifica. |
| [GetListValue](../../aspose.cells/validation/getlistvalue/)(int, int) | Ottieni il valore per l'elenco della convalida per la cella specificata. |
| [GetValue](../../aspose.cells/validation/getvalue/)(int, int, bool) | Ottieni il valore della convalida sulla cella specifica. |
| [RemoveACell](../../aspose.cells/validation/removeacell/)(int, int) | Rimuovi le impostazioni di convalida nella cella. |
| [RemoveArea](../../aspose.cells/validation/removearea/)(CellArea) | Rimuovi le impostazioni di convalida nell'intervallo. |
| [RemoveAreas](../../aspose.cells/validation/removeareas/)(CellArea[]) | Rimuove questa convalida dalle aree specificate. |
| [SetFormula1](../../aspose.cells/validation/setformula1/)(string, bool, bool) | Imposta il valore o l'espressione associati a questa convalida. |
| [SetFormula2](../../aspose.cells/validation/setformula2/)(string, bool, bool) | Imposta il valore o l'espressione associati a questa convalida. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationDemo
    {
        public static void ValidationExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definisci un'area di celle per la convalida
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Accedi alla raccolta delle convalide
            ValidationCollection validations = worksheet.Validations;

            // Aggiungi una nuova convalida alla raccolta
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Imposta le proprietà di convalida
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;

            // Salva la cartella di lavoro
            workbook.Save("ValidationExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


