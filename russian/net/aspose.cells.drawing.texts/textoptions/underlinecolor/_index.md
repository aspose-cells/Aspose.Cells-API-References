---
title: "TextOptions.UnderlineColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Получает или задает цвет подчеркивания"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/underlinecolor/
---
## TextOptions.UnderlineColor property

Получает или задает цвет подчеркивания.

```csharp
public CellsColor UnderlineColor { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyUnderlineColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму с текстом, чтобы продемонстрировать параметры текста
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Underline Color Demo";
            
            // Получите TextOptions из формы
            TextOptions textOptions = shape.TextOptions;

            try
            {
                // Отобразить текущее значение UnderlineColor
                CellsColor currentColor = textOptions.UnderlineColor;
                Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");

                // Установить новое значение UnderlineColor (поскольку свойство доступно для чтения и записи)
                CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
                newColor.Color = System.Drawing.Color.Red;
                textOptions.UnderlineColor = newColor;

                // Включите подчеркивание, чтобы увидеть эффект
                textOptions.Underline = FontUnderlineType.Single;

                // Отобразить новое значение UnderlineColor
                Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");

                // Сохранить рабочую книгу, чтобы увидеть эффект
                workbook.Save("UnderlineColorDemo.xlsx");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


