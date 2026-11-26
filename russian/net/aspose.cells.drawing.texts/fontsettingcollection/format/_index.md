---
title: "FontSettingCollection.Format"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontSettingCollection. Форматировать текст с использованием настроек шрифта"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/format/
---
## FontSettingCollection.Format method

Форматирует текст с помощью настройки шрифта.

```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 | Начальный индекс. |
| длина | Int32 | Длина. |
| шрифт | Шрифт | Шрифт. |
| флаг | StyleFlag | Флаги шрифта. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodFormatWithInt32Int32FontStyleFlagDemo
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
            fontSettingCollection.Text = "Sample Text for Formatting";

            try
            {
                // Создайте стиль и задайте его свойства шрифта
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                style.Font.IsBold = true;
                style.Font.Color = System.Drawing.Color.Red;

                // Создать флаг стиля, чтобы указать, какие свойства шрифта применять
                StyleFlag styleFlag = new StyleFlag();
                styleFlag.FontName = true;
                styleFlag.FontSize = true;
                styleFlag.FontBold = true;
                styleFlag.FontColor = true;

                // Отформатировать символы с индекса 7 по 11 (слово "Text")
                fontSettingCollection.Format(7, 4, style.Font, styleFlag);

                // Сохраните книгу, чтобы показать эффект
                workbook.Save("FontSettingCollectionFormatDemo.xlsx");
                Console.WriteLine("Format method executed successfully. Text 'Text' is now bold, red Arial 14pt.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


