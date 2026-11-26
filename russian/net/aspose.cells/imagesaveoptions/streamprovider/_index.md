---
title: "ImageSaveOptions.StreamProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageSaveOptions. Получает или задает IStreamProvider для экспорта объектов"
type: docs
url: /ru/net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

Получает или задает IStreamProvider для экспорта объектов.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Примечания

Если сохраняется как Tiff, это свойство игнорируется. В противном случае, если нужно сохранить более одного изображения, мы будем записывать остальные изображения с помощью этого свойства. Для расширенного использования, пожалуйста, используйте [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) или [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Примеры

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
            // Реализация, когда поток не предоставлен
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
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test StreamProvider");

            // Установите параметры сохранения с пользовательским провайдером потока
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new CustomStreamProvider();

            // Сохранить с провайдером потока
            workbook.Save("output.png", saveOptions);
        }
    }
}
```

### См. также

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


