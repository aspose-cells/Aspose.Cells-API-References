---
title: "Класс Cell"
linktitle: "Cell"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Cell. Инкапсулирует объект, представляющий cell в Go."
type: docs
weight: 200
url: /ru/go-cpp/cell/
---

## Cell class

Инкапсулирует объект, представляющий отдельную ячейку книги Workbook.

```go

type Cell struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [Calculate](./calculate/) | Вычисляет формулу ячейки. |
| [GetWorksheet](./getworksheet/) | Получает родительский лист. |
| [PutValue_Bool](./putvalue_bool/) | Помещает логическое значение в ячейку. |
| [PutValue_Int](./putvalue_int/) | Помещает целочисленное значение в ячейку. |
| [PutValue_Double](./putvalue_double/) | Помещает значение типа double в ячейку. |
| [PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | Помещает значение в ячейку; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [PutValue_String_Bool](./putvalue_string_bool/) | Помещает строковое значение в ячейку и при необходимости преобразует его в другой тип данных. |
| [PutValue_String](./putvalue_string/) | Помещает строковое значение в ячейку. |
| [PutValue_Date](./putvalue_date/) | Помещает значение DateTime в ячейку. |
| [PutValue_Object](./putvalue_object/) | Помещает объектное значение в ячейку. |
| [GetRow](./getrow/) | Получает номер строки (нумерация с нуля) ячейки. |
| [GetColumn](./getcolumn/) | Получает номер столбца (нумерация с нуля) ячейки. |
| [IsFormula](./isformula/) | Отображает, содержит ли указанная ячейка формулу. |
| [GetHasCustomFunction](./gethascustomfunction/) | Проверяет, есть ли в формуле этой ячейки пользовательская функция (неподдерживаемая функция). |
| [GetType](./gettype/) | Отображает тип значения ячейки. |
| [GetName](./getname/) | Получает имя ячейки. |
| [IsErrorValue](./iserrorvalue/) | Проверяет, является ли значение этой ячейки ошибкой. |
| [IsNumericValue](./isnumericvalue/) | Указывает, является ли значение этой ячейки числовым (int, double и datetime). |
| [GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | Получает строковое значение по определённой стратегии форматирования. |
| [GetStringValue](./getstringvalue/) | Получает строковое значение, содержащееся в ячейке. Если тип этой ячейки — строка, то возвращается само строковое значение. Для других типов ячеек будет возвращено отформатированное строковое значение (отформатированное согласно указанному стилю этой ячейки). Отформатированное значение ячейки совпадает с тем, что можно получить из Excel при копировании ячейки как текста (например, при копировании ячейки в текстовый редактор или экспорте в CSV). |
| [GetNumberCategoryType](./getnumbercategorytype/) | Отображает тип категории числового форматирования этой ячейки. |
| [GetDisplayStringValue](./getdisplaystringvalue/) | Получает отформатированное строковое значение этой ячейки согласно её стилю отображения. |
| [GetIntValue](./getintvalue/) | Получает целочисленное значение, содержащееся в ячейке. |
| [GetDoubleValue](./getdoublevalue/) | Получает значение double, содержащееся в ячейке. |
| [GetFloatValue](./getfloatvalue/) | Получает значение float, содержащееся в ячейке. |
| [GetDateTimeValue](./getdatetimevalue/) | Получает значение DateTime, содержащееся в ячейке. |
| [GetBoolValue](./getboolvalue/) | Получает логическое значение, содержащееся в ячейке. |
| [GetWidthOfValue](./getwidthofvalue/) | Получает ширину значения в пикселях. |
| [GetHeightOfValue](./getheightofvalue/) | Получает высоту значения в пикселях. |
| [GetDisplayStyle](./getdisplaystyle/) | Получает стиль отображения этой ячейки. |
| [GetDisplayStyle_Bool](./getdisplaystyle_bool/) | Получает стиль отображения этой ячейки. |
| [GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | Получает стиль отображения этой ячейки. |
| [GetFormatConditions](./getformatconditions/) | Получает условия форматирования, применяемые к этой ячейке. |
| [GetStyle](./getstyle/) | Получает стиль ячейки. |
| [GetStyle_Bool](./getstyle_bool/) | Если checkBorders равно true, проверяется, влияют ли границы других ячеек на стиль этой ячейки. |
| [SetStyle_Style](./setstyle_style/) | Устанавливает стиль ячейки. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Применяет изменённое свойство стиля к ячейке. |
| [SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | Применяет стиль ячейки на основе флагов. |
| [GetHasCustomStyle](./gethascustomstyle/) | Указывает, имеет ли эта ячейка пользовательские настройки стиля (отличные от стиля по умолчанию, унаследованного от соответствующей строки, столбца или книги). |
| [GetSharedStyleIndex](./getsharedstyleindex/) | Получает индекс общего стиля ячейки в пуле стилей. |
| [GetFormula](./getformula/) | Получает или задает формулу ячейки. |
| [SetFormula_String](./setformula_string/) | Получает или задает формулу ячейки. |
| [GetFormulaLocal](./getformulalocal/) | Получает локализованную формулу ячейки. |
| [SetFormulaLocal](./setformulalocal/) | Получает локализованную формулу ячейки. |
| [GetR1C1Formula](./getr1c1formula/) | Получает или задает формулу R1C1 ячейки. |
| [SetR1C1Formula](./setr1c1formula/) | Получает или задает формулу R1C1 ячейки. |
| [SetFormula_String_Object](./setformula_string_object/) | Устанавливает формулу и значение (рассчитанный результат) формулы. |
| [SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | Устанавливает формулу и значение (рассчитанный результат) формулы. |
| [GetFormula_Bool_Bool](./getformula_bool_bool/) | Получает формулу этой ячейки. |
| [SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | Устанавливает формулу и значение (рассчитанный результат) формулы. |
| [SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | Устанавливает массивную формулу (устаревшую массивную формулу, вводимую с помощью CTRL+SHIFT+ENTER в MS Excel) для диапазона ячеек. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | Устанавливает массивную формулу для диапазона ячеек. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | Устанавливает массивную формулу для диапазона ячеек. |
| [SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | Устанавливает общие формулы для диапазона ячеек. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | Устанавливает общие формулы для диапазона ячеек. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | Устанавливает общие формулы для диапазона ячеек. |
| [GetContainsExternalLink](./getcontainsexternallink/) | Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только к ячейкам с формулой. |
| [GetPrecedents](./getprecedents/) | Получает все ссылки, присутствующие в формуле этой ячейки. |
| [GetDependents](./getdependents/) | Получает все ячейки, формулы которых напрямую ссылаются на эту ячейку. |
| [GetPrecedentsInCalculation](./getprecedentsincalculation/) | Получает все предшествующие (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при её вычислении. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Получает все ячейки, результат вычисления которых зависит от этой ячейки. |
| [IsArrayHeader](./isarrayheader/) | Указывает, что формула ячейки является массивной формулой и что эта ячейка является первой в массиве. |
| [IsDynamicArrayFormula](./isdynamicarrayformula/) | Указывает, является ли формула ячейки динамической массивной формулой (true) или устаревшей массивной формулой (false). |
| [GetArrayRange](./getarrayrange/) | Получает диапазон массива, если формула ячейки является массивной формулой. |
| [IsArrayFormula](./isarrayformula/) | Указывает, является ли формула ячейки массивной формулой. |
| [IsSharedFormula](./issharedformula/) | Указывает, является ли формула ячейки частью общей формулы. |
| [IsTableFormula](./istableformula/) | Указывает, является ли эта ячейка частью табличной формулы. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | Устанавливает динамическую массивную формулу и, если возможно, позволяет ей распространяться на соседние ячейки. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | Устанавливает динамическую массивную формулу и, если возможно, позволяет ей распространяться на соседние ячейки. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | Устанавливает динамическую массивную формулу и, если возможно, позволяет ей распространяться на соседние ячейки. |
| [SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | Создаёт таблицу данных с двумя переменными для указанного диапазона, начиная с этой ячейки. |
| [SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | Создаёт таблицу данных с одной переменной для указанного диапазона, начиная с этой ячейки. |
| [SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | Создаёт таблицу данных с двумя переменными для указанного диапазона, начиная с этой ячейки. |
| [SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | Создаёт таблицу данных с одной переменной для указанного диапазона, начиная с этой ячейки. |
| [RemoveArrayFormula](./removearrayformula/) | Удалить массивную формулу. |
| [Copy](./copy/) | Копирует данные из исходной ячейки. |
| [GetValue](./getvalue/) | Получает/устанавливает значение, содержащееся в этой ячейке. |
| [SetValue](./setvalue/) | Получает/устанавливает значение, содержащееся в этой ячейке. |
| [IsStyleSet](./isstyleset/) | Указывает, установлен ли стиль ячейки. Если возвращает false, это означает, что у этой ячейки формат по умолчанию. |
| [Characters](./characters/) | Возвращает объект Characters, представляющий диапазон символов в тексте ячейки. |
| [Replace](./replace/) | Заменяет текст ячейки с параметрами. |
| [InsertText](./inserttext/) | Вставляет несколько символов в ячейку. Если ячейка имеет rich‑форматирование, этот метод может сохранить оригинальное форматирование. |
| [IsRichText](./isrichtext/) | Указывает, является ли строковое значение этой ячейки текстом с rich‑форматированием. |
| [GetCharacters](./getcharacters/) | Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки. |
| [GetCharacters_Bool](./getcharacters_bool/) | Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки. |
| [SetCharacters](./setcharacters/) | Устанавливает rich‑текстовое форматирование ячейки. |
| [IsMerged](./ismerged/) | Проверяет, является ли ячейка частью объединённого диапазона. |
| [GetMergedRange](./getmergedrange/) | Возвращает объект Range, представляющий объединённый диапазон. |
| [GetComment](./getcomment/) | Получает комментарий этой ячейки. |
| [GetHtmlString](./gethtmlstring/) | Получает и устанавливает HTML‑строку, содержащую данные и некоторые форматы в этой ячейке. |
| [SetHtmlString](./sethtmlstring/) | Получает и устанавливает HTML‑строку, содержащую данные и некоторые форматы в этой ячейке. |
| [GetHtmlString_Bool](./gethtmlstring_bool/) | Получает HTML‑строку, содержащую данные и некоторые форматы в этой ячейке. |
| [ToString](./tostring/) | Возвращает строку, представляющую текущий объект Cell. |
| [ToJson](./tojson/) | Преобразует ячейку в данные структуры JSON. |
| [Equals_Object](./equals_object/) | Проверяет, ссылается ли этот объект на ту же ячейку, что и другой. |
| [GetHashCode](./gethashcode/) | Служит хеш‑функцией для определённого типа. |
| [Equals_Cell](./equals_cell/) | Проверяет, ссылается ли этот объект на ту же ячейку, что и другой объект ячейки. |
| [GetConditionalFormattingResult](./getconditionalformattingresult/) | Получить результат условного форматирования. |
| [GetValidation](./getvalidation/) | Получает проверку, применённую к этой ячейке. |
| [GetValidationValue](./getvalidationvalue/) | Получает значение проверки, применённой к этой ячейке. |
| [GetTable](./gettable/) | Получает таблицу, содержащую эту ячейку. |
| [IsCheckBoxStyle](./ischeckboxstyle/) | Указывает, устанавливается ли эта ячейка как флажок. |
| [SetIsCheckBoxStyle](./setischeckboxstyle/) | Указывает, устанавливается ли эта ячейка как флажок. |
| [GetRichValue](./getrichvalue/) | Получает rich‑значение ячейки. |
| [GetEmbeddedImage](./getembeddedimage/) | Получает и устанавливает встроенное изображение в ячейке. |
| [SetEmbeddedImage](./setembeddedimage/) | Получает и устанавливает встроенное изображение в ячейке. |
| [GetPicture](./getpicture/) | Получает объект Aspose.Cells.Drawing.Picture, представляющий встроенное изображение в этой ячейке, или null, если для этой ячейки нет встроенного изображения. |
|[Dispose](./dispose/) |  | 
