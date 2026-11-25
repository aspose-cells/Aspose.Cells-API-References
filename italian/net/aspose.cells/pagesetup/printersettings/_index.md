---
title: "PageSetup.PrinterSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup proprietà. Ottiene e imposta le impostazioni della stampante predefinita"
type: docs
url: /it/net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

Ottiene e imposta le impostazioni della stampante predefinita.

```csharp
public byte[] PrinterSettings { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrinterSettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Test Printer Settings");
            
            // Accedi alla configurazione della pagina
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta le impostazioni della stampante (come array di byte)
            byte[] printerSettings = new byte[10]; // Simplified example
            pageSetup.PrinterSettings = printerSettings;
            
            // Verifica che le impostazioni della stampante siano impostate
            Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
            
            // Salva la cartella di lavoro
            workbook.Save("PrinterSettingsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


