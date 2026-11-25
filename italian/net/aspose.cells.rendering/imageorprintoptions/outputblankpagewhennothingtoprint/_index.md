---
title: "ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Indica se emettere una pagina vuota quando non c'è nulla da stampare"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Indica se generare una pagina vuota quando non c'è nulla da stampare.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook vuoto
            Workbook workbook = new Workbook();
            
            // Accedi al primo worksheet che è vuoto
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le opzioni di immagine o di stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Dimostra la proprietà OutputBlankPageWhenNothingToPrint
            options.OutputBlankPageWhenNothingToPrint = true;
            
            // Renderizza il foglio
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // L'output produrrà comunque una pagina vuota a causa dell'impostazione della proprietà
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
            
            // Salva la prima pagina nello stream di memoria
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            Console.WriteLine("Image data length: " + stream.ToArray().Length);
            
            // Ora imposta la proprietà su false
            options.OutputBlankPageWhenNothingToPrint = false;
            SheetRender renderer2 = new SheetRender(worksheet, options);
            
            // L'output avrà ora zero pagine
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


