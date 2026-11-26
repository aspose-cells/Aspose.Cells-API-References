---
title: "TextOptions.LatinName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Получает и задает латинское имя"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/latinname/
---
## TextOptions.LatinName property

Получает и задает латинское название.

```csharp
public string LatinName { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyLatinNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму, чтобы продемонстрировать параметры текста
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Text = "Sample Text";

            // Получите TextOptions из первого абзаца формы
            TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;

            // Отобразить текущее значение LatinName
            Console.WriteLine("Current LatinName value: " + textOptions.LatinName);

            // Установить новое значение LatinName
            textOptions.LatinName = "Times New Roman";

            // Создайте другую форму для сравнения отображения шрифта
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
            shape2.Text = "Comparison Text";
            shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";

            // Сохраните книгу, чтобы увидеть эффекты
            workbook.Save("PropertyLatinNameDemo.xlsx");

            // Отобразить новое значение LatinName
            Console.WriteLine("New LatinName value: " + textOptions.LatinName);
        }
    }
}
```

### См. также

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


