---
title: "Classe LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "classe Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders. Implementazione per fornire opzioni di salvataggio che salvano le parti divise in file e il percorso del file risultante è definito con segnaposti"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

Implementazione per fornire opzioni di salvataggio che salvano le parti divise in file e il percorso del file risultante è definito con segnaposti.

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | Istanzia un'istanza per fornire le opzioni di salvataggio in base ai modelli specificati. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. Il valore predefinito è false, cioè, quando c'è un solo foglio, l'indice e il nome del foglio e il prefisso corrispondente([`SheetNamePrefix`](./sheetnameprefix/)) non verranno aggiunti al percorso del file. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | Indica se aggiungere sempre l'indice della parte divisa al percorso del file. Il valore predefinito è false, cioè, quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente([`SplitPartPrefix`](./splitpartprefix/)) non verranno aggiunti al percorso del file. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | Il modello per creare un'istanza delle opzioni di salvataggio in [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | Prefisso per l'indice del foglio di lavoro. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | Prefisso per l'indice del foglio di lavoro. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | Scostamento dell'indice della parte divisa tra quello usato nel percorso del file e il suo valore reale ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | Prefisso per l'indice della parte divisa. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Rilascia le risorse dopo l'elaborazione della parte divisa corrente (ereditato da [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte divisa corrente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola il foglio di lavoro con dati di esempio
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Crea un provider con modello di percorso contenente segnaposti
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // Configura le proprietà del provider
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // Configura il modello delle opzioni di salvataggio
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Configura le opzioni di immagine o stampa per il rendering diviso
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // Crea il rendering del foglio con configurazione divisa
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### Vedi anche

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


