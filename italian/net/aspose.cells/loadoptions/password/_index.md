---
title: "LoadOptions.Password"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene e imposta la password della cartella di lavoro"
type: docs
url: /it/net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Ottiene e imposta la password del workbook.

```csharp
public string Password { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento e imposta la password
            LoadOptions options = new LoadOptions();
            options.Password = "test";

            // Carica cartella di lavoro protetta da password
            Workbook workbook = new Workbook("protected.xlsx", options);

            // Rimuovi la protezione con password dopo il caricamento
            workbook.Settings.Password = null;

            // Salva il workbook non protetto
            workbook.Save("unprotected.xlsx");
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


