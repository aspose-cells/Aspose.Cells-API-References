---
title: "FontSettingCollection.InsertText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontSettingCollection. Вставить индекс в указанную позицию"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/inserttext/
---
## FontSettingCollection.InsertText method

Вставляет индекс в позицию.

```csharp
public void InsertText(int index, string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Начальный индекс. |
| текст | String | Текст. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var fontSettingCollection = textBox.TextBody;

            // Устанавливает начальный текст
            fontSettingCollection.Text = "Initial Text";

            try
            {
                // Вызовите метод InsertText, чтобы вставить текст по индексу 7
                fontSettingCollection.InsertText(7, " Inserted");

                // Отобразить изменённый текст
                Console.WriteLine("Text after insertion: " + fontSettingCollection.Text);
                
                // Сохраните книгу
                workbook.Save("FontSettingCollectionInsertTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertText method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


