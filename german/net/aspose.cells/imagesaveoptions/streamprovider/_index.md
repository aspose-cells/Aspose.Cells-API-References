---
title: "ImageSaveOptions.StreamProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageSaveOptions-Eigenschaft. Gibt den IStreamProvider zum Exportieren von Objekten zurück oder setzt ihn"
type: docs
url: /de/net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

Liest oder setzt den IStreamProvider für den Export von Objekten.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Hinweise

Wenn als Tiff gespeichert wird, wird diese Eigenschaft ignoriert. Andernfalls, wenn mehr als ein Bild gespeichert werden soll, schreiben wir weitere Bilder damit. Für erweiterte Nutzung bitte [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) oder [`SheetRender`](../../../aspose.cells.rendering/sheetrender/) verwenden.

### Beispiele

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
            // Implementierung, wenn kein Stream bereitgestellt wird
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
            // Arbeitsmappe erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test StreamProvider");

            // Speicheroptionen mit benutzerdefiniertem Stream-Provider festlegen
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new CustomStreamProvider();

            // Mit Stream-Provider speichern
            workbook.Save("output.png", saveOptions);
        }
    }
}
```

### Siehe auch

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


