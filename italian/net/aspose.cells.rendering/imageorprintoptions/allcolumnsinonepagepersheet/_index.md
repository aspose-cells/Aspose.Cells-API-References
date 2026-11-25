---
title: "ImageOrPrintOptions.AllColumnsInOnePagePerSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà emesso su una sola pagina nel risultato. La larghezza della dimensione della carta di pagesetup sarà invalida e le altre impostazioni di pagesetup continueranno ad avere effetto"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/
---
## ImageOrPrintOptions.AllColumnsInOnePagePerSheet property

Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà output su una sola pagina nel risultato. La larghezza della dimensione della carta del pagesetup sarà invalida, e le altre impostazioni del pagesetup continueranno ad avere effetto.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci alcuni dati nel foglio di lavoro
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crea opzioni di salvataggio dell'immagine
            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;

            // Salva la cartella di lavoro in uno stream di memoria come PNG
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, pngOptions);
                Console.WriteLine("Workbook saved as PNG with all columns in one page per sheet.");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


