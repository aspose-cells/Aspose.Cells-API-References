---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор ImageSaveOptions. Создаёт параметры для сохранения файла изображения"
type: docs
url: /ru/net/aspose.cells/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions() {#constructor}

Создаёт параметры для сохранения файла изображения.

```csharp
public ImageSaveOptions()
```

### Примечания

Тип по умолчанию — Tiff.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ImageSaveOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Продемонстрировать конструктор без параметров
                ImageSaveOptions defaultOptions = new ImageSaveOptions();
                Console.WriteLine("Created ImageSaveOptions with default constructor");

                // Продемонстрировать конструктор с параметром SaveFormat
                ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
                Console.WriteLine("Created ImageSaveOptions with SaveFormat.Png");

                // Получите доступ к только для чтения свойству ImageOrPrintOptions
                var imageOptions = pngOptions.ImageOrPrintOptions;
                Console.WriteLine($"ImageOrPrintOptions type: {imageOptions.GetType().Name}");

                // Установите свойство StreamProvider
                pngOptions.StreamProvider = null;
                Console.WriteLine("StreamProvider set to null");

                // Сохраните книгу с созданными параметрами
                workbook.Save("output.png", pngOptions);
                Console.WriteLine("Workbook saved successfully with ImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImageSaveOptions(SaveFormat) {#constructor_1}

Создаёт параметры для сохранения файла изображения.

```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат файла. Он должен быть одним из следующих типов: Tiff, Svg, Bmp, Png, Jpg, Emf или Gif, в противном случае формат сохранения будет автоматически установлен как Tiff. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и добавьте тестовые данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Save Demo");
            
            // Создайте ImageSaveOptions с SaveFormat.Tiff
            try
            {
                ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Tiff);
                
                // Настройте параметры рендеринга изображения
                saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
                saveOptions.ImageOrPrintOptions.VerticalResolution = 300;

                // Сохраните книгу в виде многостраничного TIFF
                workbook.Save("WorksheetImage.tiff", saveOptions);
                
                Console.WriteLine("Workbook successfully saved as TIFF image with 300 DPI resolution.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image save operation: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


