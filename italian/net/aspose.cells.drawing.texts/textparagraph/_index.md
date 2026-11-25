---
title: "Classe TextParagraph"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Texts.TextParagraph. Rappresenta l'impostazione del paragrafo di testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/
---
## TextParagraph class

Rappresenta l'impostazione del paragrafo di testo.

```csharp
public class TextParagraph : FontSetting
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | Ottiene e imposta il tipo di allineamento orizzontale del testo del paragrafo. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | Ottiene il bullet. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | Ottiene tutti i run di testo in questo paragrafo. Se questo paragrafo è vuoto, restituisce lo stesso paragrafo. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | Ottiene e imposta la dimensione predefinita per un carattere di tabulazione all'interno di questo paragrafo. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | Specifica la dimensione dell'indentazione che verrà applicata alla prima riga di testo del paragrafo. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Restituisce il font di questo oggetto.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | Determina dove, verticalmente, su una riga di testo, le parole effettive sono posizionate. Questo riguarda il posizionamento verticale dei caratteri rispetto alle linee di base. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | Specifica se una parola dell'Est asiatico può essere divisa a metà e spostata alla riga successiva senza aggiungere un trattino. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | Specifica se la punteggiatura deve essere forzatamente posizionata su una riga di testo o spostata su una riga diversa. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | Specifica se una parola latina può essere divisa a metà e spostata alla riga successiva senza aggiungere un trattino. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | Specifica il margine sinistro del paragrafo. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Ottiene la lunghezza dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | Ottiene e imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | Ottiene e imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | Specifica il margine destro del paragrafo. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | Ottiene e imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | Ottiene e imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | Ottiene e imposta la quantità di spazio bianco verticale che sarà presente prima di un paragrafo. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | Ottiene e imposta la quantità di spazio bianco verticale che sarà presente prima di un paragrafo. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Ottiene l'indice iniziale dei caratteri.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | Ottiene l'elenco dei tabulatori. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Restituisce le opzioni di testo.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | Ottiene il tipo di nodo di testo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Imposta lo stile WordArt predefinito.(Ereditato da [`FontSetting`](../../aspose.cells/fontsetting/).) |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
            
            // Imposta il contenuto di testo con più paragrafi
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Accedi e modifica i paragrafi di testo
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                // Imposta le proprietà del paragrafo
                paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
                paragraph.LineSpace = 20;
                paragraph.AlignmentType = TextAlignmentType.Center;
            }

            // Salva la cartella di lavoro
            workbook.Save("TextParagraphDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


