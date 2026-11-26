---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Настройка рендеринга EMF‑метафайлов в исходном файле"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

Настройка рендеринга Emf метафайлов в исходном файле.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Примечания

EMF‑метафайлы, идентифицированные как "EMF+ Dual", могут содержать как записи EMF+, так и записи EMF. Любой тип записей может быть использован для рендеринга изображения, только записи EMF+, или только записи EMF. Когда параметр EmfPlusPrefer установлен, при рендеринге изображения будут обрабатываться записи EMF+, иначе будут обрабатываться только записи EMF. Значение по умолчанию — EmfOnly. Для фреймворков, зависящих от .NET System.Drawing.Common, эта настройка игнорируется.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Создать новую рабочую книгу с тестовым содержимым
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // Создать параметры рендеринга изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // Отобразить текущую настройку
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // Выполнить рендеринг с настройками EMF по умолчанию
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // Измените настройку рендеринга EMF и отрендерьте снова
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### См. также

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


