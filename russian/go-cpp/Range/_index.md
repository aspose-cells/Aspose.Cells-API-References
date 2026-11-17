---
title: "Класс Range"
linktitle: "Range"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Range. Инкапсулирует объект, представляющий range в Go."
type: docs
weight: 200
url: /ru/go-cpp/range/
---

## Range class

Инкапсулирует объект, представляющий диапазон ячеек в электронной таблице.

```go

type Range struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewRange_CellArea_Cells](./newrange_cellarea_cells/) | Конструктор класса. |
| [NewRange_Int_Int_Int_Int_Cells](./newrange_int_int_int_int_cells/) | Конструктор класса. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [AutoFill_Range](./autofill_range/) | Автоматически заполняет целевой диапазон. |
| [AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | Автоматически заполняет целевой диапазон. |
| [GetCurrentRegion](./getcurrentregion/) | Возвращает объект Range, представляющий текущий регион. Текущий регион — это диапазон, ограниченный любой комбинацией пустых строк и пустых столбцов. |
| [GetHyperlinks](./gethyperlinks/) | Получает все гиперссылки в диапазоне. |
| [AddHyperlink](./addhyperlink/) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [GetEnumerator](./getenumerator/) | Получает перечислитель ячеек в этом диапазоне Range. |
| [IsIntersect](./isintersect/) | Указывает, пересекается ли диапазон. |
| [Intersect](./intersect/) | Возвращает объект Range, представляющий прямоугольное пересечение двух диапазонов. |
| [UnionRanges](./unionranges/) | Возвращает результат объединения двух диапазонов. |
| [GetRowCount](./getrowcount/) | Получает количество строк в диапазоне. |
| [GetColumnCount](./getcolumncount/) | Получает количество столбцов в диапазоне. |
| [GetName](./getname/) | Получает или задает имя диапазона. |
| [SetName](./setname/) | Получает или задает имя диапазона. |
| [GetRefersTo](./getrefersto/) | Получает, к чему относится диапазон. |
| [GetAddress](./getaddress/) | Получает адрес диапазона. |
| [IsBlank](./isblank/) | Указывает, содержит ли диапазон значения. |
| [GetLeft](./getleft/) | Получает расстояние в пунктах от левого края столбца A до левого края диапазона. |
| [GetTop](./gettop/) | Получает расстояние в пунктах от верхнего края строки 1 до верхнего края диапазона. |
| [GetWidth](./getwidth/) | Получает ширину диапазона в пунктах. |
| [GetHeight](./getheight/) | Получает ширину диапазона в пунктах. |
| [GetFirstRow](./getfirstrow/) | Получает индекс первой строки диапазона. |
| [GetFirstColumn](./getfirstcolumn/) | Получает индекс первого столбца диапазона. |
| [Merge](./merge/) | Объединяет диапазон ячеек в одну ячейку. |
| [UnMerge](./unmerge/) | Разъединяет объединённые ячейки этого диапазона. |
| [PutValue](./putvalue/) | Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [GetValue](./getvalue/) | Получает и задает значение диапазона. |
| [SetValue](./setvalue/) | Получает и задает значение диапазона. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Применить стиль ячейки. |
| [ApplyStyle](./applystyle/) | Применяет форматы для всего диапазона. |
| [SetStyle_Style](./setstyle_style/) | Устанавливает стиль диапазона. |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Устанавливает контурные границы вокруг диапазона ячеек. |
| [SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | Устанавливает контурную границу вокруг диапазона ячеек. |
| [SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | Устанавливает контурную границу вокруг диапазона ячеек. |
| [SetInsideBorders](./setinsideborders/) | Устанавливает внутренние границы диапазона. |
| [GetColumnWidth](./getcolumnwidth/) | Устанавливает или получает ширину столбца этого диапазона |
| [SetColumnWidth](./setcolumnwidth/) | Устанавливает или получает ширину столбца этого диапазона |
| [GetRowHeight](./getrowheight/) | Устанавливает или получает высоту строк в этом диапазоне |
| [SetRowHeight](./setrowheight/) | Устанавливает или получает высоту строк в этом диапазоне |
| [MoveTo](./moveto/) | Перемещает текущий диапазон в целевой диапазон. |
| [CopyData](./copydata/) | Копирует данные ячеек (включая формулы) из исходного диапазона. |
| [CopyValue](./copyvalue/) | Копирует значение ячейки из исходного диапазона. |
| [CopyStyle](./copystyle/) | Копирует настройки стиля из исходного диапазона. |
| [Copy_Range_PasteOptions](./copy_range_pasteoptions/) | Копирует диапазон с параметрами «Специальная вставка». |
| [Transpose](./transpose/) | Транспонирует (поворачивает) данные из строк в столбцы и наоборот. |
| [Copy_Range](./copy_range/) | Копирует данные (включая формулы), форматирование, графические объекты и т.д. из исходного диапазона. |
| [Get](./get/) | Получает объект Cell в этом диапазоне. |
| [GetCellOrNull](./getcellornull/) | Получает объект Cell или null в этом диапазоне. |
| [GetOffset](./getoffset/) | Получает диапазон Range по смещению. |
| [GetEntireColumn](./getentirecolumn/) | Получает объект Range, представляющий весь столбец (или столбцы), содержащий указанный диапазон. |
| [GetEntireRow](./getentirerow/) | Получает объект Range, представляющий всю строку (или строки), содержащую указанный диапазон. |
| [GetWorksheet](./getworksheet/) | Получает объект Worksheet, который содержит этот диапазон. |
| [ToString](./tostring/) | Возвращает строку, представляющую текущий объект Range. |
| [ToImage](./toimage/) | Преобразует диапазон в изображение. |
| [ToJson](./tojson/) | Преобразует диапазон в значение JSON. |
| [ToHtml](./tohtml/) | Преобразует диапазон в HTML. |
| [Clear](./clear/) | Очищает этот диапазон. |
| [ClearContents](./clearcontents/) | Очищает содержимое этого диапазона. |
| [ClearFormats](./clearformats/) | Очищает форматы этого диапазона. |
| [ClearComments](./clearcomments/) | Очищает комментарии этого диапазона. |
| [ClearHyperlinks](./clearhyperlinks/) | Только удаляет гиперссылки. |
