---
title: "SaveOptions.WarningCallback"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta il callback di avviso"
type: docs
url: /it/net/aspose.cells/saveoptions/warningcallback/
---
## SaveOptions.WarningCallback property

Ottiene o imposta il callback di avviso.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data");

            // Crea opzioni di salvataggio
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta callback di avviso personalizzato
            saveOptions.WarningCallback = new CustomWarningCallback();

            // Questo genererà un avviso riguardo a una funzionalità non supportata nel formato HTML
            worksheet.PageSetup.PrintTitleRows = "$1:$1";

            // Salva con opzioni che potrebbero generare avvisi
            workbook.Save("WarningCallbackDemo.html", saveOptions);
        }
    }

    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Gestisci l'avviso - in questo caso mostrala semplicemente
            Console.WriteLine($"Warning: {warningInfo.Description}");
            Console.WriteLine($"Warning type: {warningInfo.WarningType}");
        }
    }
}
```

### Vedi anche

* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


