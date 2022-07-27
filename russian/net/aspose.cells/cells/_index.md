---
title: Cells
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует коллекцию объектов относящихся к ячейке таких какCell./cell Row./row ...и т.д.
type: docs
weight: 300
url: /ru/net/aspose.cells/cells/
---
## Cells class

Инкапсулирует коллекцию объектов, относящихся к ячейке, таких как[`Cell`](../cell) ,[`Row`](../row) ...и т.д.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | Получает коллекцию[`Column`](../column) объекты, представляющие отдельные столбцы на этом листе. |
| [Count](../../aspose.cells/cells/count) { get; } | Получает общее количество экземпляров объектов Cell. |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | Получает общее количество экземпляров объектов Cell. |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | Получает первую ячейку на этом листе. |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | Указывает, что высота строки и высота шрифта по умолчанию совпадают |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | Указывает, скрыта ли строка по умолчанию. |
| [Item](../../aspose.cells/cells/item) { get; } | Получает[`Cell`](../cell) элемент с указанным индексом строки ячейки и индексом столбца. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | Получает последнюю ячейку на этом листе. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | Минимальный индекс столбца для тех ячеек, которые были созданы в коллекции (не включает столбец , где стиль определен для всего столбца, но в нем не было создано ни одной ячейки). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | Максимальный индекс столбца ячейки, содержащей данные. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | Максимальный индекс строки ячейки, содержащей данные. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | Получает максимальный диапазон, включающий данные, объединенные ячейки и фигуры. |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | Максимальный индекс строки ячейки, содержащей данные или стиль. |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | Получает или задает параметр использования памяти для этих ячеек. |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | Получает коллекцию объединенных ячеек. |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | Минимальный индекс столбца для тех ячеек, которые были созданы в коллекции (не включает столбец , где стиль определен для всего столбца, но в нем не было создано ни одной ячейки). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | Минимальный индекс столбца ячейки, содержащей данные. |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | Минимальный индекс строки ячейки, содержащей данные. |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | Минимальный индекс строки ячейки, содержащей данные или стиль. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | Получает или задает, должна ли модель данных ячеек поддерживать многопоточное чтение. Значение этого свойства по умолчанию — false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | Получает список полей ods. |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | Получает или задает значение, указывающее, сохраняются ли все значения рабочего листа в виде строк. Значение по умолчанию — false. |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | Получает коллекцию[`Range`](../range)объекты, созданные во время выполнения. |
| [Rows](../../aspose.cells/cells/rows) { get; } | Получает коллекцию[`Row`](../row) объекты, представляющие отдельные строки на этом листе. |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | Получает или задает высоту строки по умолчанию на этом листе в пунктах. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | Получает или задает высоту строки по умолчанию на этом листе в дюймах. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | Получает или задает высоту строки по умолчанию на этом листе в пикселях. |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | Получает или задает ширину столбца по умолчанию на листе в единицах символов. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | Получает или задает ширину столбца по умолчанию на листе в дюймах. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | Получает или задает ширину столбца по умолчанию на листе в пикселях. |
| [Style](../../aspose.cells/cells/style) { get; set; } | Получает и устанавливает стиль по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | Добавляет ссылку на объект диапазона в cell |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | Применяет форматы ко всему столбцу. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | Применяет формат ко всей строке. |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | Применяет форматы ко всему рабочему листу. |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | Получает[`Cell`](../cell) элемент или нуль в указанном индексе строки ячейки и индексе столбца. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | Получает[`Column`](../column) элемент или нуль в указанном индексе столбца. |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | Получает[`Row`](../row) элемента или по указанному индексу строки ячейки. |
| [Clear](../../aspose.cells/cells/clear)() | Очищает все объекты ячеек и строк. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | Очищает содержимое диапазона. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | Очищает содержимое диапазона. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | Очищает форматирование диапазона. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | Очищает форматирование диапазона. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | Очищает все объединенные диапазоны. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | Очищает содержимое и форматирование диапазона. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | Очищает содержимое и форматирование диапазона. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | Преобразует строковые данные в ячейках в числовое значение, если это возможно. |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | Копирует данные и форматы всего столбца. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | Копирует данные и форматы всего столбца. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | Копирует данные и форматы целых столбцов. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | Копирует данные и форматы всего столбца. |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | Копирует данные и форматы всей строки. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | Копирует данные и форматы некоторых целых строк. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | Копирует данные и форматы некоторых целых строк. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Копирует данные и форматы некоторых целых строк. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | Создает[`Range`](../range) объект с адреса диапазона. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | Создает[`Range`](../range) объект из диапазона ячеек. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | Создает[`Range`](../range) объект из строк ячеек или столбцов ячеек. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | Создает[`Range`](../range) объект из диапазона ячеек. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | Удалить все пустые столбцы, не содержащие данных. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | Удалить все пустые столбцы, не содержащие данных. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | Удалить все пустые строки, не содержащие данных. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | Удалить все пустые строки, не содержащие данных. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | Удаляет столбец. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | Удаляет столбец. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | Удаляет несколько столбцов. |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | Удаляет строку. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | Удаляет несколько строк. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | Удаляет несколько строк на листе. |
| [Dispose](../../aspose.cells/cells/dispose)() | Выполняет определяемые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | Получает последнюю ячейку в этом столбце. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | Получает последнюю ячейку с максимальным индексом столбца в этом диапазоне. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | Получает последнюю ячейку в этой строке. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | Получает последнюю ячейку с максимальным индексом строки в этом диапазоне. |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | Экспортирует данные в[`Cells`](../cells) коллекция в объект двумерного массива. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | Экспортирует данные в[`Cells`](../cells) сбор вDataTable объект. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | Экспортирует данные в[`Cells`](../cells) сбор вDataTable объект. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Экспортирует данные в[`Cells`](../cells) сбор вDataTable объект. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | Экспортирует данные в[`Cells`](../cells) сбор вDataTable объект. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | Экспортирует данные в[`Cells`](../cells) сбор вDataTable объект. |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | Экспортирует тип значения ячейки в[`Cells`](../cells) коллекция в объект двумерного массива. |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | Находит ячейку, содержащую входной объект. |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | Находит ячейку, содержащую входной объект. |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | Получает[`Cell`](../cell) элемент или нуль в указанном индексе строки ячейки и индексе столбца. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | Получить стиль данной ячейки. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | Получает ширину указанного столбца в обычном представлении |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | Получает ширину указанного столбца в обычном представлении в дюймах. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | Получает ширину указанного столбца в обычном режиме просмотра в пикселях. |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | Получить все ячейки, которые ссылаются на определенную ячейку. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation)(int, int, bool) | Получает все ячейки, расчетный результат которых зависит от конкретной ячейки. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | Получает перечислитель ячеек. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | Получает уровень структуры (отсчитываемый от нуля) столбца. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | Получает уровень структуры (отсчитываемый от нуля) строки. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | Получает индекс последней строки ячейки, которая содержит данные в указанном столбце. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | Получает максимальный уровень структуры сгруппированного столбца (отсчитывается от нуля). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | Получает максимальный уровень структуры сгруппированных строк (отсчитывается от нуля). |
| [GetRow](../../aspose.cells/cells/getrow)(int) | Получает[`Row`](../row) элемент по указанному индексу строки ячейки. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | Получает перечислитель строк. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | Получает высоту указанной строки. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | Получает высоту указанной строки в дюймах. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | Получает высоту указанной строки в пикселях. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | Получает высоту исходной строки в пунктах, если строка скрыта |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | Получить ширину в другом типе представления. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | Получает высоту указанной строки. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | Получает высоту указанной строки в дюймах. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | Группирует столбцы. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | Группирует столбцы. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | Группирует строки. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | Группирует строки. |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | Скрывает столбец. |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | Скрыть несколько столбцов. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | Сворачивает сгруппированные строки/столбцы. |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | Скрывает строку. |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | Скрывает несколько строк. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | Импортирует массив двойных чисел в рабочий лист. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | Импортирует массив целых чисел в рабочий лист. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | Импортирует массив строк в рабочий лист. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | Импорт массива данных на лист. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | Импорт файла CSV в ячейки. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | Импорт файла CSV в ячейки. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | Импорт файла CSV в ячейки. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | Импорт файла CSV в ячейки. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Импортирует пользовательские объекты. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Импортирует пользовательские объекты. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | Импорт данных изIDataReader объект. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | Импорт данных из пользовательской таблицы данных. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | Импорт данных из представления данных. |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Импорт данных из пользовательской таблицы данных. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | Импорт данных изIDataReader объект. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | ИмпортируетDataGrid в рабочий лист. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | ИмпортируетDataGrid в рабочий лист. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | ИмпортируетDataGrid в рабочий лист. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | ИмпортируетDataGrid в рабочий лист. Этот метод не пытается преобразовать текст в числовые значения. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | Импортирует DataRow в файл Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | ИмпортируетDataView в рабочий лист. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | Импортирует массив формул на лист. |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | Импортирует вид сетки в эти ячейки. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | Импортирует массив данных на лист. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | Импортирует массив данных на лист. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | Вставляет новый столбец в рабочий лист. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | Вставляет новый столбец в рабочий лист. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | Вставляет несколько столбцов на лист. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | Вставляет несколько столбцов на лист. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | Вставить диапазон обрезки. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | Вставляет новую строку в рабочий лист. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | Вставляет несколько строк в рабочий лист. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | Вставляет несколько строк в рабочий лист. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | Вставляет несколько строк в рабочий лист. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | Проверяет, является ли данный столбец пустым (не содержит данных). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | Проверяет, скрыт ли столбец с данным индексом. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | Проверить, можно ли удалить диапазон. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | Проверяет, скрыта ли строка с данным индексом. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | Ссылка на карту xml. |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | Перемещает диапазон. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | Удаляет повторяющиеся строки на листе. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | Удаляет повторяющиеся значения в диапазоне. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | Удаляет повторяющиеся данные диапазона. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | Удаляет все формулы и заменяет значением формулы. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | Извлекает настройку промежуточных итогов диапазона. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | Устанавливает ширину указанного столбца в обычном представлении. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | Устанавливает ширину столбца в дюймах в обычном режиме просмотра. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | Устанавливает ширину столбца в пикселях в обычном режиме просмотра. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | Устанавливает высоту указанной строки. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | Устанавливает высоту строки в дюймах. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | Устанавливает высоту строки в пикселях. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | Устанавливает ширину столбца в другом представлении. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | Разворачивает сгруппированные строки/столбцы. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Создает промежуточные итоги для диапазона. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Создает промежуточные итоги для диапазона. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | Разбивает текст в столбце на столбцы. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | Разгруппирует столбцы. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | Разгруппирует строки. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | Разгруппирует строки. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | Отображает скрытый столбец |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | Показать несколько столбцов. |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | Отображает строку. |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | Отображает скрытые строки. |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | Разъединяет указанный диапазон объединенных ячеек. |

### Примеры

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Установить высоту строки по умолчанию
cells.StandardHeight = 20;
//Установить высоту строки
cells.SetRowHeight(2, 20.5);

//Установить ширину столбца по умолчанию
cells.StandardWidth = 15;
//Установить ширину столбца
cells.SetColumnWidth(3, 12.57);

//Объединить ячейки
cells.Merge(5, 4, 2, 2);

//Помещаем значения в ячейки
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

//Экспорт данных
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Установить высоту строки по умолчанию
cells.StandardHeight = 20
'Установить высоту строки
cells.SetRowHeight(2, 20.5)

'Установить ширину столбца по умолчанию
cells.StandardWidth = 15
'Установить ширину столбца
cells.SetColumnWidth(3, 12.57)

'Объединить ячейки
cells.Merge(5, 4, 2, 2)

'Экспорт данных
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
