---
title: "FontSettingCollection.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontSettingCollection."
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/equals/
---
## FontSettingCollection.Equals method

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Установить некоторый текст
            fontSettingCollection.Text = "Sample Text";

            try
            {
                // Создать другой FontSettingCollection для сравнения
                var anotherTextBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var anotherFontSettingCollection = anotherTextBox.TextBody;
                anotherFontSettingCollection.Text = "Sample Text";

                // Вызвать метод Equals для сравнения двух коллекций
                bool areEqual = fontSettingCollection.Equals(anotherFontSettingCollection);

                // Отобразить результат
                Console.WriteLine($"Are the FontSettingCollections equal? {areEqual}");

                // Сохраните книгу
                workbook.Save("FontSettingCollectionEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Equals: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


