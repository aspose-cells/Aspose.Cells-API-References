---
title: Style
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет стиль отображения документа Excel например шрифт цвет выравнивание границу и т. д. Объект Style содержит все атрибуты стиля шрифт числовой формат выравнивание и т. д. в виде свойств.
type: docs
weight: 5750
url: /ru/net/aspose.cells/style/
---
## Style class

Представляет стиль отображения документа Excel, например шрифт, цвет, выравнивание, границу и т. д. Объект Style содержит все атрибуты стиля (шрифт, числовой формат, выравнивание и т. д.) в виде свойств.

```csharp
public class Style
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | Получает и задает цвет фона с 32-битным значением ARGB. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | Получает или задает цвет фона стиля. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | Получает и устанавливает цвет фона темы. |
| [Borders](../../aspose.cells/style/borders) { get; } | Получает[`BorderCollection`](../bordercollection) стиля. |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | Получает и задает строку шаблона, зависящую от языка и региональных параметров, для числового формата. Если для этого объекта не задан числовой формат, будет возвращено значение null. Если числовой формат является встроенным, будет возвращена строка шаблона, соответствующая встроенному номеру. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не задан (например, числовой формат является встроенным), будет возвращено "" . |
| [Font](../../aspose.cells/style/font) { get; } | Получает[`Font`](./font) объект. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | Получает и задает цвет переднего плана с 32-битным значением ARGB. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | Получает или задает цвет переднего плана стиля. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | Получает и устанавливает цвет темы переднего плана. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | Проверяет, установлены ли границы для стиля. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | Получает или задает тип горизонтального выравнивания текста в ячейке. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | Получает независимую от региональных параметров строку шаблона для числового формата. Если для этого объекта не задан числовой формат, будет возвращено значение NULL. Если числовой формат является встроенным, будет возвращена строка шаблона, соответствующая встроенному номеру. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | Указывает, является ли числовой формат форматом даты. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | Указывает, будет ли скрыта формула, когда рабочий лист защищен. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | Указывает, является ли затенение ячеек градиентным узором. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | Указывает, следует ли использовать выравнивание ячеек по ширине или распределенное выравнивание в последней строке текста. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | Получает или задает значение, указывающее, можно ли изменить ячейку или нет. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | Указывает, является ли числовой формат процентным форматом. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | Получает или задает значение, указывающее, переносится ли текст в ячейке. |
| [Name](../../aspose.cells/style/name) { get; set; } | Получает или задает имя стиля. |
| [Number](../../aspose.cells/style/number) { get; set; } | Получает или задает формат отображения чисел и дат. Шаблоны форматирования различаются для разных регионов. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | Получает родительский стиль этого стиля. |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | Получает или задает тип шаблона фона ячейки. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | Представляет угол поворота текста. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | Указывает, сжимается ли текст автоматически, чтобы соответствовать доступной ширине столбца. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | Представляет порядок чтения текста. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | Получает или задает тип вертикального выравнивания текста в ячейке. |

## Методы

| Имя | Описание |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | Копирует данные из другого объекта стиля |
| override [Equals](../../aspose.cells/style/equals)(object) | Определяет, равны ли два экземпляра стиля. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | Служит хэш-функцией для объекта Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | Получить настройку двухцветного градиента. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | Проверяет, были ли изменены указанные свойства стиля. Используется для стиля ConditionalFormattings, чтобы проверить, следует ли использовать указанные свойства этого стиля при применении ConditionalFormattings к ячейке. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | Устанавливает границы стиля. |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | Устанавливает строку пользовательского числового формата ячейки. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | Устанавливает цвет фона. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | Устанавливает для указанной заливки двухцветный градиент. |
| [Update](../../aspose.cells/style/update)() | Применить именованный стиль к стилям ячеек, которые используют этот именованный стиль. Работает аналогично нажатию кнопки «ОК» после завершения изменения стиля. Применяется только к именованному стилю. |

### Примеры

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
