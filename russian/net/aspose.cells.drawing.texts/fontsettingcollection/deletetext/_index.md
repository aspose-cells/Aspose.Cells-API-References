---
title: "FontSettingCollection.DeleteText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontSettingCollection. Удалить некоторые символы"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/deletetext/
---
## FontSettingCollection.DeleteText method

Удаляет некоторые символы.

```csharp
public void DeleteText(int index, int count)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Начальный индекс. |
| количество | Int32 | Количество символов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodDeleteTextWithInt32Int32Demo
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
            fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";

            try
            {
                // Отобразить исходный текст
                Console.WriteLine("Original text: " + fontSettingCollection.Text);

                // Вызовите метод DeleteText, чтобы удалить 7 символов, начиная с индекса 5
                fontSettingCollection.DeleteText(5, 7);

                // Отобразить изменённый текст
                Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);

                // Сохраните книгу
                workbook.Save("FontSettingCollectionDeleteTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteText method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


