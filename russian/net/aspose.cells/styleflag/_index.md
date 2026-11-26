---
title: "Класс StyleFlag"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.StyleFlag. Представляет флаги, указывающие применённые свойства форматирования"
type: docs
url: /ru/net/aspose.cells/styleflag/
---
## StyleFlag class

Представляет флаги, указывающие применённые свойства форматирования.

```csharp
public class StyleFlag
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [StyleFlag](styleflag/)() | Создаёт объект со всеми флагами, установленными в false. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | Настройка выравнивания будет применена. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | Все свойства будут применены. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | Все настройки границ будут применены. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | Настройки нижней границы будут применены. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | Настройка затенения ячейки будет применена. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | Настройки диагональной нижней границы будут применены. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | Настройки диагональной верхней границы будут применены. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | Настройки шрифта будут применены. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | Настройка полужирного шрифта будет применена. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | Настройка цвета шрифта будет применена. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | Настройка курсивного шрифта будет применена. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | Настройка названия шрифта будет применена. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | Настройка скрипта шрифта будет применена. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | Настройка размера шрифта будет применена. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | Настройка зачеркивания шрифта будет применена. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | Настройка подчеркивания шрифта будет применена. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | Настройка скрытия формулы будет применена. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | Настройка горизонтального выравнивания будет применена. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | Настройка уровня отступа будет применена. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | Настройки левой границы будут применены. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | Настройка блокировки будет применена. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | Настройка числового формата будет применена. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | Настройка скрытия формулы будет применена. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | Настройки правой границы будут применены. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | Настройка вращения будет применена. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | Настройка сжатия до размера будет применена. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | Настройка направления текста будет применена. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | Настройки верхней границы будут применены. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | Настройка вертикального выравнивания будет применена. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | Настройка переноса текста будет применена. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagDemo
    {
        public static void StyleFlagExample()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Создать новый объект стиля
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Создать новый объект StyleFlag
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // Применить стиль к диапазону ячеек
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // Сохраните книгу
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


