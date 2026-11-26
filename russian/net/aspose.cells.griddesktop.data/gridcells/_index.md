---
title: "Класс GridCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridDesktop.Data.GridCells. Инкапсулирует коллекцию объектов Cell"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Инкапсулирует коллекцию объектов Cell.

```csharp
public class GridCells : IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns/) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count/) { get; } | Возвращает количество ячеек. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell/) { get; } | Получает первую ячейку в этом листе. |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item/) { get; } | Возвращает элемент [`GridCell`](../gridcell/) по указанному индексу строки ячейки и индексу столбца. (2 индексатора) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell/) { get; } | Получает последнюю ячейку в этом листе. |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn/) { get; } | Максимальный индекс столбца ячейки, содержащей данные или стиль. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn/) { get; } | Максимальный индекс столбца ячейки, содержащей данные. |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow/) { get; } | Максимальный индекс строки ячейки, содержащей данные. |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow/) { get; } | Максимальный индекс строки ячейки, содержащей данные или стиль. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells/) { get; } | Возвращает коллекцию объединённых ячеек. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn/) { get; } | Минимальный индекс столбца среди ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка в нём не создана). |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn/) { get; } | Минимальный индекс столбца ячейки, содержащей данные. |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow/) { get; } | Минимальный индекс строки ячейки, содержащей данные. |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow/) { get; } | Минимальный индекс строки ячейки, содержащей данные или стиль. |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator/) { get; } | Получает перечислитель строк |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows/) { get; } | Возвращает коллекцию объектов [`GridRow`](../gridrow/), представляющих отдельные строки в этом листе. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight/) { get; set; } | Возвращает или задает высоту строки по умолчанию в этом листе, в единицах точек. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels/) { get; set; } | Возвращает или задает высоту строки по умолчанию в этом листе, в единицах пикселей. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth/) { get; set; } | Возвращает или задает ширину столбца по умолчанию в листе, в единицах символов. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch/) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell/)(int, int) | Возвращает элемент [`GridCell`](../gridcell/) или null по указанному индексу строки ячейки и индексу столбца. |
| [CheckRow](../../aspose.cells.griddesktop.data/gridcells/checkrow/)(int) | Возвращает элемент [`GridRow`](../gridrow/) или null по указанному индексу строки ячейки. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear/)() | Очистить все ячейки в коллекции. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Очищает содержимое диапазона. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Очищает содержимое диапазона. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats)(GridCellArea) | Очищает форматирование диапазона. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Очищает форматирование диапазона. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange)(GridCellArea) | Очищает содержимое и форматирование диапазона. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Очищает содержимое и форматирование диапазона. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn/)(GridCells, int, int) | Копирует данные и форматирование целого столбца. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns/)(GridCells, int, int, int) | Копирует данные и форматирование целого столбца. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow/)(GridCells, int, int) | Копирует данные и форматирование целой строки. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows/)(GridCells, int, int, int) | Копирует данные и форматирование нескольких целых строк. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns/)() | Удаляет все пустые столбцы, которые не содержат никаких данных. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows/)() | Удалить все пустые строки, которые не содержат данных. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn)(int) | Удаляет столбец. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Удаляет столбец. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns/)(int, int, bool) | Удаляет несколько столбцов. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow/)(int) | Удаляет строку. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows)(int, int) | Удаляет несколько строк. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Удаляет несколько строк в листе. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle/)(int, int) | Получить стиль заданной ячейки. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn/)(int) | Возвращает элемент [`GridColumn`](../gridcolumn/) по указанному индексу столбца ячейки. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth/)(int) | Возвращает ширину указанного столбца |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch/)(int) | Возвращает ширину указанного столбца, в единицах дюймов. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel/)(int) | Возвращает ширину указанного столбца, в единицах пикселей. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator/)() | Получает перечислитель строк |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow/)(int) | Возвращает элемент [`GridRow`](../gridrow/) по указанному индексу строки ячейки. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight/)(int) | Получает высоту указанной строки. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch/)(int) | Получает высоту указанной строки в дюймах. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel/)(int) | Получает высоту указанной строки в пикселях. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel/)(int) | Получает ширину в разных типах представления. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Группирует столбцы. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Группирует столбцы. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows/)(int, int) | Группирует строки. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn/)(int) | Скрывает столбец. |
| [HideColumns](../../aspose.cells.griddesktop.data/gridcells/hidecolumns/)(int, int) | Скрывает несколько столбцов. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow/)(int) | Скрывает строку. |
| [HideRows](../../aspose.cells.griddesktop.data/gridcells/hiderows/)(int, int) | Скрывает несколько строк. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn)(int) | Вставляет новый столбец в лист. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Вставляет новый столбец в лист. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Вставляет несколько столбцов в лист. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Вставляет несколько столбцов в лист. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow/)(int) | Вставляет новую строку в лист. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows)(int, int) | Вставляет несколько строк в лист. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Вставляет несколько строк в лист. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn/)(int) | Проверяет, является ли указанный столбец пустым (не содержит данных). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden/)(int) | Проверяет, скрыт ли столбец с указанным индексом. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden/)(int) | Проверяет, скрыта ли строка с указанным индексом. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge/)(int, int, int, int) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas/)() | Удаляет все формулы и заменяет их значением формулы. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth/)(int, double) | Задает ширину указанного столбца. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch/)(int, double) | Устанавливает ширину столбца в дюймах. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel/)(int, int) | Устанавливает ширину столбца в пикселях. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight/)(int, double) | Устанавливает высоту указанной строки. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch/)(int, double) | Устанавливает высоту строки в дюймах. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel/)(int, int) | Устанавливает высоту строки в пикселях. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle)(CellRange, Style) | Устанавливает стиль для указанного диапазона ячеек. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_2)(string, Style) | Устанавливает стиль для указанного диапазона ячеек. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_1)(int, int, int, int, Style) | Устанавливает стиль для указанного диапазона ячеек. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) | Сортирует данные области. |
| [SortAsNumber](../../aspose.cells.griddesktop.data/gridcells/sortasnumber/)(int, int, int, int, int[], SortOrder[], SortOrientation) | Сортирует данные области (значения в ключевом столбце должны быть числом). |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns/)(int, int) | Разгруппирует столбцы. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows/)(int, int) | Разгруппирует строки. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn/)(int, double) | Отображает скрытый столбец |
| [UnhideColumns](../../aspose.cells.griddesktop.data/gridcells/unhidecolumns/)(int, int, double) | Отображает несколько скрытых столбцов. |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow/)(int, int) | Отображает скрытую строку. |
| [UnhideRows](../../aspose.cells.griddesktop.data/gridcells/unhiderows/)(int, int, double) | Отображает скрытые строки. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge/)(int, int, int, int) | Разъединяет указанный диапазон объединённых ячеек. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname/)(int, int) | Получает имя ячейки в соответствии с её индексами строки и столбца. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex/)(string, out int, out int) | Получает индексы строки и столбца ячейки по её имени |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname/)(int) | Получает имя столбца в соответствии с индексом столбца. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex/)(string) | Получает индекс столбца в соответствии с именем столбца. |

### См. также

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


