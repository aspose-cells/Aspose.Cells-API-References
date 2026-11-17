---
title: "UnionRange Класс"
linktitle: "UnionRange"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "UnionRange класс. Инкапсулирует объект, представляющий unionrange в Go."
type: docs
weight: 200
url: /ru/go-cpp/unionrange/
---

## UnionRange class

Представляет объединённый диапазон.

```go

type UnionRange struct  {
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
| [GetFirstRow](./getfirstrow/) | Получает индекс первой строки диапазона. |
| [GetFirstColumn](./getfirstcolumn/) | Получает индекс первого столбца диапазона. |
| [GetRowCount](./getrowcount/) | Получает количество строк в диапазоне. |
| [GetColumnCount](./getcolumncount/) | Получает количество строк в диапазоне. |
| [Merge](./merge/) | Объединяет диапазон ячеек в одну ячейку. |
| [UnMerge](./unmerge/) | Разъединяет объединённые ячейки этого диапазона. |
| [PutValue](./putvalue/) | Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [GetValue](./getvalue/) | Получает и задает значения диапазона. |
| [SetValue](./setvalue/) | Получает и задает значения диапазона. |
| [GetName](./getname/) | Получает или задает имя диапазона. |
| [SetName](./setname/) | Получает или задает имя диапазона. |
| [GetRefersTo](./getrefersto/) | Получает, к чему относится диапазон. |
| [GetHasRange](./gethasrange/) | Указывает, имеет ли это диапазон. |
| [GetHyperlinks](./gethyperlinks/) | Получает все гиперссылки в диапазоне. |
| [SetStyle](./setstyle/) | Устанавливает стиль диапазона. |
| [ApplyStyle](./applystyle/) | Применяет форматы для всего диапазона. |
| [Copy](./copy/) | Копирует диапазон с параметрами «Специальная вставка». |
| [GetEnumerator](./getenumerator/) | Получает перечислитель ячеек в этом диапазоне Range. |
| [GetCellCount](./getcellcount/) | Получает общее количество ячеек в диапазоне. |
| [GetRangeCount](./getrangecount/) | Получает количество диапазонов. |
| [GetRanges](./getranges/) | Получает все объединённые диапазоны. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Устанавливает контурные границы вокруг диапазона ячеек. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [Intersect_String](./intersect_string/) | Пересекает другой диапазон. |
| [Intersect_UnionRange](./intersect_unionrange/) | Пересекает другой диапазон. |
| [Intersect_RangeArray](./intersect_rangearray/) | Пересекает другой диапазон. |
| [Union_String](./union_string/) | Объединить другой диапазон. |
| [Union_UnionRange](./union_unionrange/) | Объединить другой диапазон. |
| [Union_RangeArray](./union_rangearray/) | Объединить диапазоны. |
