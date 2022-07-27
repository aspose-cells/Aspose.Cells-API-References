---
title: Validation
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta la convalida dei dati.impostazioni.
type: docs
weight: 6200
url: /it/net/aspose.cells/validation/
---
## Validation class

Rappresenta la convalida dei dati.impostazioni.

```csharp
public class Validation
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle) { get; set; } | Rappresenta lo stile di avviso di convalida. |
| [Areas](../../aspose.cells/validation/areas) { get; } | Ottiene tutto[`CellArea`](../cellarea) che contengono le impostazioni di convalida dei dati. |
| [ErrorMessage](../../aspose.cells/validation/errormessage) { get; set; } | Rappresenta il messaggio di errore di convalida dei dati. |
| [ErrorTitle](../../aspose.cells/validation/errortitle) { get; set; } | Rappresenta il titolo della finestra di dialogo dell'errore di convalida dei dati. |
| [Formula1](../../aspose.cells/validation/formula1) { get; set; } | Rappresenta il valore o l'espressione associata alla convalida dei dati. |
| [Formula2](../../aspose.cells/validation/formula2) { get; set; } | Rappresenta il valore o l'espressione associata alla convalida dei dati. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank) { get; set; } | Indica se i valori vuoti sono consentiti dalla convalida dei dati dell'intervallo. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown) { get; set; } | Indica se la convalida dei dati visualizza un elenco a discesa che contiene valori accettabili. |
| [InputMessage](../../aspose.cells/validation/inputmessage) { get; set; } | Rappresenta il messaggio di input di convalida dei dati. |
| [InputTitle](../../aspose.cells/validation/inputtitle) { get; set; } | Rappresenta il titolo della finestra di dialogo di input di convalida dei dati. |
| [Operator](../../aspose.cells/validation/operator) { get; set; } | Rappresenta l'operatore per la convalida dei dati. |
| [ShowError](../../aspose.cells/validation/showerror) { get; set; } | Indica se il messaggio di errore di convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi. |
| [ShowInput](../../aspose.cells/validation/showinput) { get; set; } | Indica se il messaggio di input di convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida dei dati. |
| [Type](../../aspose.cells/validation/type) { get; set; } | Rappresenta il tipo di convalida dei dati. |
| [Value1](../../aspose.cells/validation/value1) { get; set; } | Rappresenta il primo valore associato alla convalida dei dati. |
| [Value2](../../aspose.cells/validation/value2) { get; set; } | Rappresenta il secondo valore associato alla convalida dei dati. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea#addarea)(CellArea) | Applica la convalida all'area. |
| [AddArea](../../aspose.cells/validation/addarea#addarea_1)(CellArea, bool, bool) | Applica la convalida all'area. |
| [AddAreas](../../aspose.cells/validation/addareas)(CellArea[], bool, bool) | Applica la convalida a determinate aree. |
| [Copy](../../aspose.cells/validation/copy)(Validation, CopyOptions) | Convalida copia. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1)(bool, bool) | Ottiene il valore o l'espressione associata a questa convalida. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1_1)(bool, bool, int, int) | Ottiene il valore o l'espressione associata a questa convalida per una cella specifica. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2)(bool, bool) | Ottiene il valore o l'espressione associata a questa convalida. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2_1)(bool, bool, int, int) | Ottiene il valore o l'espressione associata a questa convalida per una cella specifica. |
| [GetListValue](../../aspose.cells/validation/getlistvalue)(int, int) | Ottieni il valore per l'elenco della convalida per la cella specificata. |
| [RemoveACell](../../aspose.cells/validation/removeacell)(int, int) | Rimuovi le impostazioni di convalida nella cella. |
| [RemoveArea](../../aspose.cells/validation/removearea)(CellArea) | Rimuovi le impostazioni di convalida nell'intervallo. |
| [RemoveAreas](../../aspose.cells/validation/removeareas)(CellArea[]) | Rimuove questa convalida da determinate aree. |
| [SetFormula1](../../aspose.cells/validation/setformula1)(string, bool, bool) | Imposta il valore o l'espressione associata a questa convalida. |
| [SetFormula2](../../aspose.cells/validation/setformula2)(string, bool, bool) | Imposta il valore o l'espressione associata a questa convalida. |

### Esempi

```csharp
[C#]
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.Worksheets[0].Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
validation.Type = Aspose.Cells.ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim validations as ValidationCollection  = workbook.Worksheets(0).Validations
Dim area as CellArea = CellArea.CreateCellArea(0, 0, 1, 1);
Dim validation as Validation = validations(validations.Add(area))
validation.Type = ValidationType.WholeNumber
validation.Operator = OperatorType.Between
validation.Formula1 = "3"
validation.Formula2 = "1234"
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
