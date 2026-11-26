---
title: "Класс FontSettingCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Texts.FontSettingCollection class. Представляет список FontSetting"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/
---
## FontSettingCollection class

Представляет список [`FontSetting`](../../aspose.cells/fontsetting/).

```csharp
public class FontSettingCollection : CollectionBase<FontSetting>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [HtmlString](../../aspose.cells.drawing.texts/fontsettingcollection/htmlstring/) { get; set; } | Получает и задает HTML-строку, содержащую данные и некоторые форматы в этой форме. |
| [Item](../../aspose.cells.drawing.texts/fontsettingcollection/item/) { get; } | Получает [`FontSetting`](../../aspose.cells/fontsetting/) по индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Text](../../aspose.cells.drawing.texts/fontsettingcollection/text/) { get; set; } | Получает и задает текст фигуры. |
| [TextAlignment](../../aspose.cells.drawing.texts/fontsettingcollection/textalignment/) { get; } | Представляет настройку выравнивания тела текста. |
| [TextParagraphs](../../aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/) { get; } | Получает все абзацы. |

## Методы

| Имя | Описание |
| --- | --- |
| [AppendText](../../aspose.cells.drawing.texts/fontsettingcollection/appendtext/)(string) | Добавляет текст. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [Clear](../../aspose.cells.drawing.texts/fontsettingcollection/clear/#clear)() | Очищает все настройки. (2 метода) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FontSetting) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FontSetting[], int, int) |  |
| [DeleteText](../../aspose.cells.drawing.texts/fontsettingcollection/deletetext/)(int, int) | Удаляет некоторые символы. |
| override [Equals](../../aspose.cells.drawing.texts/fontsettingcollection/equals/)(object) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FontSetting&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FontSetting&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FontSetting&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FontSetting&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FontSetting&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FontSetting&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FontSetting&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FontSetting&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FontSetting&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FontSetting&gt;) |  |
| [Format](../../aspose.cells.drawing.texts/fontsettingcollection/format/)(int, int, Font, StyleFlag) | Форматирует текст с помощью настройки шрифта. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| override [GetHashCode](../../aspose.cells.drawing.texts/fontsettingcollection/gethashcode/)() |  |
| [GetParagraphEnumerator](../../aspose.cells.drawing.texts/fontsettingcollection/getparagraphenumerator/)() | Получает перечислитель абзацев. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int, int) |  |
| [InsertText](../../aspose.cells.drawing.texts/fontsettingcollection/inserttext/)(int, string) | Вставляет индекс в позицию. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace_1)(string, string) | Заменяет текст. |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace)(int, int, string) | Заменяет текст. |
| [SetWordArtStyle](../../aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/)(PresetWordArtStyle) | Устанавливает предустановленный стиль WordArt. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassFontSettingCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettings = textBox.TextBody;

            // Устанавливает начальный текст
            fontSettings.Text = "Initial Text";
            Console.WriteLine("Initial Text: " + fontSettings.Text);

            // Добавить текст
            fontSettings.AppendText("\nAppended Text");
            Console.WriteLine("After Append: " + fontSettings.Text);

            // Вставить текст
            fontSettings.InsertText(7, "Inserted ");
            Console.WriteLine("After Insert: " + fontSettings.Text);

            // Заменить текст по позиции
            fontSettings.Replace(0, 7, "Modified");
            Console.WriteLine("After Position Replace: " + fontSettings.Text);

            // Заменить текст по значению
            fontSettings.Replace("Appended", "Replaced");
            Console.WriteLine("After Value Replace: " + fontSettings.Text);

            // Форматировать текст
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.Color = System.Drawing.Color.Red;

            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontColor = true;

            fontSettings.Format(0, 8, style.Font, flag);

            // Продемонстрировать HTML-строку
            fontSettings.HtmlString = "<b>Bold HTML</b> <i>Italic HTML</i>";
            Console.WriteLine("HTML String: " + fontSettings.HtmlString);

            // Получить доступ к абзацам текста
            var paragraphs = fontSettings.TextParagraphs;
            Console.WriteLine("Paragraph Count: " + paragraphs.Count);

            // Установить стиль WordArt
            fontSettings.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);

            // Сохраните книгу
            workbook.Save("TextsClassFontSettingCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


