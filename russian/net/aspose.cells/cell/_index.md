---
title: "Класс Cell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Cell. Инкапсулирует объект, представляющий отдельную ячейку книги."
type: docs
url: /ru/net/aspose.cells/cell/
---
## Cell class

Инкапсулирует объект, представляющий отдельную ячейку Workbook.

```csharp
public class Cell
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | Получает логическое значение, содержащееся в ячейке. |
| [Column](../../aspose.cells/cell/column/) { get; } | Получает номер столбца (нумерация с нуля) ячейки. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | Получает комментарий этой ячейки. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только к ячейкам с формулой. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | Получает значение DateTime, содержащееся в ячейке. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | Получает отформатированное строковое значение этой ячейки в соответствии со стилем отображения ячейки. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | Получает значение double, содержащееся в ячейке. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | Получает и задает встроенное изображение в ячейке. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | Получает значение float, содержащееся в ячейке. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | Получает или задает формулу `Cell`. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | Получить локализованную отформатированную формулу ячейки. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | Проверяет, есть ли пользовательская функция (неподдерживаемая функция) в формуле этой ячейки. |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | Указывает, имеет ли эта ячейка пользовательские настройки стиля (отличные от стандартных, унаследованных от соответствующей строки, столбца или книги). |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | Получает и задает HTML-строку, содержащую данные и некоторые форматы в этой ячейке. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | Получает целочисленное значение, содержащееся в ячейке. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | Указывает, является ли формула ячейки массивной формулой. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | Указывает, что формула ячейки является массивной формулой и эта ячейка является первой ячейкой массива. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | Указывает, можно ли установить эту ячейку как флажок. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | Указывает, является ли формула ячейки динамической массивной формулой (true) или устаревшей массивной формулой (false). |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | Проверяет, является ли значение этой ячейки ошибкой. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | Представляет, содержит ли указанная ячейка формулу. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) Указывает, является ли формула ячейки массивной формулой. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) Указывает, является ли эта ячейка частью формулы таблицы. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | Проверяет, является ли ячейка частью объединённого диапазона. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | Указывает, является ли значение этой ячейки числовым (int, double и datetime). |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | Указывает, является ли формула ячейки частью общей формулы. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | Указывает, установлен ли стиль ячейки. Если возвращается false, это означает, что у ячейки используется формат по умолчанию. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | Указывает, является ли эта ячейка частью формулы таблицы. |
| [Name](../../aspose.cells/cell/name/) { get; } | Получает имя ячейки. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | Представляет тип категории числового форматирования этой ячейки. |
| [Picture](../../aspose.cells/cell/picture/) { get; } | Получает экземпляр [`Picture`](../../aspose.cells.drawing/picture/), представляющий встроенное изображение в этой ячейке, или null, если для этой ячейки нет встроенного изображения. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | Получает или задаёт R1C1‑формулу `Cell`. |
| [Row](../../aspose.cells/cell/row/) { get; } | Получает номер строки (нумерация с нуля) ячейки. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | Получает индекс общего стиля ячейки в пуле стилей. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | Получает строковое значение, содержащееся в ячейке. Если тип этой ячейки — строка, возвращается само строковое значение. Для остальных типов ячеек будет возвращено отформатированное строковое значение (отформатированное с использованием указанного стиля этой ячейки). Отформатированное значение ячейки совпадает с тем, что можно получить из Excel при копировании ячейки как текста (например, при копировании ячейки в текстовый редактор или экспорте в CSV). |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) Получает значение ячейки как строку без какого-либо форматирования. |
| [Type](../../aspose.cells/cell/type/) { get; } | Представляет тип значения ячейки. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | Получает/устанавливает значение, содержащееся в этой ячейке. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | Получает родительский лист. |

## Методы

| Имя | Описание |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | Вычисляет формулу ячейки. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | Возвращает объект Characters, представляющий диапазон символов внутри текста ячейки. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | Копирует данные из исходной ячейки. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | Проверяет, ссылается ли этот объект на ту же ячейку, что и другой объект ячейки. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | Проверяет, ссылается ли этот объект на ту же ячейку, что и другой. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | Получает диапазон массива, если формула ячейки является массивной формулой. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | Получить результат условного форматирования. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | Получить все ячейки, формула которых напрямую ссылается на эту ячейку. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | Получает все ячейки, результат вычисления которых зависит от этой ячейки. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | Получает стиль отображения этой ячейки. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | Получает стиль отображения этой ячейки. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | Получает стиль отображения этой ячейки. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | Получает условия форматирования, применяемые к этой ячейке. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | Получить формулу этой ячейки. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | Служит хеш-функцией для определённого типа. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | Получает высоту значения в пикселях. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | Получает HTML-строку, содержащую данные и некоторые форматы в этой ячейке. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) Получить все ячейки, которые ссылаются на эту ячейку напрямую и должны быть обновлены, когда эта ячейка изменяется. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) Получить все ячейки, которые будут обновлены, когда эта ячейка изменяется. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | Возвращает объект [`Range`](../range/), который представляет объединённый диапазон. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | Получает все ссылки, появляющиеся в формуле этой ячейки. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | Получает все предшествующие (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при её вычислении. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | Получает расширенное значение ячейки. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | Получает строковое значение по определённой стратегии форматирования. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | Получает стиль ячейки. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | Если checkBorders истинно, проверяет, повлияют ли границы других ячеек на стиль этой ячейки. |
| [GetTable](../../aspose.cells/cell/gettable/)() | Получает таблицу, содержащую эту ячейку. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | Получает проверку, применённую к этой ячейке. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | Получает значение проверки, примененной к этой ячейке. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | Получает ширину значения в пикселях. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | Вставляет несколько символов в ячейку. Если ячейка имеет богатое форматирование, этот метод может сохранить исходное форматирование. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | Указывает, является ли строковое значение этой ячейки текстом с богатым форматированием. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | Записывает логическое значение в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | Записывает значение DateTime в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | Записывает значение double в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | Записывает целочисленное значение в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | Записывает объектное значение в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | Записывает строковое значение в ячейку. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | Записывает строковое значение в ячейку и при необходимости преобразует его в другой тип данных. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | Записывает значение в ячейку; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | Удалить формулу массива. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | Заменить текст ячейки с параметрами. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | Устанавливает массивную формулу (устаревшую массивную формулу, вводимую с помощью CTRL+SHIFT+ENTER в MS Excel) для диапазона ячеек. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | Устанавливает массивную формулу для диапазона ячеек. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Устанавливает массивную формулу для диапазона ячеек. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Устанавливает массивную формулу для диапазона ячеек. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | Устанавливает форматирование RTF ячейки. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Устанавливает динамическую массивную формулу и, если возможно, позволяет ей вытекать в соседние ячейки. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Устанавливает динамическую массивную формулу и, если возможно, позволяет ей вытекать в соседние ячейки. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | Устанавливает динамическую массивную формулу и, если возможно, позволяет ей вытекать в соседние ячейки. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | Устанавливает формулу и значение (рассчитанный результат) формулы. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | Устанавливает формулу и значение (рассчитанный результат) формулы. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | Устанавливает формулу и значение (рассчитанный результат) формулы. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsolete.**) Устанавливает формулу и значение формулы. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | Устанавливает общие формулы для диапазона ячеек. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | Устанавливает общие формулы для диапазона ячеек. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Устанавливает формулу для диапазона ячеек. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Устанавливает общие формулы для диапазона ячеек. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | Устанавливает стиль ячейки. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | Применяет изменённое свойство стиля к ячейке. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | Применить стиль ячейки на основе флагов. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | Создать однопараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | Создать двухпараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | Создать однопараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | Создать двухпараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки. |
| [ToJson](../../aspose.cells/cell/tojson/)() | Преобразовать `Cell` в данные структуры JSON. |
| override [ToString](../../aspose.cells/cell/tostring/)() | Возвращает строку, представляющую текущий объект Cell. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellDemo
    {
        public static void CellExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            // Получить доступ к коллекции ячеек
            Cells cells = worksheet.Cells;

            // Поместить строку в ячейку
            Cell cell = cells[0, 0];
            cell.PutValue("Hello");

            // Поместить целое число в ячейку
            cell = cells["B1"];
            cell.PutValue(12);

            // Поместить число с плавающей точкой в ячейку
            cell = cells[0, 2];
            cell.PutValue(-1.234);

            // Поместить формулу в ячейку
            cell = cells["D1"];
            cell.Formula = "=B1 + C1";

            // Поместить комбинированную формулу: "sum(average(b1,c1), b1)" в ячейку b2
            cell = cells["B2"];
            cell.Formula = "=sum(average(b1,c1), b1)";

            // Установить стиль ячейки
            Style style = cell.GetStyle();
            // Установить цвет фона
            style.BackgroundColor = System.Drawing.Color.Yellow;
            // Установить шрифт ячейки
            style.Font.Name = "Courier New";
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("CellExample.xlsx");
            workbook.Save("CellExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


