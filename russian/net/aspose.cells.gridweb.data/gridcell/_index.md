---
title: "Класс GridCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridWeb.Data.GridCell класс. Представляет объект ячейки"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Представляет объект ячейки.

```csharp
public class GridCell
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue/) { get; } | Получает логическое значение, содержащееся в ячейке. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column/) { get; } | Получает номер столбца (нумерация с нуля) ячейки. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue/) { get; } | Получает значение DateTime, содержащееся в ячейке. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue/) { get; } | Получает отформатированное строковое значение этой ячейки. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue/) { get; } | Получает значение double, содержащееся в ячейке. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue/) { get; } | Получает значение float, содержащееся в ячейке. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula/) { get; set; } | Получает или задаёт формулу `GridCell`. |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring/) { get; set; } | Получает и задает HTML-строку, содержащую данные и некоторые форматирования в этой ячейке. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue/) { get; } | Получает целочисленное значение, содержащееся в ячейке. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset/) { get; } | Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что у ячейки используется формат по умолчанию. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name/) { get; } | Получает имя ячейки. Например: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row/) { get; } | Получает номер строки (нумерация с нуля) ячейки. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue/) { get; } | Получает строковое значение, содержащееся в ячейке. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style/) { get; set; } | Получает копию стиля ячейки. Устанавливает стиль для ячейки. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type/) { get; } | Возвращает тип значения ячейки, значение можно посмотреть в GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value/) { get; set; } | Получает значение, содержащееся в этой ячейке. |

## Методы

| Имя | Описание |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink/)() | Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только к ячейкам с формулой. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy/)(GridCell) | Копирует данные из исходной ячейки. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle/)(GridTableItemStyle) | Копирует стиль и задает стиль для ячейки |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment/)(string, string, bool) | Создаёт объект комментария для ячейки. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation/)(GridValidationType, bool) | Создаёт объект проверки для ячейки. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals/)(object) | Проверяет, ссылается ли этот объект на ту же ячейку, что и другой объект ячейки. |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment/)() | Получить объект комментария в этой ячейке |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode/)() | Служит хеш-функцией для определённого типа. |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue/)() | Получает ширину значения в пикселях. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue/)() | Проверяет, может ли формула правильно вычислить результат. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula/)() | Представляет, содержит ли указанная ячейка формулу. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue)(bool) | Записывает логическое значение в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_3)(DateTime) | Записывает значение DateTime в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_1)(double) | Записывает значение double в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_2)(int) | Помещает целочисленное значение в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_4)(object) | Помещает объектное значение в ячейку. То же, что setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_5)(string) | Помещает строковое значение в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_6)(string, bool) | Записывает строковое значение в ячейку и при необходимости преобразует его в другой тип данных. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Записывает значение в ячейку; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue/)(string) | Устанавливает значение ячейки строковым значением и задаёт формат ячейки по этому значению. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment/)() | Удаляет объект комментария ячейки. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation/)() | Удаляет объект проверки ячейки. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder/)(WebBorderStyle) | Устанавливает границы (верх, низ, слева и справа) для ячейки, все границы имеют одинаковый стиль. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom/)(string) | Устанавливает пользовательский формат, null или пустая строка означают отсутствие пользовательского формата. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula/)(string, object) | Устанавливает формулу и значение формулы. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype/)(int) | устанавливает формат отображения чисел и дат |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring/#tostring)() | Возвращает строку, представляющую текущий объект Cell. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality/) |  |

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


