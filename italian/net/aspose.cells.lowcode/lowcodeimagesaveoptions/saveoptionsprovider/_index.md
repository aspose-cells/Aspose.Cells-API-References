---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeImageSaveOptions. Provider delle opzioni di salvataggio per il salvataggio delle immagini generate"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

Provider di opzioni di salvataggio per salvare le immagini generate.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Osservazioni

L'output([`OutputFile`](../../lowcodesaveoptions/outputfile/) o [`OutputStream`](../../lowcodesaveoptions/outputstream/)) specificato da questa istanza non avrà alcun effetto quando questa proprietà è specificata. Invece, l'output di ogni immagine generata sarà specificato dal provider.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // Crea un'istanza di LowCodeImageSaveOptions
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // Crea un SaveOptionsProvider personalizzato
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // Visualizza il SaveOptionsProvider corrente
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // Dimostra l'effetto salvando con opzioni diverse
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // Cambia al provider null
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Restituisci opzioni di salvataggio personalizzate per ogni parte
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Esegui eventuali pulizie dopo il salvataggio
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### Vedi anche

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


