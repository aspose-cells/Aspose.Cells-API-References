---
title: "FontSetting.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSetting. Получает тип узла текста"
type: docs
url: /ru/net/aspose.cells/fontsetting/type/
---
## FontSetting.Type property

Получает тип текстового узла.

```csharp
public virtual TextNodeType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;  // Added this using directive
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текст в ячейку
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Получить настройки шрифта для символов ячейки
            FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);

            // Отобразить текущее значение Type
            Console.WriteLine("Current Type value: " + fontSetting.Type);

            // Продемонстрировать, как Type влияет на обработку текста
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("The text is a standard text run.");
            }
            else if (fontSetting.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("The text is part of a paragraph.");
            }
            else if (fontSetting.Type == TextNodeType.Equation)
            {
                Console.WriteLine("The text represents an equation.");
            }

            // Применить различное форматирование в зависимости от Type
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                fontSetting.Font.Color = System.Drawing.Color.Red;
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
            }

            // Сохранить результат
            workbook.Save("FontSettingTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


