---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LowCodeSaveOptionsProviderOfPlaceHolders proprietà. Il modello per creare un'istanza di opzioni di salvataggio in GetSaveOptions"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate property

Il modello per creare un'istanza delle opzioni di salvataggio in [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Osservazioni

Se il modello è stato specificato, l'istanza creata copierà tutte le impostazioni da esso e aggiornerà il file di output di conseguenza.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            
            // Inizializza il provider con il modello di percorso contenente segnaposti
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/Sheet_{sheet}_Part_{part}.pdf");
            
            // Visualizza lo stato iniziale del modello
            Console.WriteLine($"Initial SaveOptionsTemplate: {(provider.SaveOptionsTemplate == null ? "Not set" : "Configured")}");
            
            // Crea e configura un nuovo modello di opzioni di salvataggio
            provider.SaveOptionsTemplate = new LowCodePdfSaveOptions
            {
                PdfOptions = new PdfSaveOptions  // Fixed property name from PdfSaveOptions to PdfOptions
                {
                    Compliance = PdfCompliance.PdfA1a,
                    ExportDocumentStructure = true
                }
            };

            // Configura i parametri di divisione
            provider.BuildPathWithSheetAlways = true;
            provider.SplitPartPrefix = "Split_";
            
            // Visualizza le opzioni PDF configurate
            var pdfOptions = (LowCodePdfSaveOptions)provider.SaveOptionsTemplate;
            Console.WriteLine($"Configured PDF Compliance: {pdfOptions.PdfOptions.Compliance}");  // Fixed property access
            Console.WriteLine($"Document Structure Export: {pdfOptions.PdfOptions.ExportDocumentStructure}");  // Fixed property access

            // Aggiungi interruzione di pagina per creare parti divise
            worksheet.HorizontalPageBreaks.Add(0);
            
            // Salva utilizzando la configurazione del provider (la divisione/salvataggio reale avverrebbe qui)
            Console.WriteLine("Workbook prepared with SaveOptionsTemplate configuration");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


