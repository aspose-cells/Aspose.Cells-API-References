---
title: "TextParagraph.Children"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает все текстовые фрагменты в этом абзаце. Если абзац пуст, возвращает сам абзац"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/children/
---
## TextParagraph.Children property

Получает все текстовые фрагменты в этом абзаце. Если этот абзац пуст, возвращает сам абзац.

```csharp
public FontSetting[] Children { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyChildrenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            textBox.Text = "First line\nSecond line\nThird line";

            // Получить коллекцию текстовых абзацев
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Отобразить количество дочерних элементов (текстовых фрагментов) в абзаце
            Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);

            // Изменить настройки шрифта каждого дочернего элемента (текстового фрагмента)
            foreach (FontSetting child in textParagraph.Children)
            {
                child.Font.Size = 12;
                child.Font.Color = System.Drawing.Color.Blue;
                child.Font.IsBold = true;
            }

            // Добавить еще одну строку с другим форматированием
            textBox.Text += "\nFourth line";
            fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
            textParagraph = (TextParagraph)fontSetting;

            // Отобразить обновленное количество дочерних элементов
            Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);

            // Сохраните книгу
            workbook.Save("TextParagraphChildrenDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


