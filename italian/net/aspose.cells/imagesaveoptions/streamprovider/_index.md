---
title: "ImageSaveOptions.StreamProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageSaveOptions. Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti"
type: docs
url: /it/net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Osservazioni

Se si salva come Tiff, questa proprietà è ignorata. Altrimenti, se deve essere salvata più di un'immagine, scriveremo le altre immagini con questa. Per un utilizzo avanzato, si prega di utilizzare [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) o [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomStreamProvider : IStreamProvider
    {
        private int m_count = 0;

        public void InitStream(StreamProviderOptions options)
        {
            m_count++;
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            return new FileStream(options.DefaultPath + m_count + ".png", FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementazione quando non viene fornito alcuno stream
        }

        public void CloseStream(StreamProviderOptions options, Stream stream)
        {
            stream.Dispose();
        }
    }

    public class ImageSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Crea cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test StreamProvider");

            // Imposta le opzioni di salvataggio con un provider di stream personalizzato
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new CustomStreamProvider();

            // Salva con il provider di stream
            workbook.Save("output.png", saveOptions);
        }
    }
}
```

### Vedi anche

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


