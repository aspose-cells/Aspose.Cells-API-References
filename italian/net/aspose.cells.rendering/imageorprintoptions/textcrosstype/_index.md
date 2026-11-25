---
title: "ImageOrPrintOptions.TextCrossType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/textcrosstype/
---
## ImageOrPrintOptions.TextCrossType property

Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta un testo lungo che supererà la larghezza della cella
            worksheet.Cells["A1"].PutValue("This is a long text that exceeds cell width");
            worksheet.Cells["A1"].GetStyle().ShrinkToFit = false;

            // Crea opzioni di immagine o stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Dimostra diverse impostazioni di TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveAsImage(workbook, options, "TextCrossType_Default.png");

            options.TextCrossType = TextCrossType.CrossKeep;
            SaveAsImage(workbook, options, "TextCrossType_CrossKeep.png");

            options.TextCrossType = TextCrossType.CrossOverride;
            SaveAsImage(workbook, options, "TextCrossType_CrossOverride.png");

            options.TextCrossType = TextCrossType.StrictInCell;
            SaveAsImage(workbook, options, "TextCrossType_StrictInCell.png");
        }

        private static void SaveAsImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Vedi anche

* enum [TextCrossType](../../../aspose.cells/textcrosstype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


