---
title: GridCell
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет объект ячейки.
type: docs
weight: 370
url: /ru/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Представляет объект ячейки.

```csharp
public class GridCell
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue) { get; } | Получает логическое значение, содержащееся в ячейке. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column) { get; } | Получает номер столбца (начиная с нуля) ячейки. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue) { get; } | Получает значение DateTime, содержащееся в ячейке. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue) { get; } | Получает форматированное строковое значение этой ячейки. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue) { get; } | Получает двойное значение, содержащееся в ячейке. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue) { get; } | Получает значение с плавающей запятой, содержащееся в ячейке. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula) { get; set; } | Получает или задает формулуCell . |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring) { get; set; } | Получает и задает строку HTML, содержащую данные и некоторые параметры форматирования в этой ячейке. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue) { get; } | Получает целочисленное значение, содержащееся в ячейке. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset) { get; } | Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что эта ячейка имеет формат ячейки по умолчанию. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name) { get; } | Получает имя ячейки. Например: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected) { get; set; } | Указывает, защищена ли ячейка. Если значение равно "true", пользователь не может изменять ячейку через пользовательский интерфейс. Этот атрибут не имеет ничего общего со свойством Style.CellLocked и не будет сохранен в файл при данные сетки экспортированы. Значение по умолчанию "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row) { get; } | Получает номер строки (начиная с нуля) ячейки. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue) { get; } | Получает строковое значение, содержащееся в ячейке. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style) { get; set; } | Получает копию стиля ячейки. установить стиль для ячейки. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type) { get; } | возвращает тип значения ячейки, значение можно увидеть GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value) { get; set; } | Получает значение, содержащееся в этой ячейке. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet) { get; } | Получает объект рабочего листа. |

## Методы

| Имя | Описание |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink)() | Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только в том случае, если ячейка является ячейкой формулы. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy)(GridCell) | Копирует данные из исходной ячейки. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle)(Style) | скопируйте стиль и установите стиль для ячейки |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont)() | Получает шрифт ячейки. При изменении шрифта вы должны вызвать метод "SetFont", для установки шрифта ячейки. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor)() | Получает цвет шрифта ячейки. При изменении цвета следует вызвать метод "SetFontColor", для установки цвета шрифта ячейки. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle)() | Получает стиль ячейки. При изменении стиля следует вызвать метод "SetStyle", для установки стиля ячейки. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation)() | Получает проверку, примененную к этой ячейке. Если не задано, возвращает значение null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue)() | Получает ширину значения в пикселях. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet)() | Получает родительский рабочий лист. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue)() | Проверяет, может ли формула правильно оценить результат. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula)() | Указывает, содержит ли указанная ячейка формулу. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue)(bool) | Помещает логическое значение в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_3)(DateTime) | Помещает значение DateTime в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_1)(double) | Помещает в ячейку двойное значение. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_2)(int) | Помещает значение int в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_4)(object) | Помещает значение объекта в ячейку. То же, что и setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_5)(string) | Помещает строковое значение в ячейку. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_6)(string, bool) | Помещает строковое значение в ячейку и при необходимости преобразует значение в другой тип данных. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Помещает значение в ячейку, при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue)(string) | Устанавливает значение ячейки со строковым значением и устанавливает формат ячейки по этому значению. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue)(object) | Если значение является формулой, этот метод устанавливает значение ячейки как FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom)(string) | задает пользовательский формат, нулевая или пустая строка означает отсутствие пользовательского формата. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont)(Font) | Устанавливает шрифт в ячейку. Для повышения производительности реализуйте метод "SetFont", не реализуйте свойство "Шрифт". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor)(Color) | Устанавливает цвет шрифта для ячейки. Для повышения производительности реализуйте метод "SetFontColor", не реализуйте свойство "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula)(string, object) | Установить формулу и значение формулы. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype)(int) | установить формат отображения чисел и дат |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle)(Style) | Устанавливает стиль для ячейки. Для повышения производительности реализуйте метод "SetStyle", не реализуйте свойство "Стиль". |
| [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring#tostring)() | Возвращает строку, представляющую текущий объект Cell. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality) |  |

### Смотрите также

* пространство имен [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* сборка [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
