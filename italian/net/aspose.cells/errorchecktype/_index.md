---
title: "Enum ErrorCheckType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.ErrorCheckType. Rappresenta tutti i tipi di verifica degli errori"
type: docs
url: /it/net/aspose.cells/errorchecktype/
---
## ErrorCheckType enumeration

Rappresenta tutti i tipi di controllo errori.

```csharp
public enum ErrorCheckType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| EvaluationError | `1` | Ignora gli errori quando le celle contengono formule che producono un errore. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Ignora gli errori quando le formule fanno riferimento a celle vuote. |
| NumberStoredAsText | `4` | Ignora gli errori quando i numeri sono formattati come testo o sono preceduti da un apostrofo |
| TextNumber | `4` | Ignora gli errori quando i numeri sono formattati come testo o sono preceduti da un apostrofo |
| InconsistRange | `8` | Ignora gli errori quando le formule omettono alcune celle in una regione. |
| InconsistFormula | `16` | Ignora gli errori quando una formula in una regione del tuo foglio di lavoro differisce dalle altre formule nella stessa regione. |
| TwoDigitTextYear | `32` | Ignora gli errori quando le formule contengono celle formattate come testo con anni rappresentati con 2 cifre. |
| TextDate | `32` | Ignora gli errori quando le formule contengono celle formattate come testo con anni rappresentati con 2 cifre. |
| UnlockedFormula | `64` | Ignora gli errori quando le celle sbloccate contengono formule. |
| UnproctedFormula | `64` | Ignora gli errori quando le celle sbloccate contengono formule. |
| TableDataValidation | `128` | Ignora gli errori quando il valore di una cella in una Tabella non rispetta le regole di convalida dati specificate. |
| Validation | `128` | Ignora gli errori quando il valore di una cella in una Tabella non rispetta le regole di convalida dati specificate. |
| CalculatedColumn | `129` | Ignora gli errori quando le celle contengono un valore diverso da una formula di colonna calcolata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckTypeDemo
    {
        public static void ErrorCheckTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a ErrorCheckOptionCollection
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Aggiungi una nuova ErrorCheckOption
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // Imposta vari tipi di controllo errori su false
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // Definisci un'area di celle per l'opzione di controllo errori
            CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
            errorCheckOption.AddRange(cellArea);

            // Salva la cartella di lavoro
            workbook.Save("ErrorCheckTypeExample.xlsx");
            workbook.Save("ErrorCheckTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


