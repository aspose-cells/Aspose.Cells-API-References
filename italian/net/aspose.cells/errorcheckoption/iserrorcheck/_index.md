---
title: "ErrorCheckOption.IsErrorCheck"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ErrorCheckOption. Verifica se il tipo di errore specificato sarà controllato"
type: docs
url: /it/net/aspose.cells/errorcheckoption/iserrorcheck/
---
## ErrorCheckOption.IsErrorCheck method

Verifica se il tipo di errore fornito sarà controllato.

```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | il tipo di errore può essere controllato |

### Valore di ritorno

restituisce vero se il tipo di errore specificato sarà controllato (verrà mostrato un triangolo verde nella cella se il controllo fallisce).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodIsErrorCheckWithErrorCheckTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            int index = options.Add();
            ErrorCheckOption option = options[index];

            // Configura le impostazioni di controllo errori
            option.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            option.SetErrorCheck(ErrorCheckType.EvaluationError, true);
            option.SetErrorCheck(ErrorCheckType.InconsistRange, false);

            // Aggiungi intervallo per applicare queste impostazioni
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 10;
            area.StartColumn = 0;
            area.EndColumn = 5;
            option.AddRange(area);

            // Verifica e visualizza le impostazioni
            Console.WriteLine("NumberStoredAsText check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.NumberStoredAsText));
            Console.WriteLine("EvaluationError check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.EvaluationError));
            Console.WriteLine("InconsistRange check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.InconsistRange));
        }
    }
}
```

### Vedi anche

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


