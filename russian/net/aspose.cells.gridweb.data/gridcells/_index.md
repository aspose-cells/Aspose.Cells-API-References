---
title: "Класс GridCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridWeb.Data.GridCells класс. Инкапсулирует коллекцию объектов GridCell"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Инкапсулирует коллекцию объектов [`GridCell`](../gridcell/).

```csharp
public class GridCells : IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns/) { get; } | Получает коллекцию объектов [`GridColumn`](../gridcolumn/), представляющих отдельные столбцы в этом листе. |
| [Count](../../aspose.cells.gridweb.data/gridcells/count/) { get; } | Возвращает количество ячеек. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell/) { get; } | Получает первую ячейку в этом листе. |
| [Item](../../aspose.cells.gridweb.data/gridcells/item/) { get; } | Возвращает элемент [`GridCell`](../gridcell/) по указанному индексу строки ячейки и индексу столбца. (2 индексатора) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell/) { get; } | Получает последнюю ячейку в этом листе. |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn/) { get; } | Максимальный индекс столбца ячейки, содержащей данные или стиль. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn/) { get; } | Максимальный индекс столбца ячейки, содержащей данные. |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow/) { get; } | Максимальный индекс строки ячейки, содержащей данные. |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow/) { get; } | Максимальный индекс строки ячейки, содержащей данные или стиль. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells/) { get; } | Возвращает коллекцию объединённых ячеек. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn/) { get; } | Минимальный индекс столбца среди ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка в нём не создана). |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn/) { get; } | Минимальный индекс столбца ячейки, содержащей данные. |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow/) { get; } | Минимальный индекс строки ячейки, содержащей данные. |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow/) { get; } | Минимальный индекс строки ячейки, содержащей данные или стиль. |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator/) { get; } | Получает перечислитель строк |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows/) { get; } | Возвращает коллекцию объектов [`GridRow`](../gridrow/), представляющих отдельные строки в этом листе. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight/) { get; set; } | Возвращает или задает высоту строки по умолчанию в этом листе, в единицах точек. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels/) { get; set; } | Возвращает или задает высоту строки по умолчанию в этом листе, в единицах пикселей. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth/) { get; set; } | Возвращает или задает ширину столбца по умолчанию в листе, в единицах символов. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch/) { get; set; } | Получает или задает ширину столбца по умолчанию в листе, в единицах дюймов. |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels/) { get; set; } | Получает или задает ширину столбца по умолчанию в листе, в единицах пикселей. |

## Методы

| Имя | Описание |
| --- | --- |
| [CheckCell](../../aspose.cells.gridweb.data/gridcells/checkcell/)(int, int) | Возвращает элемент [`GridCell`](../gridcell/) или null по указанному индексу строки ячейки и индексу столбца. |
| [CheckColumn](../../aspose.cells.gridweb.data/gridcells/checkcolumn/)(int) | Получает элемент [`GridColumn`](../gridcolumn/) или null по указанному индексу столбца. |
| [CheckRow](../../aspose.cells.gridweb.data/gridcells/checkrow/)(int) | Возвращает элемент [`GridRow`](../gridrow/) или null по указанному индексу строки ячейки. |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear/)() | Очистить все ячейки в коллекции. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Очищает содержимое диапазона. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Очищает содержимое диапазона. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats)(GridCellArea) | Очищает форматирование диапазона. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Очищает форматирование диапазона. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange)(GridCellArea) | Очищает содержимое и форматирование диапазона. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Очищает содержимое и форматирование диапазона. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn/)(GridCells, int, int) | Копирует данные и форматирование целого столбца. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns/)(GridCells, int, int, int) | Копирует данные и форматирование целого столбца. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow/)(GridCells, int, int) | Копирует данные и форматирование целой строки. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows/)(GridCells, int, int, int) | Копирует данные и форматирование нескольких целых строк. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns/)() | Удаляет все пустые столбцы, которые не содержат никаких данных. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows/)() | Удалить все пустые строки, которые не содержат данных. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn)(int) | Удаляет столбец. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Удаляет столбец. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns/)(int, int, bool) | Удаляет несколько столбцов. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange/)(int, int, int, int, GridShiftType) | Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow/)(int) | Удаляет строку. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows)(int, int) | Удаляет несколько строк. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Удаляет несколько строк в листе. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export/)(int, int, int, int, bool, bool) | Экспортирует данные из коллекции Cells веб‑листa WebWorksheet в новый объект DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray/)(int, int, int, int) | Экспортирует данные из коллекции `GridCells` в объект двумерного массива. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell/)(int, int) | Получает элемент [`GridCell`](../gridcell/) по указанному индексу строки и индексу столбца ячейки. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth/)(int) | Возвращает ширину указанного столбца |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch/)(int) | Возвращает ширину указанного столбца, в единицах дюймов. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel/)(int) | Возвращает ширину указанного столбца, в единицах пикселей. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator/)() | Получает перечислитель строк |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow/)(int) | Возвращает элемент [`GridRow`](../gridrow/) по указанному индексу строки ячейки. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight/)(int) | Получает высоту указанной строки. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch/)(int) | Получает высоту указанной строки в дюймах. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel/)(int) | Получает высоту указанной строки в пикселях. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel/)(int) | Получает уровень структуры строки. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel/)(int) | Получает ширину в разных типах представления. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Группирует столбцы. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Группирует столбцы. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows/)(int, int) | Группирует строки. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn/)(int) | Скрывает столбец. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow/)(int) | Скрывает строку. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn)(int) | Вставляет новый столбец в лист. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Вставляет новый столбец в лист. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Вставляет несколько столбцов в лист. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Вставляет несколько столбцов в лист. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange)(GridCellArea, GridShiftType) | Вставляет диапазон ячеек и смещает ячейки в соответствии с параметром смещения. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Вставляет диапазон ячеек и смещает ячейки в соответствии с параметром смещения. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow/)(int) | Вставляет новую строку в лист. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows)(int, int) | Вставляет несколько строк в лист. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Вставляет несколько строк в лист. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn/)(int) | Проверяет, является ли указанный столбец пустым (не содержит данных). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden/)(int) | Проверяет, скрыт ли столбец с указанным индексом. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden/)(int) | Проверяет, скрыта ли строка с указанным индексом. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge/)(int, int, int, int) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange/)(GridCellArea, int, int) | Перемещает диапазон. |
| [RemoveDuplicates](../../aspose.cells.gridweb.data/gridcells/removeduplicates/)(int, int, int, int) | Удаляет дублирующие значения в диапазоне. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas/)() | Удаляет все формулы и заменяет их значением формулы. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Устанавливает границы для диапазона ячеек. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth/)(int, double) | Задает ширину указанного столбца. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch/)(int, double) | Устанавливает ширину столбца в дюймах. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel/)(int, int) | Устанавливает ширину столбца в пикселях. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight/)(int, double) | Устанавливает высоту указанной строки. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch/)(int, double) | Устанавливает высоту строки в дюймах. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel/)(int, int) | Устанавливает высоту строки в пикселях. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel/)(int, int) | Устанавливает уровень структуры строки. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle_1)(string, GridTableItemStyle) | Устанавливает стиль для указанного диапазона ячеек. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle)(int, int, int, int, GridTableItemStyle) | Устанавливает стиль для указанного диапазона ячеек. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки. |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns/)(int, int) | Разгруппирует столбцы. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows/)(int, int) | Разгруппирует строки. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn/)(int, double) | Отображает скрытый столбец |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow/)(int) | Отображает скрытую строку. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge/)(int, int, int, int) | Разъединяет указанный диапазон объединённых ячеек. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname/)(int, int) | Получает имя ячейки в соответствии с её индексами строки и столбца. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex/)(string, out int, out int) | Получает индексы строки и столбца ячейки по её имени |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname/)(int) | Получает имя столбца в соответствии с индексом столбца. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex/)(string) | Получает индекс столбца в соответствии с именем столбца. |

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


