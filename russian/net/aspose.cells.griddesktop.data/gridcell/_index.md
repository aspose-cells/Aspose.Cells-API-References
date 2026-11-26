---
title: "Класс GridCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridDesktop.Data.GridCell. Представляет объект ячейки"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Представляет объект ячейки.

```csharp
public class GridCell
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | Получает логическое значение, содержащееся в ячейке. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | Получает номер столбца (нумерация с нуля) ячейки. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | Получает значение DateTime, содержащееся в ячейке. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | Получает отформатированное строковое значение этой ячейки. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | Получает значение double, содержащееся в ячейке. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | Получает значение float, содержащееся в ячейке. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | Получает или задает формулу ячейки. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | Указывает, имеет ли эта ячейка пользовательские настройки стиля (отличные от стандартных, унаследованных от соответствующей строки, столбца или книги). |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | Получает и задает HTML-строку, содержащую данные и некоторые форматирования в этой ячейке. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | Получает целочисленное значение, содержащееся в ячейке. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что у ячейки используется формат по умолчанию. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | Получает имя ячейки. Например: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | Указывает, защищена ли ячейка. Если значение "true", пользователь не может изменить ячейку через пользовательский интерфейс. Этот атрибут не связан со свойством Style.CellLocked и не будет сохранён в файл при экспорте данных сетки. Значение по умолчанию — "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | Получает номер строки (нумерация с нуля) ячейки. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | Получает строковое значение, содержащееся в ячейке. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | Получает копию стиля ячейки. Устанавливает стиль для ячейки. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | Возвращает тип значения ячейки, значение можно посмотреть в GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | Получает значение, содержащееся в этой ячейке. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | Получает объект листа. |

## Методы

| Имя | Описание |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только к ячейкам с формулой. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | Копирует данные из исходной ячейки. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | Копирует стиль и задает стиль для ячейки |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | Получает шрифт ячейки. При изменении шрифта следует вызвать метод "SetFont", чтобы установить шрифт в ячейку. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | Получает цвет шрифта ячейки. При изменении цвета следует вызвать метод "SetFontColor", чтобы установить цвет шрифта в ячейку. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | Получает стиль ячейки. При изменении стиля следует вызвать метод "SetStyle", чтобы установить стиль в ячейку. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | Получает проверку, применённую к этой ячейке. Если не задано, возвращает null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | Получает ширину значения в пикселях. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | Получает родительский лист. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | Проверяет, может ли формула правильно вычислить результат. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | Представляет, содержит ли указанная ячейка формулу. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | Записывает логическое значение в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | Записывает значение DateTime в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | Записывает значение double в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | Помещает целочисленное значение в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | Помещает объектное значение в ячейку. То же, что setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | Помещает строковое значение в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | Записывает строковое значение в ячейку и при необходимости преобразует его в другой тип данных. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Записывает значение в ячейку; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | Устанавливает значение ячейки строковым значением и задаёт формат ячейки по этому значению. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | Если значение является формулой, этот метод устанавливает значение ячейки как FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | Устанавливает пользовательский формат, null или пустая строка означают отсутствие пользовательского формата. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | Устанавливает шрифт в ячейку. Чтобы улучшить производительность, реализуйте метод "SetFont", а не свойство "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | Устанавливает цвет шрифта в ячейке. Чтобы улучшить производительность, реализуйте метод "SetFontColor", а не свойство "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | Устанавливает формулу и значение формулы. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | устанавливает формат отображения чисел и дат |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | Устанавливает стиль в ячейку. Чтобы улучшить производительность, реализуйте метод "SetStyle", а не свойство "Style". |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | Возвращает строку, представляющую текущий объект Cell. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |

### См. также

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


