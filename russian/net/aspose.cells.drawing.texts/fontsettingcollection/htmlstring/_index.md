---
title: "FontSettingCollection.HtmlString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSettingCollection. Получает и задает HTML-строку, содержащую данные и некоторые форматы в таком виде"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/htmlstring/
---
## FontSettingCollection.HtmlString property

Получает и задает HTML-строку, содержащую данные и некоторые форматы в этой форме.

```csharp
public string HtmlString { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 300, 100);
            var fontSettingCollection = textBox.TextBody;

            // Установить начальный текст с HTML-форматированием
            string initialHtml = "<b>Bold Text</b> and <i>Italic Text</i>";
            fontSettingCollection.HtmlString = initialHtml;

            // Отобразить текущую HTML-строку
            Console.WriteLine("Initial HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text: " + fontSettingCollection.Text);

            // Изменить HTML-строку, чтобы добавить больше форматирования
            string modifiedHtml = "<font color='red'>Red Text</font> and <u>Underlined Text</u>";
            fontSettingCollection.HtmlString = modifiedHtml;

            // Отобразить изменённые значения
            Console.WriteLine("\nModified HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text after modification: " + fontSettingCollection.Text);

            // Добавить ячейку с текстом, отформатированным в HTML
            var cell = worksheet.Cells["A1"];
            cell.HtmlString = "<b>Cell HTML</b> <i>Formatted</i> <font color='blue'>Text</font>";

            // Сохранить книгу, чтобы показать как форматирование текстового поля, так и ячейки в HTML
            workbook.Save("FontSettingCollectionHtmlStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


