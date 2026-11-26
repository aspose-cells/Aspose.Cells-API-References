---
title: "FontSettingCollection.AppendText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontSettingCollection. Добавляет текст"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/appendtext/
---
## FontSettingCollection.AppendText method

Добавляет текст.

```csharp
public void AppendText(string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | Текст. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodAppendTextWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Устанавливает начальный текст
            fontSettingCollection.Text = "Hello, ";

            try
            {
                // Вызвать метод AppendText, чтобы добавить дополнительный текст
                fontSettingCollection.AppendText("World!");

                // Отобразить изменённый текст
                Console.WriteLine("Text after append: " + fontSettingCollection.Text);

                // Сохраните книгу
                workbook.Save("FontSettingCollectionAppendTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AppendText method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


