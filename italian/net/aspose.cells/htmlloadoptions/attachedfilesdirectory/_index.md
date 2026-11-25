---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. La directory in cui verranno salvati i file allegati"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

La directory in cui verranno salvati i file allegati.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà HtmlLoadOptions.StreamProvider. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2014. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Crea un'istanza di HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Imposta la directory per i file allegati
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // Carica un file HTML in una cartella di lavoro utilizzando le opzioni specificate
            Workbook workbook = new Workbook("input.html", options);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


