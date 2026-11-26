---
title: "Класс TextOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Texts.TextOptions class. Представляет параметры текста"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/
---
## TextOptions class

Представляет параметры текста.

```csharp
public class TextOptions : Font
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Получает и задает цвет с 32-битным значением ARGB. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [CapsType](../../aspose.cells.drawing.texts/textoptions/capstype/) { get; set; } | Получает и задает тип заглавных букв для текста формы. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Представляет набор символов. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [Color](../../aspose.cells/font/color/) { get; set; } | Получает или задает цвет шрифта. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Получает и задает двойной размер шрифта. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [FarEastName](../../aspose.cells.drawing.texts/textoptions/fareastname/) { get; set; } | Получает и задает название FarEast. |
| [Fill](../../aspose.cells.drawing.texts/textoptions/fill/) { get; } | Представляет формат заливки текста. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Получает или задает значение, указывающее, является ли шрифт полужирным. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Получает или задает значение, указывающее, является ли шрифт курсивным. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [IsNormalizeHeights](../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) { get; set; } | Указывает, будет ли применяться нормализация высоты к последовательности текста. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Получает или задает значение, указывающее, имеет ли шрифт одинарное зачеркивание. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Получает или задает значение, указывающее, является ли шрифт нижним индексом. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Получает или задает значение, указывающее, является ли шрифт верхним индексом. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [Kerning](../../aspose.cells.drawing.texts/textoptions/kerning/) { get; set; } | Указывает минимальный размер шрифта, при котором будет применяться кернинг символов в этой последовательности текста. |
| [LanguageCode](../../aspose.cells.drawing.texts/textoptions/languagecode/) { get; set; } | Получает и задает язык пользовательского интерфейса. |
| [LatinName](../../aspose.cells.drawing.texts/textoptions/latinname/) { get; set; } | Получает и задает латинское название. |
| override [Name](../../aspose.cells.drawing.texts/textoptions/name/) { get; set; } | Получает и задает имя фигуры. |
| [Outline](../../aspose.cells.drawing.texts/textoptions/outline/) { get; } | Представляет формат контура текста. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Получает и задает тип схемы шрифта. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Получает и задает смещение скрипта в процентах. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [Shadow](../../aspose.cells.drawing.texts/textoptions/shadow/) { get; } | Представляет объект [`ShadowEffect`](../../aspose.cells.drawing/shadoweffect/), который задает эффект тени для элемента диаграммы или формы. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Получает или задает размер шрифта. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [Spacing](../../aspose.cells.drawing.texts/textoptions/spacing/) { get; set; } | Указывает интервал между символами в последовательности текста. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Получает тип зачеркивания текста. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Получает и задает цвет темы. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Получает или задает тип подчеркивания шрифта. (Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [UnderlineColor](../../aspose.cells.drawing.texts/textoptions/underlinecolor/) { get; set; } | Получает или задает цвет подчеркивания. |

## Методы

| Имя | Описание |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/)(Font) | Проверяет, равны ли два шрифта.(Унаследовано от [`Font`](../../aspose.cells/font/).) |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Задает имя и схему шрифта.(Унаследовано от [`Font`](../../aspose.cells/font/).) |
| override [ToString](../../aspose.cells/font/tostring/)() | Возвращает строку, представляющую текущий объект Cell.(Унаследовано от [`Font`](../../aspose.cells/font/).) |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте форму на лист со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            
            // Добавьте текст к форме и получите TextOptions
            shape.TextBody.Text = "Sample Text";
            TextOptions textOptions = shape.TextBody[2].TextOptions;
            
            // Установите параметры текста
            textOptions.Fill.SolidFill.Color = System.Drawing.Color.Red;
            textOptions.Fill.SolidFill.Transparency = 0.5;
            
            // Сохраните книгу
            workbook.Save("TextOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../aspose.cells/font/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


