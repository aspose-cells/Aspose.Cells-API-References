---
title: "TextOptions.Spacing"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Указывает интервал между символами в текстовом фрагменте"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/spacing/
---
## TextOptions.Spacing property

Указывает интервал между символами в последовательности текста.

```csharp
public double Spacing { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertySpacingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
            textBox.Text = "Sample Text with Spacing";

            // Получите параметры текста текстового поля
            TextOptions textOptions = textBox.TextOptions;

            // Отобразите текущее значение интервала
            Console.WriteLine("Current Spacing value: " + textOptions.Spacing);

            // Установите новые значения интервала и посмотрите результаты
            textOptions.Spacing = 2.0; // Increased spacing
            Console.WriteLine("Text with increased spacing (2.0)");

            // Сохраните книгу с первым интервалом
            workbook.Save("TextSpacingDemo1.xlsx");

            // Измените интервал на отрицательное значение (символы ближе друг к другу)
            textOptions.Spacing = -1.0;
            Console.WriteLine("Text with decreased spacing (-1.0)");

            // Сохраните книгу со вторым интервалом
            workbook.Save("TextSpacingDemo2.xlsx");

            // Сбросьте к интервалу по умолчанию
            textOptions.Spacing = 0.0;
            Console.WriteLine("Text with default spacing (0.0)");

            // Сохраните книгу с интервалом по умолчанию
            workbook.Save("TextSpacingDemo3.xlsx");
        }
    }
}
```

### См. также

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


