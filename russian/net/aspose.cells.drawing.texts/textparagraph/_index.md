---
title: "Класс TextParagraph"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Texts.TextParagraph. Представляет настройки текстового абзаца"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/
---
## TextParagraph class

Представляет настройку абзаца текста.

```csharp
public class TextParagraph : FontSetting
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | Получает и задает тип горизонтального выравнивания текста абзаца. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | Получает маркер. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | Получает все текстовые фрагменты в этом абзаце. Если этот абзац пуст, возвращает сам абзац. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | Получает и задает размер по умолчанию символа табуляции в этом абзаце. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | Указывает размер отступа, который будет применён к первой строке текста в абзаце. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Возвращает шрифт этого объекта (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | Определяет, где вертикально на строке текста располагаются реальные слова. Это относится к вертикальному размещению символов относительно базовых линий. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | Указывает, можно ли разрывать слово восточноазиатского происхождения и переносить его на следующую строку без добавления дефиса. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | Указывает, следует ли принудительно размещать пунктуацию в строке текста или переносить её на другую строку. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | Указывает, можно ли разрывать латинское слово и переносить его на следующую строку без добавления дефиса. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | Указывает левый отступ абзаца. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Получает длину символов (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | Получает и задает количество вертикального пустого пространства, которое будет использоваться в абзаце. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | Получает и задает количество вертикального пустого пространства, которое будет использоваться в абзаце. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | Указывает правый отступ абзаца. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | Получает и задает количество вертикального пустого пространства, которое будет присутствовать после абзаца. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | Получает и задает количество вертикального пустого пространства, которое будет присутствовать после абзаца. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | Получает и задает количество вертикального пустого пространства, которое будет присутствовать перед абзацем. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | Получает и задает количество вертикального пустого пространства, которое будет присутствовать перед абзацем. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Получает начальный индекс символов (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | Получает список табуляций. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Возвращает параметры текста (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | Получает тип текстового узла. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Устанавливает предустановленный стиль WordArt.(Наследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
            
            // Установить текстовое содержимое с несколькими абзацами
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Получать доступ и изменять текстовые абзацы
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                // Установить свойства абзаца
                paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
                paragraph.LineSpace = 20;
                paragraph.AlignmentType = TextAlignmentType.Center;
            }

            // Сохраните книгу
            workbook.Save("TextParagraphDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


