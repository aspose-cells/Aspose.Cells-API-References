---
title: "TextOptions.Kerning"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Указывает минимальный размер шрифта, при котором будет применяться кернинг символов для этого текстового фрагмента"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/kerning/
---
## TextOptions.Kerning property

Указывает минимальный размер шрифта, при котором будет применяться кернинг символов в этой последовательности текста.

```csharp
public double Kerning { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyKerningDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму с текстом, чтобы продемонстрировать кернинг
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Kerning Demonstration Text";

            // Получите TextOptions формы
            TextOptions textOptions = shape.TextOptions;

            // Отобразить текущее значение кернинга
            Console.WriteLine("Current Kerning value: " + textOptions.Kerning);

            // Установите кернинг на 12 пунктов (минимальный размер шрифта для применения кернинга)
            textOptions.Kerning = 12;

            // Установите больший размер шрифта, чтобы наблюдать эффект кернинга
            textOptions.Size = 24;

            // Сохранить рабочую книгу, чтобы увидеть эффект
            workbook.Save("PropertyKerningDemo.xlsx");

            // Создайте другую фигуру с другим кернингом для сравнения
            var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
            shape2.Text = "Comparison Text Without Kerning";
            shape2.TextOptions.Size = 24;
            shape2.TextOptions.Kerning = 0; // No kerning

            // Сохраните снова с обоими примерами
            workbook.Save("PropertyKerningDemoWithComparison.xlsx");
        }
    }
}
```

### См. также

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


