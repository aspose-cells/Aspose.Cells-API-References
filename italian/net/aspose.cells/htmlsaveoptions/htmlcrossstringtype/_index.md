---
title: "HtmlSaveOptions.HtmlCrossStringType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se una stringa crosscell verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato html. Per impostazione predefinita il valore è Default, quindi per le stringhe crosscell c'è poca differenza tra i file html creati da Aspose.Cells e MS Excel. Tuttavia le prestazioni per la creazione di grandi file html impostando il valore su Cross sarebbero diverse volte più rapide rispetto a impostarlo su Default o Fit2Cell"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato HTML. Per impostazione predefinita il valore è Default, quindi, per le stringhe che attraversano più celle, c'è poca differenza tra i file HTML creati da Aspose.Cells e MS Excel. Tuttavia le prestazioni per la creazione di file HTML di grandi dimensioni, impostando il valore su Cross, sarebbero diverse volte più rapide rispetto a impostarlo su Default o Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio che dimostreranno il comportamento delle stringhe cross
            worksheet.Cells["A1"].PutValue("Left Content");
            worksheet.Cells["B1"].PutValue("Right Content");
            
            // Ottieni e modifica gli stili delle celle
            Style styleA1 = worksheet.Cells["A1"].GetStyle();
            styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["A1"].SetStyle(styleA1);
            
            Style styleB1 = worksheet.Cells["B1"].GetStyle();
            styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["B1"].SetStyle(styleB1);

            // Configura le opzioni di salvataggio HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            // Salva la cartella di lavoro in HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with CrossHideRight option.");
        }
    }
}
```

### Vedi anche

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


