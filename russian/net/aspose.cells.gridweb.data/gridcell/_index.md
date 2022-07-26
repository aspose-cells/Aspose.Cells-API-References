---
title: GridCell
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет объект ячейки.
type: docs
weight: 150
url: /ru/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Представляет объект ячейки.

```csharp
public class GridCell
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | Получает логическое значение, содержащееся в ячейке. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | Получает номер столбца (начиная с нуля) ячейки. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | Получает значение DateTime, содержащееся в ячейке. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | Получает форматированное строковое значение этой ячейки. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | Получает двойное значение, содержащееся в ячейке. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | Получает значение с плавающей запятой, содержащееся в ячейке. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | Получает или задает формулуCell . |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | Получает и задает строку HTML, содержащую данные и некоторые параметры форматирования в этой ячейке. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | Получает целочисленное значение, содержащееся в ячейке. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что эта ячейка имеет формат ячейки по умолчанию. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | Получает имя ячейки. Например: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | Получает номер строки (начиная с нуля) ячейки. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | Получает строковое значение, содержащееся в ячейке. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | Получает копию стиля ячейки. установить стиль для ячейки. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | возвращает тип значения ячейки, значение можно увидеть GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | Получает значение, содержащееся в этой ячейке. |

## Методы

| Имя | Описание |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только в том случае, если ячейка является ячейкой формулы. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | Копирует данные из исходной ячейки. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | скопируйте стиль и установите стиль для ячейки |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | Создает объект комментария для ячейки. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | Создает объект проверки для ячейки. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | Получить объект комментария к этой ячейке |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | Получает ширину значения в пикселях. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | Проверяет, может ли формула правильно оценить результат. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | Указывает, содержит ли указанная ячейка формулу. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | Помещает логическое значение в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | Помещает значение DateTime в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | Помещает в ячейку двойное значение. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | Помещает значение int в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | Помещает значение объекта в ячейку. То же, что и setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | Помещает строковое значение в ячейку. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | Помещает строковое значение в ячейку и при необходимости преобразует значение в другой тип данных. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Помещает значение в ячейку, при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | Устанавливает значение ячейки со строковым значением и устанавливает формат ячейки по этому значению. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | Удаляет объект комментария ячейки. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | Удаляет объект проверки ячейки. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | Устанавливает границы (сверху, снизу, слева и справа) для ячейки, все границы имеют одинаковый стиль границы. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | задает пользовательский формат, нулевая или пустая строка означает отсутствие пользовательского формата. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | Установить формулу и значение формулы. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | установить формат отображения чисел и дат |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | Возвращает строку, представляющую текущий объект Cell. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### Смотрите также

* пространство имен [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* сборка [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
