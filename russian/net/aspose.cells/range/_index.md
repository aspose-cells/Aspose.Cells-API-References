---
title: Range
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий диапазон ячеек в электронной таблице.
type: docs
weight: 5030
url: /ru/net/aspose.cells/range/
---
## Range class

Инкапсулирует объект, представляющий диапазон ячеек в электронной таблице.

```csharp
public class Range
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Получает адрес диапазона. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Получает количество столбцов в диапазоне. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Устанавливает или получает ширину столбца этого диапазона |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Возвращает объект Range, представляющий текущий регион. Текущая область представляет собой диапазон, ограниченный любой комбинацией пустых строк и пустых столбцов. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Получает объект Range, представляющий весь столбец (или столбцы), содержащий указанный диапазон. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Получает объект Range, представляющий всю строку (или строки), содержащую указанный диапазон. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Получает индекс первого столбца диапазона. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Получает индекс первой строки диапазона. |
| [Height](../../aspose.cells/range/height) { get; } | Получает ширину диапазона в пунктах. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Получает все гиперссылки в диапазоне. |
| [Item](../../aspose.cells/range/item) { get; } | получает[`Cell`](../cell) объект в этом диапазоне. |
| [Left](../../aspose.cells/range/left) { get; } | Получает расстояние в пунктах от левого края столбца A до левого края диапазона. |
| [Name](../../aspose.cells/range/name) { get; set; } | Получает или задает имя диапазона. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Получает ссылки на диапазон. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Получает количество строк в диапазоне. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Устанавливает или получает высоту строк в этом диапазоне |
| [Top](../../aspose.cells/range/top) { get; } | Получает расстояние в пунктах от верхнего края строки 1 до верхнего края диапазона. |
| [Value](../../aspose.cells/range/value) { get; set; } | Получает и устанавливает значение диапазона. |
| [Width](../../aspose.cells/range/width) { get; } | Получает ширину диапазона в пунктах. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | Получает[`Worksheet`](./worksheet) объект, который содержит этот диапазон. |

## Методы

| Имя | Описание |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Применяет форматы ко всему диапазону. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Автоматически заполнять целевой диапазон. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Автоматически заполнять целевой диапазон. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Копирует данные (включая формулы), форматирование, объекты рисования и т. д. из исходного диапазона. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Копирование диапазона со специальными параметрами вставки. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Копирует данные ячейки (включая формулы) из исходного диапазона. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Копирует настройки стиля из исходного диапазона. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Копирует значение ячейки из исходного диапазона. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Экспортирует данные из этого диапазона вDataTable объект. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Экспортирует данные из этого диапазона вDataTable объект. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Экспортирует данные из этого диапазона вDataTable объект. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | получает[`Cell`](../cell) объект или ноль в этом диапазоне. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Получает перечислитель для ячеек в этом диапазоне. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | получает[`Range`](../range) диапазон по смещению. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Возвращает[`Range`](../range) объект, представляющий прямоугольное пересечение двух диапазонов. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Указывает, пересекается ли диапазон. |
| [Merge](../../aspose.cells/range/merge)() | Объединяет диапазон ячеек в одну ячейку. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Переместить текущий диапазон в диапазон назначения. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Помещает значение в диапазон, при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Установить внутренние границы диапазона. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Устанавливает границу контура вокруг диапазона ячеек. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Устанавливает границы контура вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Устанавливает границы строки вокруг диапазона ячеек. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Устанавливает стиль диапазона. |
| override [ToString](../../aspose.cells/range/tostring)() | Возвращает строку, представляющую текущий объект Range. |
| [Union](../../aspose.cells/range/union)(Range) | Возвращает объединение двух диапазонов. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Разъединяет объединенные ячейки этого диапазона. |

### Примеры

```csharp

[C#]

//Создание экземпляра объекта Workbook
Workbook workbook = new Workbook();
// Получить первые ячейки рабочего листа.
Cells cells = workbook.Worksheets[0].Cells;
// Создаем диапазон (A1:D3).
Range range = cells.CreateRange("A1", "D3");
// Установить значение в диапазоне.
range.Value = "Hello";
// Сохраняем файл Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Создание экземпляра объекта Workbook
Dim workbook As Workbook = New Workbook()
'Получите первые ячейки рабочего листа.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Создайте диапазон (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Установите значение в диапазоне.
range.Value = "Hello"
'Сохраните файл Excel
workbook.Save("book1.xlsm")
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
