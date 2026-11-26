---
title: "Класс LowCodeImageSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LowCode.LowCodeImageSaveOptions класс. Параметры сохранения изображения в режиме low code"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

Параметры сохранения изображения в режиме low code.

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | Параметры рендеринга изображений. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Получает и задает файл (с путем, если необходимо) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, [`OutputStream`](../lowcodesaveoptions/outputstream/) будет игнорироваться. (Унаследовано от [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Получает и задает поток для записи сгенерированных данных. При установке этого свойства значением, отличным от null, [`OutputFile`](../lowcodesaveoptions/outputfile/) будет игнорироваться. (Унаследовано от [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | Получает или задает формат сохранения. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | Поставщик параметров сохранения для сохранения сгенерированных изображений. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить примерные данные в лист
                worksheet.Cells["A1"].PutValue("LowCode Image Save Demo");
                worksheet.Cells["A2"].PutValue("This demonstrates LowCodeImageSaveOptions");

                // Создайте экземпляр LowCodeImageSaveOptions
                LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();

                // Установите базовые свойства
                saveOptions.SaveFormat = SaveFormat.Png;
                saveOptions.ImageOptions = new ImageOrPrintOptions();

                // Отобразить текущие настройки
                Console.WriteLine("SaveFormat: " + saveOptions.SaveFormat);
                Console.WriteLine("ImageOptions HorizontalResolution: " +
                    saveOptions.ImageOptions.HorizontalResolution);

                // Изменить некоторые параметры изображения
                saveOptions.ImageOptions.HorizontalResolution = 300;
                saveOptions.ImageOptions.VerticalResolution = 300;

                // Создайте простой поставщик параметров сохранения
                saveOptions.SaveOptionsProvider = new SimpleSaveOptionsProvider();

                // Сохраните лист как изображение
                SheetRender renderer = new SheetRender(worksheet, saveOptions.ImageOptions);
                renderer.ToImage(0, "LowCodeImageOutput.png");

                Console.WriteLine("Image saved successfully with LowCodeImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LowCodeImageSaveOptions: {ex.Message}");
            }
        }
    }

    public class SimpleSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Png,
                ImageOptions = new ImageOrPrintOptions()
                {
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


