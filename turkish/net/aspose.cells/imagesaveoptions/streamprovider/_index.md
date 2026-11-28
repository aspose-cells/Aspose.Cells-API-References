---
title: "ImageSaveOptions.StreamProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageSaveOptions özelliği. Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Açıklamalar

Eğer Tiff olarak kaydediliyorsa, bu özellik yok sayılır. Aksi takdirde, birden fazla görüntü kaydedilmesi gerekiyorsa, diğer görüntüleri bununla yazarız. Gelişmiş kullanım için lütfen [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) veya [`SheetRender`](../../../aspose.cells.rendering/sheetrender/) kullanın.

### Örnekler

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
            // Akış sağlanmadığında uygulama
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
            // Çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test StreamProvider");

            // Özel akış sağlayıcı ile kaydetme seçeneklerini ayarla
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new CustomStreamProvider();

            // Akış sağlayıcı ile kaydet
            workbook.Save("output.png", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


