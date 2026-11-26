---
title: "FontSettingCollection.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSettingCollection. Получает и задаёт текст фигуры"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/text/
---
## FontSettingCollection.Text property

Получает и задает текст фигуры.

```csharp
public string Text { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionPropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            try
            {
                // Устанавливает начальный текст
                fontSettingCollection.Text = "Initial Text Value";
                Console.WriteLine("Initial Text value: " + fontSettingCollection.Text);

                // Изменить текст
                fontSettingCollection.Text = "Modified Text Value";
                Console.WriteLine("Modified Text value: " + fontSettingCollection.Text);

                // Продемонстрировать добавление текста
                fontSettingCollection.AppendText(" (Appended)");
                Console.WriteLine("After AppendText: " + fontSettingCollection.Text);

                // Сохраните книгу
                workbook.Save("FontSettingCollectionTextDemo.xlsx");
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

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


