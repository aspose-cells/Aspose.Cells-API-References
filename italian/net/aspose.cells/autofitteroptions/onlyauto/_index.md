---
title: "AutoFitterOptions.OnlyAuto"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Indica se adattare solo le righe la cui altezza non è personalizzata"
type: docs
url: /it/net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Indica se adattare solo le righe la cui altezza non è personalizzata.

```csharp
public bool OnlyAuto { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyOnlyAutoDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento e imposta la proprietà OnlyAuto
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;

            // Carica la cartella di lavoro con le opzioni di adattamento automatico
            Workbook workbook = new Workbook("example.xml", loadOptions);
            
            // Dimostra l'adattamento automatico controllando la larghezza della colonna
            Console.WriteLine("Column width after auto-fit: " + 
                workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
            
            // Salva e ricarica per verificare la persistenza
            workbook.Save("example_output.xlsx");
            Workbook reloaded = new Workbook("example_output.xlsx");
            Console.WriteLine("Reloaded column width: " + 
                reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


