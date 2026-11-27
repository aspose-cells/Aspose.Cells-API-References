---
title: "ImageSaveOptions.StreamProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageSaveOptions‑egenskap. Hämtar eller anger IStreamProvider för att exportera objekt"
type: docs
url: /sv/net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

Hämtar eller anger IStreamProvider för export av objekt.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Anmärkningar

Om du sparar som Tiff ignoreras denna egenskap. Annars, om mer än en bild ska sparas, kommer vi att skriva andra bilder med detta. För avancerad användning, använd [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) eller [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Exempel

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
            // Implementering när ingen ström tillhandahålls
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
            // Skapa arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test StreamProvider");

            // Ställ in sparalternativ med anpassad strömleverantör
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new CustomStreamProvider();

            // Spara med strömleverantör
            workbook.Save("output.png", saveOptions);
        }
    }
}
```

### Se även

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


