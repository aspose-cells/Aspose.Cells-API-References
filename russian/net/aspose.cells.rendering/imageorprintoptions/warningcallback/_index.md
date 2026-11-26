---
title: "ImageOrPrintOptions.WarningCallback"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Возвращает или задает callback предупреждений"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/warningcallback/
---
## ImageOrPrintOptions.WarningCallback property

Получает или задаёт обратный вызов предупреждения.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте содержимое, которое вызовет предупреждение во время рендеринга
            worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
            Style style = workbook.CreateStyle();
            style.Font.Name = "NonExistentFont";
            worksheet.Cells["A1"].SetStyle(style);

            // Создайте экземпляр ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Отобразить начальное значение WarningCallback
            Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);

            // Создайте и назначьте пользовательский callback предупреждений
            var warningCallback = new RenderingWarningCallback();
            options.WarningCallback = warningCallback;

            // Создайте SheetRender для демонстрации callback во время рендеринга
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_image.png");

            // Проверьте, были ли захвачены предупреждения
            Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
        }
    }

    // Пользовательская реализация callback для обработки предупреждений рендеринга
    public class RenderingWarningCallback : IWarningCallback
    {
        public int WarningCount { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            // Обработать предупреждения о замене шрифтов
            if (warningInfo.WarningType == WarningType.FontSubstitution)
            {
                Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
                WarningCount++;
            }
        }
    }
}
```

### См. также

* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


