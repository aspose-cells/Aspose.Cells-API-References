---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeImageSaveOptions. Получает или задает формат сохранения"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

Получает или задает формат сохранения.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Примечания

Если указаны [`ImageOptions`](../imageoptions/), установка этого свойства также изменит значение [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/) у него.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // Инициализируйте LowCodeImageSaveOptions со значениями по умолчанию
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // Отобразите начальный SaveFormat (по умолчанию - Png)
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Настройте вывод в формате JPEG
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // Переключите на формат PNG и сохраните снова
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // Отобразите лист, используя настроенные параметры
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### См. также

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


