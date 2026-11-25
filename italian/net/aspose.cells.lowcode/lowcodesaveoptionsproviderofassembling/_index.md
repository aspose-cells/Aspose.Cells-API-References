---
title: "Classe LowCodeSaveOptionsProviderOfAssembling"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "classe Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling. Implementazione per fornire opzioni di salvataggio che salvano le parti divise in file e il percorso del file risultante è denominato come può contenere directory PathHeaderSheetPrefixSheetIndexor SheetName SplitPartPrefixSplitPartIndexPathTail"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

Implementazione per fornire opzioni di salvataggio che salvano le parti divise in file e il percorso del file risultante è denominato come (può contenere directory): [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(o SheetName) +[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. Il valore predefinito è false, cioè, quando c'è un solo foglio, l'indice (o il nome) del foglio e il prefisso corrispondente non verranno aggiunti al percorso del file. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | Indica se aggiungere sempre l'indice della parte divisa al percorso del file. Il valore predefinito è false, cioè, quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente non verranno aggiunti al percorso del file. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | Parte intestazione (prima del contenuto aggiunto del foglio e della parte divisa) del percorso del file. |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | Parte finale (dopo i numeri di sequenza) del percorso del file. Deve includere l'estensione del nome file. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | Il modello per creare un'istanza delle opzioni di salvataggio in [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | Prefisso per l'indice del foglio di lavoro. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | Scostamento dell'indice della parte divisa tra quello usato nel percorso del file e il suo valore reale ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | Prefisso per l'indice della parte divisa. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | Indica se costruire il percorso del file con il nome del foglio invece dell'indice del foglio. Il valore predefinito è false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Rilascia le risorse dopo l'elaborazione della parte divisa corrente (ereditato da [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte divisa corrente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // Inizializza e configura il provider delle opzioni di salvataggio
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Configura le opzioni di salvataggio XLSX con divisione usando LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Salva la cartella di lavoro con le opzioni abilitate dal provider usando il formato di salvataggio corretto
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### Vedi anche

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


