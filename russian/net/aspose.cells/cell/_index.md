---
title: Cell
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий одну ячейку книги.
type: docs
weight: 230
url: /ru/net/aspose.cells/cell/
---
## Cell class

Инкапсулирует объект, представляющий одну ячейку книги.

```csharp
public class Cell
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | Получает логическое значение, содержащееся в ячейке. |
| [Column](../../aspose.cells/cell/column) { get; } | Получает номер столбца (с нуля) ячейки. |
| [Comment](../../aspose.cells/cell/comment) { get; } | Получает комментарий этой ячейки. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только в том случае, если ячейка является ячейкой формулы. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | Получает значение DateTime, содержащееся в ячейке. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | Получает отформатированное строковое значение этой ячейки по стилю отображения ячейки. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | Получает двойное значение, содержащееся в ячейке. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | Получает значение с плавающей запятой, содержащееся в ячейке. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | Получает или задает формулу[`Cell`](../cell). |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | Получить формулу ячейки в формате локали. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | Получает и устанавливает строку html, которая содержит данные и некоторые форматы в этой ячейке. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | Получает целочисленное значение, содержащееся в ячейке. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | Указывает, является ли формула ячейки формулой массива. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | Указывает, что формула ячейки и формула массива и это первая ячейка массива. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | Проверяет, является ли значение этой ячейки ошибкой. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | Указывает, содержит ли указанная ячейка формулу. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | Проверяет, является ли ячейка частью объединенного диапазона или нет. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | Указывает, является ли внутреннее значение этой ячейки числовым (int, double и datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | Указывает, является ли формула ячейки частью общей формулы. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что эта ячейка имеет формат ячейки по умолчанию. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | Указывает, является ли эта ячейка частью формулы таблицы. |
| [Name](../../aspose.cells/cell/name) { get; } | Получает имя ячейки. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | Представляет тип категории числового форматирования этой ячейки. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | Получает или задает формулу R1C1 для[`Cell`](../cell). |
| [Row](../../aspose.cells/cell/row) { get; } | Получает номер строки (начиная с нуля) ячейки. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | Получает общий индекс стиля ячейки в пуле стилей. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | Получает строковое значение, содержащееся в ячейке. Если тип этой ячейки — строка, верните само строковое значение. Для других типов ячеек будет возвращено форматированное строковое значение (отформатированное в соответствии с указанным стилем этой ячейки). Отформатированное значение ячейки совпадает с тем, что вы можете получить из Excel при копировании ячейки в виде текста (например, копирование ячейки в текстовый редактор или экспорт в csv). |
| [Type](../../aspose.cells/cell/type) { get; } | Представляет тип значения ячейки. |
| [Value](../../aspose.cells/cell/value) { get; set; } | Получает значение, содержащееся в этой ячейке. |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | Получает родительский рабочий лист. |

## Методы

| Имя | Описание |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | Вычисляет формулу ячейки. |
| [Characters](../../aspose.cells/cell/characters)(int, int) | Возвращает объект символов, представляющий диапазон символов в тексте ячейки. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | Копирует данные из исходной ячейки. |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | Проверяет, ссылается ли этот объект на ту же ячейку с другим объектом ячейки. |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | Проверяет, ссылается ли этот объект на одну и ту же ячейку с другой. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | Получает диапазон массива, если формула ячейки является формулой массива. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | Возвращает все объекты символов , представляющие диапазон символов в тексте ячейки. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | Возвращает все объекты символов , представляющие диапазон символов в тексте ячейки. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | Получить результат условного форматирования. |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | Получить все ячейки, формула которых напрямую ссылается на эту ячейку. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | Получает все ячейки, результат вычислений которых зависит от этой ячейки. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | Получает стиль отображения ячейки. Если на эту ячейку также влияют другие настройки, такие как условное форматирование, объекты списка и т. д., тогда стиль отображения может отличаться от cell.GetStyle(). |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | Получает стиль отображения ячейки. Если ячейка имеет условное форматирование, стиль отображения отличается от стиля cell.GetStyle(). |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | Получает условия формата, применимые к этой ячейке. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | Получить формулу этой ячейки. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | Служит хеш-функцией для определенного типа. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | Получает высоту значения в единицах пикселей. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | Получает строку html, содержащую данные и некоторые форматы в этой ячейке. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | Возвращает объект[`Range`](../range), представляющий объединенный диапазон. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | Получает все ссылки, встречающиеся в формуле этой ячейки. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | Получает все прецеденты (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при ее вычислении. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | Получает строковое значение по определенной отформатированной стратегии. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | Получает стиль ячейки. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | Если для checkBorders установлено значение true, проверьте, повлияют ли границы других ячеек на стиль этой ячейки. |
| [GetTable](../../aspose.cells/cell/gettable)() | Получает таблицу, содержащую эту ячейку. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | Получает проверку, примененную к этой ячейке. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | Получает значение проверки, примененное к этой ячейке. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | Получает ширину значения в пикселях. |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | Указывает, является ли значение строки ячейки форматированным текстом. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | Помещает логическое значение в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | Помещает значение DateTime в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | Помещает в ячейку двойное значение. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | Помещает в ячейку целочисленное значение. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | Помещает значение объекта в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | Помещает строковое значение в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | Помещает строковое значение в ячейку и при необходимости преобразует значение в другой тип данных. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | Помещает значение в ячейку, при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | Удалить формулу массива. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | Устанавливает формулу массива (устаревшая формула массива, введенная с помощью CTRL+SHIFT+ENTER в MS Excel) для диапазона ячеек. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | Задает формулу массива для диапазона ячеек. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Задает формулу массива для диапазона ячеек. |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | Устанавливает расширенный текстовый формат ячейки. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Устанавливает формулу динамического массива и по возможности распространяет формулу на соседние ячейки. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Устанавливает формулу динамического массива и по возможности распространяет формулу на соседние ячейки. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | Установите формулу и значение формулы. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | Установите формулу и значение формулы. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | Устанавливает формулу в диапазон ячеек. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | Устанавливает формулу в диапазон ячеек. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Устанавливает формулу в диапазон ячеек. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | Устанавливает стиль ячейки. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | Применение стиля ячейки. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | Применение стиля ячейки. |
| override [ToString](../../aspose.cells/cell/tostring)() | Возвращает строку, представляющую текущий объект Cell. |

### Примеры

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

  // Поместите строку в ячейку
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
   // Поместите целое число в ячейку
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

   // Поместите двойник в ячейку
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

   // Поместите формулу в ячейку
cell = cells["D1"];
cell.Formula = "=B1 + C1";

   // Поместите комбинированную формулу: «сумма (среднее (b1, c1), b1)» в ячейку по адресу b2
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

   //Установить стиль ячейки
Style style = cell.GetStyle();
   //Установить цвет фона
style.BackgroundColor = Color.Yellow;
  //Установить формат ячейки
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'Поместите строку в ячейку
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
'Поместите целое число в ячейку
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

' Поместите двойник в ячейку
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

   // Поместите формулу в ячейку
cell = cells("D1")
cell.Formula = "=B1 + C1"

' Поместите комбинированную формулу: «сумма (среднее (b1, c1), b1)» в ячейку по адресу b2
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
'Установить стиль ячейки
Dim style as Style = cell.GetStyle()

'Установить цвет фона
style.BackgroundColor = Color.Yellow
'Установить шрифт ячейки
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
