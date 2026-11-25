---
title: "Classe ErrorCheckOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ErrorCheckOption. Impostazione di verifica errori applicata a determinati intervalli."
type: docs
url: /it/net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

Impostazione di controllo errori applicata a determinati intervalli.

```csharp
public class ErrorCheckOption
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Aggiunge un intervallo influenzato da questa impostazione. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Ottiene il conteggio degli intervalli influenzati da questa impostazione. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Ottiene l'intervallo influenzato da questa impostazione per l'indice fornito. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Verifica se il tipo di errore fornito sarà controllato. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Rimuove un intervallo per l'indice fornito. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Imposta se il tipo di errore fornito sarà controllato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionDemo
    {
        public static void ErrorCheckOptionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la ErrorCheckOptionCollection dal foglio di lavoro
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Aggiungi una nuova ErrorCheckOption alla collezione
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Imposta le opzioni di controllo errori
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Definisci un'area di celle e aggiungila alla ErrorCheckOption
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Salva la cartella di lavoro
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


