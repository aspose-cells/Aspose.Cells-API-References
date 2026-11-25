---
title: "HtmlLoadOptions.ProgId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. Ottiene l'ID programma della creazione del file. Solo per file MHT"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

Ottiene l'ID del programma che crea il file. Solo per file MHT.

```csharp
public string ProgId { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyProgIdDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML con formato MHTML
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            
            // Ottieni la proprietà ProgId
            Console.WriteLine("ProgId is: " + options.ProgId);

            // Crea un'altra istanza e ottieni il suo ProgId
            HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
            Console.WriteLine("ProgId is: " + wordOptions.ProgId);
        }
    }
}
```

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


