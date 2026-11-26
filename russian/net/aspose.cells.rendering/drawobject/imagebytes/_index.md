---
title: "DrawObject.ImageBytes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DrawObject. Указывает байты изображения отрисованной формы диаграммы при рендеринге"
type: docs
url: /ru/net/aspose.cells.rendering/drawobject/imagebytes/
---
## DrawObject.ImageBytes property

Указывает байты изображения отрисованного Chart, Shape при рендеринге.

```csharp
public byte[] ImageBytes { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class DrawObjectPropertyImageBytesDemo
    {
        // Пользовательский обработчик события для захвата байтов изображения
        private class ImageBytesHandler : DrawObjectEventHandler
        {
            public byte[] CapturedImageBytes { get; private set; }

            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                if (drawObject.Type == DrawObjectEnum.Image)
                {
                    CapturedImageBytes = drawObject.ImageBytes;
                    Console.WriteLine($"Captured image size: {CapturedImageBytes?.Length ?? 0} bytes");
                }
            }
        }

        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PNG‑изображение 1×1 красного пикселя, закодированное в Base64
            byte[] generatedImageBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");

            // Добавьте сгенерированное изображение в лист, используя поток
            using (MemoryStream imageStream = new MemoryStream(generatedImageBytes))
            {
                worksheet.Pictures.Add(0, 0, imageStream);
            }

            // Настройте параметры рендеринга
            ImageOrPrintOptions renderOptions = new ImageOrPrintOptions();
            renderOptions.ImageType = ImageType.Png;

            // Создайте экземпляр обработчика и назначьте его параметрам
            var imageHandler = new ImageBytesHandler();
            renderOptions.DrawObjectEventHandler = imageHandler;

            SheetRender sheetRenderer = new SheetRender(worksheet, renderOptions);
            
            // Отобразите лист, чтобы вызвать событие DrawObject, используя фиктивный поток
            using (MemoryStream dummyStream = new MemoryStream())
            {
                sheetRenderer.ToImage(0, dummyStream);
            }

            // Добавьте захваченное изображение в лист, если оно доступно
            byte[] capturedImageBytes = imageHandler.CapturedImageBytes;
            if (capturedImageBytes != null)
            {
                int newRowPosition = worksheet.Cells.MaxDataRow + 2;
                using (MemoryStream capturedStream = new MemoryStream(capturedImageBytes))
                {
                    worksheet.Pictures.Add(newRowPosition, 0, capturedStream);
                }
            }

            // Сохранить изменённую книгу
            workbook.Save("ImageBytesDemo.xlsx");
        }
    }
}
```

### См. также

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


