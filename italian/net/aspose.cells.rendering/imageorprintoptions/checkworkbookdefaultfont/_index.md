---
title: "ImageOrPrintOptions.CheckWorkbookDefaultFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi nell'immagine PDF. Imposta questo valore su true per provare a utilizzare il font predefinito della cartella di lavoro per visualizzare questi caratteri."
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/
---
## ImageOrPrintOptions.CheckWorkbookDefaultFont property

Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per visualizzare prima questi caratteri.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Sample Text");
            
            // Imposta il carattere predefinito per la cartella di lavoro
            workbook.DefaultStyle.Font.Name = "Arial";
            workbook.DefaultStyle.Font.Size = 12;

            // Crea opzioni di immagine o stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Abilita il controllo del carattere predefinito della cartella di lavoro
            options.CheckWorkbookDefaultFont = true;

            // Renderizza il foglio di lavoro in immagine
            SheetRender renderer = new SheetRender(sheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Salva l'immagine su file
                using (FileStream file = new FileStream("output.png", FileMode.Create))
                {
                    stream.WriteTo(file);
                }
            }
            
            Console.WriteLine("Image generated with workbook default font check.");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


