---
title: "ErrorCheckOption.GetCountOfRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ErrorCheckOption. Ottiene il numero di intervalli influenzati da questa impostazione"
type: docs
url: /it/net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Ottiene il conteggio degli intervalli influenzati da questa impostazione.

```csharp
public int GetCountOfRange()
```

### Valore di ritorno

il conteggio degli intervalli influenzati da questa impostazione.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodGetCountOfRangeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ottieni la collezione delle opzioni di controllo errori
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;

            // Aggiungi la prima opzione di controllo errori
            int index1 = optsCollection.Add();
            ErrorCheckOption opts1 = optsCollection[index1];
            opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
            opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));

            // Aggiungi la seconda opzione di controllo errori
            int index2 = optsCollection.Add();
            ErrorCheckOption opts2 = optsCollection[index2];
            opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));

            // Dimostra il metodo GetCountOfRange
            Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
            Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());

            // Salva la cartella di lavoro
            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


