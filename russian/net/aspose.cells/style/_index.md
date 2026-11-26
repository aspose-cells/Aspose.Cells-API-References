---
title: "Класс Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Style класс. Представляет стиль отображения Excel‑документов, таких как цвет шрифта, выравнивание, границы и т.д. Объект Style содержит все атрибуты стиля, такие как шрифт, числовой формат, выравнивание и т.п., в виде свойств"
type: docs
url: /ru/net/aspose.cells/style/
---
## Style class

Представляет стиль отображения Excel‑документа, такой как шрифт, цвет, выравнивание, граница и т.д. Объект Style содержит все атрибуты стиля (шрифт, числовой формат, выравнивание и т.п.) в виде свойств.

```csharp
public class Style
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Style](style/)() | (**Obsolete.**) Инициализирует новый экземпляр класса `Style`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor/) { get; set; } | Получает и задает цвет фона в виде 32‑битного значения ARGB. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor/) { get; set; } | Получает или задает цвет фона стиля. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor/) { get; set; } | Получает и задает цвет темы фона. |
| [Borders](../../aspose.cells/style/borders/) { get; } | Получает [`BorderCollection`](../bordercollection/) стиля. |
| [BottomBorder](../../aspose.cells/style/bottomborder/) { get; } | Получает нижнюю границу. |
| [CultureCustom](../../aspose.cells/style/culturecustom/) { get; set; } | Получает и задает зависящую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному числу. |
| [Custom](../../aspose.cells/style/custom/) { get; set; } | Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не задан (например, числовой формат встроенный), будет возвращена пустая строка "". |
| [Font](../../aspose.cells/style/font/) { get; } | Получает объект [`Font`](./font/). |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor/) { get; set; } | Получает и задает цвет переднего плана в виде 32‑битного значения ARGB. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor/) { get; set; } | Получает или задает цвет переднего плана стиля. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor/) { get; set; } | Получает и задает цвет переднего плана темы. |
| [HasBorders](../../aspose.cells/style/hasborders/) { get; } | Проверяет, установлены ли границы для стиля. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment/) { get; set; } | Получает или задает тип горизонтального выравнивания текста в ячейке. |
| [IndentLevel](../../aspose.cells/style/indentlevel/) { get; set; } | Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom/) { get; } | Получает независимую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному числу. |
| [IsAlignmentApplied](../../aspose.cells/style/isalignmentapplied/) { get; set; } | Указывает, следует ли применять форматирование выравнивания. |
| [IsBorderApplied](../../aspose.cells/style/isborderapplied/) { get; set; } | Указывает, следует ли применять форматирование границы. |
| [IsCheckBox](../../aspose.cells/style/ischeckbox/) { get; set; } | Указывает, является ли это стилем флажка. |
| [IsDateTime](../../aspose.cells/style/isdatetime/) { get; } | Указывает, является ли числовой формат датой. |
| [IsFillApplied](../../aspose.cells/style/isfillapplied/) { get; set; } | Указывает, следует ли применять форматирование заливки. |
| [IsFontApplied](../../aspose.cells/style/isfontapplied/) { get; set; } | Указывает, следует ли применять форматирование шрифта. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden/) { get; set; } | Представляет, будет ли формула скрыта, когда лист защищён. |
| [IsGradient](../../aspose.cells/style/isgradient/) { get; set; } | Указывает, является ли затенение ячейки градиентным шаблоном. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed/) { get; set; } | Указывает, следует ли использовать выравнивание по ширине или распределённое выравнивание ячеек в последней строке текста. |
| [IsLocked](../../aspose.cells/style/islocked/) { get; set; } | Получает или задает значение, указывающее, можно ли изменять ячейку. |
| [IsNumberFormatApplied](../../aspose.cells/style/isnumberformatapplied/) { get; set; } | Указывает, следует ли применять числовое форматирование. |
| [IsPercent](../../aspose.cells/style/ispercent/) { get; } | Указывает, является ли числовой формат процентным. |
| [IsProtectionApplied](../../aspose.cells/style/isprotectionapplied/) { get; set; } | Указывает, следует ли применять форматирование защиты. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped/) { get; set; } | Получает или задает значение, указывающее, переносится ли текст внутри ячейки. |
| [LeftBorder](../../aspose.cells/style/leftborder/) { get; } | Получает левую границу. |
| [Name](../../aspose.cells/style/name/) { get; set; } | Получает или задает имя стиля. |
| [Number](../../aspose.cells/style/number/) { get; set; } | Получает или задает формат отображения чисел и дат. Шаблоны форматирования различаются для разных регионов. |
| [ParentStyle](../../aspose.cells/style/parentstyle/) { get; } | Получает родительский стиль этого стиля. |
| [Pattern](../../aspose.cells/style/pattern/) { get; set; } | Получает или задает тип фонового узора ячейки. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix/) { get; set; } | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [RightBorder](../../aspose.cells/style/rightborder/) { get; } | Получает правую границу. |
| [RotationAngle](../../aspose.cells/style/rotationangle/) { get; set; } | Представляет угол поворота текста. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit/) { get; set; } | Представляет, автоматически ли текст уменьшается, чтобы поместиться в доступную ширину столбца. |
| [TextDirection](../../aspose.cells/style/textdirection/) { get; set; } | Представляет порядок чтения текста. |
| [TopBorder](../../aspose.cells/style/topborder/) { get; } | Получает верхнюю границу. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment/) { get; set; } | Получает или задает тип вертикального выравнивания текста в ячейке. |

## Методы

| Имя | Описание |
| --- | --- |
| [Copy](../../aspose.cells/style/copy/)(Style) | Копирует данные из другого объекта стиля |
| override [Equals](../../aspose.cells/style/equals/)(object) | Определяет, равны ли два экземпляра Style. |
| override [GetHashCode](../../aspose.cells/style/gethashcode/)() | Служит хеш-функцией для объекта Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient/)(out Color, out Color, out GradientStyleType, out int) | (**Obsolete.**) Получить настройку двухцветного градиента. |
| [GetTwoColorGradientSetting](../../aspose.cells/style/gettwocolorgradientsetting/)() | Получить настройку двухцветного градиента. |
| [IsModified](../../aspose.cells/style/ismodified/)(StyleModifyFlag) | Проверяет, были ли изменены указанные свойства стиля. Используется для стиля ConditionalFormattings, чтобы проверить, следует ли использовать указанные свойства этого стиля при применении ConditionalFormattings к ячейке. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder)(BorderType, CellBorderType, CellsColor) | Устанавливает границы стиля. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder_1)(BorderType, CellBorderType, Color) | Устанавливает границы стиля. |
| [SetCustom](../../aspose.cells/style/setcustom/)(string, bool) | Устанавливает пользовательскую строку формата числа для ячейки. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Установить контурные границы |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Установить контурные границы |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor/)(BackgroundType, Color, Color) | Устанавливает цвет фона. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient/)(Color, Color, GradientStyleType, int) | Устанавливает указанную заливку в виде двухцветного градиента. |
| [ToJson](../../aspose.cells/style/tojson/)() | Преобразовать `Style` в данные структуры JSON. |
| [Update](../../aspose.cells/style/update/)() | Применить именованный стиль к стилям ячеек, использующих этот именованный стиль. Это работает как нажатие кнопки "ok" после завершения изменения стиля. Применяется только к именованному стилю. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleDemo
    {
        public static void StyleExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к ячейке листа
            Cell cell = worksheet.Cells["A1"];
            
            // Получить стиль ячейки
            Style style = cell.GetStyle();
            
            // Установить различные свойства стиля
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // Установить стиль для ячейки
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("StyleExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


