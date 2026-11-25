---
title: "Enum StyleModifyFlag"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.StyleModifyFlag. I flag di modifica dello stile"
type: docs
url: /it/net/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enumeration

I flag di stile modificati.

```csharp
public enum StyleModifyFlag
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| LeftBorder | `256` | Indica se il bordo sinistro è stato modificato per lo stile. |
| RightBorder | `512` | Indica se il bordo destro è stato modificato per lo stile. |
| TopBorder | `1024` | Indica se il bordo superiore è stato modificato per lo stile. |
| BottomBorder | `2048` | Indica se il bordo inferiore è stato modificato per lo stile. |
| DiagonalDownBorder | `4096` | Indica se il bordo diagonale-giù è stato modificato per lo stile. |
| DiagonalUpBorder | `8192` | Indica se il bordo diagonale-su è stato modificato per lo stile. |
| HorizontalBorder | `32` | Indica se il bordo orizzontale è stato modificato per lo stile. Solo per stili dinamici, come la formattazione condizionale. |
| VerticalBorder | `64` | Indica se il bordo verticale è stato modificato per lo stile. Solo per stili dinamici, come la formattazione condizionale. |
| SideBorders | `3840` | Indica i quattro bordi laterali: LeftBorder, RightBorder, TopBorder e BottomBorder. |
| Diagonal | `12288` | Indica i bordi diagonali: DiagonalDownBorder e DiagonalUpBorder. |
| DynamicStyleBorders | `96` | Indica i bordi dello stile dinamico: HorizontalBorder e VerticalBorder. |
| Borders | `16224` | Indica se uno o più bordi (LeftBorder, RightBorder, TopBorder, BottomBorder, Diagonal, HorizontalBorder, VerticalBorder) sono stati modificati per lo stile. |
| NumberFormat | `16384` | Indica se numberformat è stato modificato. |
| HorizontalAlignment | `32768` | Indica se l'allineamento orizzontale è stato modificato. |
| VerticalAlignment | `65536` | Indica se l'allineamento verticale è stato modificato. |
| Indent | `131072` | Indica se la proprietà indent è stata modificata. |
| Rotation | `262144` | Indica se la proprietà rotation è stata modificata. |
| WrapText | `524288` | Indica se la proprietà wrap text è stata modificata. |
| ShrinkToFit | `1048576` | Indica se la proprietà shrink to fit è stata modificata. |
| TextDirection | `2097152` | Indica se la proprietà text direction è stata modificata. |
| RelativeIndent | `128` | Indica se la proprietà relative indent è stata modificata per lo stile. Solo per stili dinamici, come la formattazione condizionale. |
| AlignmentSettings | `4161664` | Indica se una o più proprietà relative all'allineamento (HorizontalAlignment, VerticalAlignment, Rotation, WrapText, WrapText, Indent, ShrinkToFit, TextDirection, RelativeIndent) sono state modificate. |
| Pattern | `4194304` | Indica se il pattern dell'ombreggiatura è stato modificato. |
| ForegroundColor | `8388608` | Indica se il colore di primo piano è stato modificato. |
| BackgroundColor | `16777216` | Indica se il colore di sfondo è stato modificato. |
| CellShading | `29360128` | Indica se una o più proprietà relative all'ombreggiatura (Pattern, ForegroundColor, BackgroundColor) sono state modificate. |
| Locked | `67108864` | Indica se la proprietà locked è stata modificata. |
| HideFormula | `134217728` | Indica se la proprietà hide formula è stata modificata. |
| ProtectionSettings | `201326592` | Indica se una o più proprietà relative alla protezione (Locked, HideFormula) sono state modificate. |
| FontSize | `1` | Indica se la dimensione del carattere è stata modificata. |
| FontName | `2` | Indica se il nome del carattere è stato modificato. |
| FontColor | `3` | Indica se il colore del carattere è stato modificato. |
| FontWeight | `4` | Indica se lo spessore del carattere è stato modificato. |
| FontItalic | `5` | Indica se la proprietà italic del carattere è stata modificata. |
| FontUnderline | `6` | Indica se la proprietà underline del carattere è stata modificata. |
| FontStrike | `7` | Indica se la proprietà strike del carattere è stata modificata. |
| FontScript | `8` | Indica se la proprietà subscript o superscript del carattere è stata modificata. |
| FontFamily | `9` | Indica se la famiglia di caratteri è stata modificata. |
| FontCharset | `10` | Indica se il set di caratteri del font è stato modificato. |
| FontScheme | `11` | non utilizzato. |
| FontDirty | `12` | non utilizzato. |
| FontSpellingError | `13` | non utilizzato. |
| FontUFillTx | `14` | non utilizzato. |
| FontSpacing | `15` | non utilizzato. |
| FontKerning | `16` | non utilizzato. |
| FontEqualize | `17` | non utilizzato. |
| FontCap | `18` | non utilizzato. |
| FontVerticalText | `19` |  |
| Font | `31` | Indica se una o più proprietà del font dello stile sono state modificate. |
| All | `234881023` | Tutte le proprietà che possono essere modificate per lo stile. |
| None | `0` | Nessuna proprietà è stata specificata. |

### Osservazioni

Le combinazioni di più proprietà sono definite per comodità dell'utente. Quando si verifica se sono state modificate per uno stile, il valore restituito indica se una o più proprietà nella combinazione sono state modificate.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleModifyFlagDemo
    {
        public static void StyleModifyFlagExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni valori nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A2"].PutValue(123.45);

            // Crea un nuovo stile
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // Applica lo stile a una cella
            worksheet.Cells["A1"].SetStyle(style);

            // Verifica quali proprietà dello stile sono state modificate
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // Restituisci i risultati
            Console.WriteLine("Font Modified: " + isFontModified);
            Console.WriteLine("Font Size Modified: " + isFontSizeModified);
            Console.WriteLine("Font Color Modified: " + isFontColorModified);
            Console.WriteLine("Horizontal Alignment Modified: " + isHorizontalAlignmentModified);

            // Salva la cartella di lavoro
            workbook.Save("StyleModifyFlagExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


