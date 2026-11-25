---
title: "LoadOptions.SetPaperSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LoadOptions. Imposta la dimensione carta di stampa predefinita dalle impostazioni della stampante predefinita"
type: docs
url: /it/net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Imposta la dimensione della carta di stampa predefinita dalle impostazioni della stampante predefinita.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | PaperSizeType | La dimensione carta predefinita. |

### Osservazioni

Se non esiste un'impostazione relativa alla dimensione della carta, MS Excel utilizzerà l'impostazione predefinita della stampante.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento e imposta la dimensione carta su A5
            LoadOptions options = new LoadOptions();
            options.SetPaperSize(PaperSizeType.PaperA5);

            // Carica la cartella di lavoro con le opzioni specificate
            Workbook workbook = new Workbook("example.xlsx", options);
            
            // Verifica che la dimensione carta sia impostata correttamente
            Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
        }
    }
}
```

### Vedi anche

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


