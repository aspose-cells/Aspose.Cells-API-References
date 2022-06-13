---
title: GridCells
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует набор объектовCell.
type: docs
weight: 410
url: /ru/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Инкапсулирует набор объектовCell.

```csharp
public class GridCells : IEnumerable
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count) { get; } | Получает количество ячеек. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item) { get; } | ПолучаетCellэлемент на листе (3 indexers) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn) { get; } | Максимальный индекс столбца ячейки, содержащей данные или стиль. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow) { get; } | Максимальный индекс строки ячейки, содержащей данные или стиль. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells) { get; } | Получает коллекцию объединенных ячеек. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator) { get; } | Получает перечислитель строк |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows) { get; } | Получает коллекцию объектов[`GridRow`](../gridrow), представляющих отдельные строки на этом листе. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight) { get; set; } | Получает или задает высоту строки по умолчанию на этом листе в пунктах. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels) { get; set; } | Получает или задает высоту строки по умолчанию на этом листе в пикселях. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth) { get; set; } | Получает или задает ширину столбца по умолчанию на листе в единицах символов. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell)(int, int) | Получает элементCellили null в указанном индексе строки ячейки и индексе столбца. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear)() | Очистить все ячейки коллекции. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents)(GridCellArea) | Очищает содержимое диапазона. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | Очищает содержимое диапазона. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats)(GridCellArea) | Очищает форматирование диапазона. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | Очищает форматирование диапазона. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange)(GridCellArea) | Очищает содержимое и форматирование диапазона. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | Очищает содержимое и форматирование диапазона. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn)(GridCells, int, int) | Копирует данные и форматирование всего столбца. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns)(GridCells, int, int, int) | Копирует данные и форматирование всего столбца. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow)(GridCells, int, int) | Копирует данные и форматирование всей строки. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows)(GridCells, int, int, int) | Копирует данные и форматирование некоторых целых строк. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns)() | Удалить все пустые столбцы, не содержащие данных. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows)() | Удалить все пустые строки, не содержащие данных. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn)(int) | Удаляет столбец. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | Удаляет столбец. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns)(int, int, bool) | Удаляет несколько столбцов. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow)(int) | Удаляет строку. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows)(int, int) | Удаляет несколько строк. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows_1)(int, int, bool) | Удаляет несколько строк на листе. |
| [GetCell](../../aspose.cells.griddesktop.data/gridcells/getcell)(int, int) | Получает элементCellили null в указанном индексе строки ячейки и индексе столбца. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle)(int, int) | Получить стиль данной ячейки. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn)(int) | Получает элемент[`GridColumn`](../gridcolumn)или указанный индекс столбца ячейки. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth)(int) | Получает ширину указанного столбца |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch)(int) | Получает ширину указанного столбца в дюймах. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel)(int) | Получает ширину указанного столбца в пикселях. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator)() | Получает перечислитель строк |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow)(int) | Получает элемент[`GridRow`](../gridrow)или указанный индекс строки ячейки. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight)(int) | Получает высоту указанной строки. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch)(int) | Получает высоту указанной строки в дюймах. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel)(int) | Получает высоту указанной строки в пикселях. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel)(int) | Получить ширину в другом типе представления. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns)(int, int) | Группирует столбцы. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | Группирует столбцы. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows)(int, int) | Группирует строки. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn)(int) | Скрывает столбец. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow)(int) | Скрывает строку. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn)(int) | Вставляет новый столбец в рабочий лист. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | Вставляет новый столбец в рабочий лист. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns)(int, int) | Вставляет несколько столбцов в рабочий лист. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | Вставляет несколько столбцов в рабочий лист. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow)(int) | Вставляет новую строку в рабочий лист. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows)(int, int) | Вставляет несколько строк в рабочий лист. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows_1)(int, int, bool) | Вставляет несколько строк в рабочий лист. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn)(int) | Проверяет, является ли данный столбец пустым (не содержит данных). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden)(int) | Проверяет, скрыт ли столбец с заданным индексом. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden)(int) | Проверяет, скрыта ли строка с заданным индексом. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge)(int, int, int, int) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas)() | Удаляет все формулы и заменяет значением формулы. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth)(int, double) | Устанавливает ширину указанного столбца. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch)(int, double) | Устанавливает ширину столбца в дюймах. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel)(int, int) | Устанавливает ширину столбца в пикселях. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight)(int, double) | Устанавливает высоту указанной строки. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch)(int, double) | Устанавливает высоту строки в дюймах. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel)(int, int) | Устанавливает высоту строки в пикселях. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle)(CellRange, Style) | Устанавливает стиль для указанного диапазона ячеек. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_2)(string, Style) | Устанавливает стиль для указанного диапазона ячеек. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_1)(int, int, int, int, Style) | Устанавливает стиль для указанного диапазона ячеек. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне рабочего листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне рабочего листа по указанному индексу строки. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns)(int, int) | Разгруппирует столбцы. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows)(int, int) | Разгруппирует строки. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn)(int, double) | Отображает столбец |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow)(int) | Отображает строку. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge)(int, int, int, int) | Разъединяет указанный диапазон объединенных ячеек. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname)(int, int) | Получает имя ячейки в соответствии с ее индексами строки и столбца. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex)(string, out int, out int) | Получает индексы строки и столбца ячейки в соответствии с ее именем |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname)(int) | Получает имя столбца по индексу столбца. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex)(string) | Получает индекс столбца по имени столбца. |

### Смотрите также

* пространство имен [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* сборка [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
