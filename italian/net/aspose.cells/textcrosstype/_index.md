---
title: "Enum TextCrossType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.TextCrossType. Elenca i tipi di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella"
type: docs
url: /it/net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

Enumera il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella.

```csharp
public enum TextCrossType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `1` | Visualizza il testo come in Microsoft Excel. |
| CrossKeep | `2` | Visualizza tutto il testo attraversando altre celle e conserva il testo delle celle attraversate. |
| CrossOverride | `3` | Visualizza tutto il testo attraversando altre celle e sovrascrivi il testo delle celle attraversate. |
| StrictInCell | `4` | Visualizza solo il testo entro la larghezza della cella. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassTextCrossTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta testo di esempio in una cella che potrebbe traboccare
            worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
            
            // Crea opzioni di immagine o stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Dimostra diverse impostazioni di TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveToImage(workbook, options, "TextCrossType_Default.png");
            
            options.TextCrossType = TextCrossType.CrossKeep;
            SaveToImage(workbook, options, "TextCrossType_CrossKeep.png");
            
            options.TextCrossType = TextCrossType.CrossOverride;
            SaveToImage(workbook, options, "TextCrossType_CrossOverride.png");
            
            options.TextCrossType = TextCrossType.StrictInCell;
            SaveToImage(workbook, options, "TextCrossType_StrictInCell.png");
        }
        
        private static void SaveToImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


