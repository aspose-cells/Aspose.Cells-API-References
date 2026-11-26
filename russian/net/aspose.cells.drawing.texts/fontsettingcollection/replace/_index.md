---
title: "FontSettingCollection.Replace"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontSettingCollection. Заменить текст"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

Заменяет текст.

```csharp
public void Replace(int index, int count, string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Начальный индекс. |
| количество | Int32 | Количество символов. |
| текст | String | Текст. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodReplaceWithInt32Int32StringDemo
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
            fontSettingCollection.Text = "Original text to be modified";

            try
            {
                // Вызовите метод Replace, чтобы заменить 8 символов, начиная с индекса 9, новым текстом
                fontSettingCollection.Replace(9, 8, "replaced");

                // Отобразить изменённый текст
                Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);

                // Сохраните книгу
                workbook.Save("FontSettingCollectionReplaceDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

Заменяет текст.

```csharp
public void Replace(string oldValue, string newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| oldValue | String | Старый текст. |
| newValue | String | Новый текст. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте форму и задайте текст
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample text ３４ for replacement";
            
            // Заменить текст в форме
            shape.TextBody.Replace("３４", "ABC");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


