---
title: "Classe StyleFlag"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.StyleFlag. Rappresenta i flag che indicano le proprietà di formattazione applicate."
type: docs
url: /it/net/aspose.cells/styleflag/
---
## StyleFlag class

Rappresenta i flag che indicano le proprietà di formattazione applicate.

```csharp
public class StyleFlag
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [StyleFlag](styleflag/)() | Costruisce un oggetto con tutti i flag impostati a false. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | L'impostazione di allineamento verrà applicata. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | Tutte le proprietà verranno applicate. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | Tutte le impostazioni dei bordi verranno applicate. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | Le impostazioni del bordo inferiore verranno applicate. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | L'impostazione di ombreggiatura della cella sarà applicata. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | Le impostazioni del bordo diagonale verso il basso saranno applicate. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | Le impostazioni del bordo diagonale verso l'alto saranno applicate. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | Le impostazioni del carattere saranno applicate. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | L'impostazione di grassetto del carattere sarà applicata. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | L'impostazione del colore del carattere sarà applicata. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | L'impostazione di corsivo del carattere sarà applicata. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | L'impostazione del nome del carattere sarà applicata. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | L'impostazione dello script del carattere sarà applicata. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | L'impostazione della dimensione del carattere sarà applicata. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | L'impostazione di barrato del carattere sarà applicata. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | L'impostazione di sottolineatura del carattere sarà applicata. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | L'impostazione di nascondi formula sarà applicata. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | L'impostazione di allineamento orizzontale sarà applicata. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | L'impostazione del livello di rientro sarà applicata. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | Le impostazioni del bordo sinistro saranno applicate. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | L'impostazione di blocco sarà applicata. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | L'impostazione del formato numerico sarà applicata. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | L'impostazione di nascondi formula sarà applicata. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | Le impostazioni del bordo destro saranno applicate. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | L'impostazione di rotazione sarà applicata. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | L'impostazione di riduzione per adattamento sarà applicata. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | L'impostazione della direzione del testo sarà applicata. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | Le impostazioni del bordo superiore saranno applicate. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | L'impostazione di allineamento verticale sarà applicata. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | L'impostazione di a capo automatico sarà applicata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagDemo
    {
        public static void StyleFlagExample()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Crea un nuovo oggetto stile
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Crea un nuovo oggetto StyleFlag
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // Applica lo stile a un intervallo di celle
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // Salva la cartella di lavoro
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


