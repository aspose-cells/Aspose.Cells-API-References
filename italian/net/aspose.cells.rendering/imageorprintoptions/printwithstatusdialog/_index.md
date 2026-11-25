---
title: "ImageOrPrintOptions.PrintWithStatusDialog"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Se PrintWithStatusDialog true verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente. altrimenti non verrà mostrata alcuna finestra di dialogo"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/
---
## ImageOrPrintOptions.PrintWithStatusDialog property

Se PrintWithStatusDialog = true, verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente; altrimenti non verrà mostrata alcuna finestra di dialogo.

```csharp
public bool PrintWithStatusDialog { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
    {
        public static void Run()
        {
            // Inizializza una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Imposta le opzioni di immagine o di stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintWithStatusDialog = false; // Disable print status dialog
            options.PageIndex = 0;
            options.PageCount = 1;

            // Crea il rendering del foglio
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            // Stampa in PDF
            sheetRender.ToImage(0, "output.png");

            // Attendi la creazione del file (logica di attesa semplificata)
            int attempts = 0;
            while (!File.Exists("output.png") && attempts < 5)
            {
                Thread.Sleep(1000);
                attempts++;
            }

            if (File.Exists("output.png"))
            {
                Console.WriteLine("Image file created successfully");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


