---
title: "HtmlSaveOptions.ImageScalable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizza unità scalabili per descrivere la larghezza della colonna. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/imagescalable/
---
## HtmlSaveOptions.ImageScalable property

Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizza unità scalabili per descrivere la larghezza della colonna. Il valore predefinito è true.

```csharp
public bool ImageScalable { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageScalableDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con un'immagine
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'immagine di esempio al foglio di lavoro
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[imgIndex];

            // Imposta le opzioni di salvataggio HTML con la proprietà ImageScalable
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ImageScalable = false; // Images won't scale with the HTML content
            
            // Salva la cartella di lavoro come HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with ImageScalable set to false.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


