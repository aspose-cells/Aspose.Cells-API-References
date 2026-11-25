---
title: "PageSetup.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Copia l'impostazione della configurazione della pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Copia le impostazioni della configurazione della pagina.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | PageSetup | L'origine. |
| copyOptions | CopyOptions | Le opzioni di copia. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Imposta le proprietà di PageSetup per il primo foglio di lavoro
            workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
            
            // Copia PageSetup dal primo foglio di lavoro al secondo foglio di lavoro con CopyOptions
            workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
            
            Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


