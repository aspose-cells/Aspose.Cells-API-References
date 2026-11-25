---
title: "NumbersLoadOptions.LoadTableType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "NumbersLoadOptions proprietà. Ottiene e imposta il tipo di caricamento di più tabelle in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Ottiene e imposta il tipo di caricamento di più tabelle in un foglio di lavoro.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // Crea un'istanza di NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Dimostra l'uso della proprietà LoadTableType
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // Altre proprietà minime richieste
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // Carica un file Numbers con le opzioni di caricamento specificate
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Salva la cartella di lavoro in formato XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


