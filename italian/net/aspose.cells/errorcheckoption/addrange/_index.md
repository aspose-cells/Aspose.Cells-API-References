---
title: "ErrorCheckOption.AddRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ErrorCheckOption. Aggiunge un intervallo influenzato da questa impostazione"
type: docs
url: /it/net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Aggiunge un intervallo influenzato da questa impostazione.

```csharp
public int AddRange(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | l'intervallo da aggiungere. |

### Valore di ritorno

l'indice dell'intervallo aggiunto nell'elenco degli intervalli di questa impostazione.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
            int index = optsCollection.Add();
            ErrorCheckOption opts = optsCollection[index];
            
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            
            // Aggiungi intervalli usando CellArea
            opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
            opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
            
            // Salva la cartella di lavoro
            workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
            
            Console.WriteLine("Workbook saved with error check options.");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


