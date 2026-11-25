---
title: "Classe AutoFitterOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AutoFitterOptions. Rappresenta tutte le opzioni di auto‑fit."
type: docs
url: /it/net/aspose.cells/autofitteroptions/
---
## AutoFitterOptions class

Rappresenta tutte le opzioni dell'auto fitter.

```csharp
public class AutoFitterOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) Indica se adattare automaticamente l'altezza della riga quando le celle sono unite in una riga. Il valore predefinito è false. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | Ottiene e imposta il tipo di adattamento automatico dell'altezza della riga per le celle unite. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | Ottiene e imposta il tipo di adattamento automatico del testo a capo. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | Ottiene o imposta la lingua di modifica predefinita. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | Ottiene e imposta la strategia di formattazione. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | Indica se adattare per scopi di rendering. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | Ignora le righe/colonne nascoste. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | Ottiene e imposta l'altezza massima della riga (in unità di Point) durante l'adattamento automatico delle righe. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | Indica se adattare solo le righe la cui altezza non è personalizzata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitterOptionsDemo
    {
        public static void AutoFitterOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // Creare un intervallo A1:B2
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // Unisci le celle
            range.Merge();

            // Crea un'istanza di AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // Applica l'adattamento automatico delle righe con le opzioni specificate
            worksheet.AutoFitRows(options);

            // Salva la cartella di lavoro
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


