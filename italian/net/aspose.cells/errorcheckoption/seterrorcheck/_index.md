---
title: "ErrorCheckOption.SetErrorCheck"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ErrorCheckOption. Imposta se il tipo di errore specificato deve essere controllato"
type: docs
url: /it/net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

Imposta se il tipo di errore fornito sarà controllato.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | il tipo di errore può essere controllato. |
| isCheck | Booleano | vero se il tipo di errore specificato deve essere controllato (verrà mostrato un triangolo verde nella cella se il controllo fallisce). |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodSetErrorCheckWithErrorCheckTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Sample text for error checking");
            
            // Configura le opzioni di controllo errori
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            
            // Dimostra SetErrorCheck con diversi valori di ErrorCheckType
            errorCheckOption.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, true);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            
            // Applica all'intero foglio di lavoro
            errorCheckOption.AddRange(CellArea.CreateCellArea(0, 0, worksheet.Cells.MaxRow, worksheet.Cells.MaxDataColumn));
            
            workbook.Save("ErrorCheckExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


