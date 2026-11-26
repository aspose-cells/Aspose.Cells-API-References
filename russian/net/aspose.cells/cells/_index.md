---
title: "Класс Cells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Cells class. Инкапсулирует коллекцию объектов, связанных с ячейками, таких как Cell Row ...etc"
type: docs
url: /ru/net/aspose.cells/cells/
---
## Cells class

Инкапсулирует коллекцию объектов, связанных с ячейками, таких как [`Cell`](../cell/), [`Row`](../row/), ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns/) { get; } | Получает коллекцию объектов [`Column`](../column/), представляющих отдельные столбцы в этом листе. |
| [Count](../../aspose.cells/cells/count/) { get; } | Получает общее количество созданных объектов Cell. |
| [CountLarge](../../aspose.cells/cells/countlarge/) { get; } | Получает общее количество созданных объектов Cell. |
| [FirstCell](../../aspose.cells/cells/firstcell/) { get; } | Получает первую ячейку в этом листе. |
| [IsDefaultColumnHidden](../../aspose.cells/cells/isdefaultcolumnhidden/) { get; set; } |  |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched/) { get; set; } | Указывает, что высота строки и высота шрифта по умолчанию совпадают. |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden/) { get; set; } | Указывает, скрыта ли строка по умолчанию. |
| [Item](../../aspose.cells/cells/item/) { get; } | Получает элемент [`Cell`](../cell/) по указанному индексу строки ячейки и индексу столбца. (2 индексатора) |
| [LastCell](../../aspose.cells/cells/lastcell/) { get; } | Получает последнюю ячейку в этом листе. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn/) { get; } | Максимальный индекс столбца среди ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка в нём не создана). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn/) { get; } | Максимальный индекс столбца ячейки, содержащей данные. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow/) { get; } | Максимальный индекс строки ячейки, содержащей данные. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange/) { get; } | Получает максимальный диапазон, включающий данные, объединённые ячейки и фигуры. |
| [MaxRow](../../aspose.cells/cells/maxrow/) { get; } | Максимальный индекс строки ячейки, содержащей данные или стиль. |
| [MemorySetting](../../aspose.cells/cells/memorysetting/) { get; set; } | Получает или задает параметр использования памяти для этих ячеек. |
| [MergedCells](../../aspose.cells/cells/mergedcells/) { get; } | (**Obsolete.**) Получает коллекцию объединённых ячеек. |
| [MinColumn](../../aspose.cells/cells/mincolumn/) { get; } | Минимальный индекс столбца среди ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка в нём не создана). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn/) { get; } | Минимальный индекс столбца ячейки, содержащей данные. |
| [MinDataRow](../../aspose.cells/cells/mindatarow/) { get; } | Минимальный индекс строки ячейки, содержащей данные. |
| [MinRow](../../aspose.cells/cells/minrow/) { get; } | Минимальный индекс строки ячейки, содержащей данные или стиль. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading/) { get; set; } | Получает или задает, должна ли модель данных ячеек поддерживать многопоточное чтение. Значение по умолчанию этого свойства — false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields/) { get; } | Получает список полей ods. |
| [PreserveString](../../aspose.cells/cells/preservestring/) { get; set; } | Получает или задает значение, указывающее, сохраняются ли все значения листа как строки. По умолчанию — false. |
| [Ranges](../../aspose.cells/cells/ranges/) { get; } | Получает коллекцию объектов [`Range`](../range/), созданных во время выполнения. |
| [Rows](../../aspose.cells/cells/rows/) { get; } | Получает коллекцию объектов [`Row`](../row/), представляющих отдельные строки на этом листе. |
| [StandardHeight](../../aspose.cells/cells/standardheight/) { get; set; } | Получает или задает высоту строки по умолчанию в этом листе, в единицах пунктов. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch/) { get; set; } | Получает или задает высоту строки по умолчанию в этом листе, в единицах дюймов. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels/) { get; set; } | Получает или задает высоту строки по умолчанию в этом листе, в единицах пикселей. |
| [StandardWidth](../../aspose.cells/cells/standardwidth/) { get; set; } | Получает или задает ширину столбца по умолчанию в листе, в единицах символов. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch/) { get; set; } | Получает или задает ширину столбца по умолчанию в листе, в единицах дюймов. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels/) { get; set; } | Получает или задает ширину столбца по умолчанию в листе, в единицах пикселей. |
| [Style](../../aspose.cells/cells/style/) { get; set; } | Получает и задает стиль по умолчанию листа. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange/)(Range) | Добавляет ссылку на объект диапазона в ячейки |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle/)(int, Style, StyleFlag) | Применяет форматы ко всему столбцу. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle/)(int, Style, StyleFlag) | Применяет форматы к целой строке. |
| [ApplyStyle](../../aspose.cells/cells/applystyle/)(Style, StyleFlag) | Применяет форматы ко всему листу. |
| [CheckCell](../../aspose.cells/cells/checkcell/)(int, int) | Получает элемент [`Cell`](../cell/) или null по указанному индексу строки ячейки и индексу столбца. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn/)(int) | Получает элемент [`Column`](../column/) или null по указанному индексу столбца. |
| [CheckRow](../../aspose.cells/cells/checkrow/)(int) | Получает элемент [`Row`](../row/) или null по указанному индексу строки ячейки. |
| [Clear](../../aspose.cells/cells/clear/)() | Очищает все данные листа. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents)(CellArea) | Очищает содержимое диапазона. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents_1)(int, int, int, int) | Очищает содержимое диапазона. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats)(CellArea) | Очищает форматирование диапазона. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats_1)(int, int, int, int) | Очищает форматирование диапазона. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells/)() | Очищает все объединённые диапазоны. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange)(CellArea) | Очищает содержимое и форматирование диапазона. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange_1)(int, int, int, int) | Очищает содержимое и форматирование диапазона. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue/)() | Преобразует все строковые данные в листе в числовое значение, если это возможно. |
| [CopyColumn](../../aspose.cells/cells/copycolumn/)(Cells, int, int) | Копирует данные и форматы целого столбца. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns)(Cells, int, int, int) | Копирует данные и форматы целых столбцов. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_2)(Cells, int, int, int, int) | Копирует данные и форматы всех столбцов. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_1)(Cells, int, int, int, PasteOptions) | Копирует данные и форматы целого столбца. |
| [CopyRow](../../aspose.cells/cells/copyrow/)(Cells, int, int) | Копирует данные и форматы целой строки. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows)(Cells, int, int, int) | Копирует данные и форматы некоторых целых строк. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_1)(Cells, int, int, int, CopyOptions) | Копирует данные и форматы некоторых целых строк. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Копирует данные и форматы некоторых целых строк. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_2)(string) | Создает объект [`Range`](../range/) из адреса диапазона. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_3)(string, string) | Создаёт объект [`Range`](../range/) из диапазона ячеек. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange)(int, int, bool) | Создаёт объект [`Range`](../range/) из строк ячеек или столбцов ячеек. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_1)(int, int, int, int) | Создаёт объект [`Range`](../range/) из диапазона ячеек. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns)() | Удаляет все пустые столбцы, которые не содержат никаких данных. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns_1)(DeleteOptions) | Удаляет все пустые столбцы, которые не содержат никаких данных. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows)() | Удаляет все пустые строки, которые не содержат никаких данных или других объектов. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows_1)(DeleteOptions) | Удаляет все пустые строки, которые не содержат никаких данных или некоторых специальных объектов, таких как видимый комментарий, сводная таблица. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn)(int) | Удаляет столбец. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn_1)(int, bool) | Удаляет столбец. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns_1)(int, int, bool) | Удаляет несколько столбцов. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns)(int, int, DeleteOptions) | Удаляет несколько столбцов. |
| [DeleteRange](../../aspose.cells/cells/deleterange/)(int, int, int, int, ShiftType) | Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow)(int) | Удаляет строку. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow_1)(int, bool) | Удаляет строку. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows)(int, int) | Удаляет несколько строк. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_2)(int, int, bool) | Удаляет несколько строк в листе. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_1)(int, int, DeleteOptions) | Удаляет несколько строк в листе. |
| [Dispose](../../aspose.cells/cells/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn)(int) | Получает последнюю ячейку в этом столбце. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn_1)(int, int, int, int) | Получает последнюю ячейку с максимальным индексом столбца в этом диапазоне. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow)(int) | Получает последнюю ячейку в этой строке. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow_1)(int, int, int, int) | Получает последнюю ячейку с максимальным индексом строки в этом диапазоне. |
| [ExportArray](../../aspose.cells/cells/exportarray/)(int, int, int, int) | Экспортирует данные из коллекции `Cells` в объект двумерного массива. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable)(int, int, int, int) | Экспортирует данные из коллекции `Cells` в объект DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_2)(int, int, int, int, bool) | Экспортирует данные из коллекции `Cells` в объект DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Экспортирует данные из коллекции `Cells` в объект DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring)(int, int, int, int) | Экспортирует данные из коллекции `Cells` в объект DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring_1)(int, int, int, int, bool) | Экспортирует данные из коллекции `Cells` в объект DataTable. |
| [ExportList&lt;T&gt;](../../aspose.cells/cells/exportlist/)(int, int, int, int, ExportTableOptions) |  |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray/)(int, int, int, int) | Экспортирует тип значения ячейки из коллекции `Cells` в объект двумерного массива. |
| [Find](../../aspose.cells/cells/find/#find)(object, Cell) | Находит ячейку, содержащую входной объект. |
| [Find](../../aspose.cells/cells/find/#find_1)(object, Cell, FindOptions) | Находит ячейку, содержащую входной объект. |
| [GetCell](../../aspose.cells/cells/getcell/)(int, int) | (**Obsolete.**) Получает элемент [`Cell`](../cell/) или null по указанному индексу строки ячейки и индексу столбца. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle)(int, int) | Получить стиль отображения заданной ячейки. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle_1)(int, int, BorderType) | Получить стиль отображения заданной ячейки. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle/)(int, int) | Получить стиль заданной ячейки. |
| [GetCellsWithPlaceInCellPicture](../../aspose.cells/cells/getcellswithplaceincellpicture/)() | Получает все ячейки, содержащие встроенное изображение. |
| [GetColumnOriginalWidthPoint](../../aspose.cells/cells/getcolumnoriginalwidthpoint/)(int) | (**Obsolete.**) Получает исходную высоту столбца в пунктах, если столбец скрыт. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth)(int) | Получает ширину (в единицах символов) указанного столбца в обычном виде. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth_1)(int, bool, CellsUnitType) | Получает ширину столбца. |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch/)(int) | (**Obsolete.**) Получает ширину указанного столбца в обычном виде, в единицах дюймов. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel)(int) | Получает ширину указанного столбца в обычном виде, в единицах пикселей. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel_1)(int, bool) | (**Obsolete.**) Получает ширину указанного столбца в обычном виде, в единицах пикселей. |
| [GetDependents](../../aspose.cells/cells/getdependents/)(bool, int, int) | Получить все ячейки, которые ссылаются на конкретную ячейку. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation/)(int, int, bool) | Получает все ячейки, результат вычисления которых зависит от конкретной ячейки. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator/)() | Получает перечислитель ячеек. |
| [GetFirstDataRow](../../aspose.cells/cells/getfirstdatarow/)(int) | Получает индекс первой строки ячейки, содержащей данные в указанном столбце. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel/)(int) | Получает уровень структуры (нумерация с нуля) столбца. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel/)(int) | Получает уровень структуры (нумерация с нуля) строки. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow/)(int) | Получает индекс последней строки ячейки, содержащей данные в указанном столбце. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/)() | Получает максимальный уровень структуры сгруппированных столбцов (нумерация с нуля). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel/)() | Получает максимальный уровень структуры сгруппированных строк (нумерация с нуля). |
| [GetMergedAreas](../../aspose.cells/cells/getmergedareas/)() | Получает все объединённые ячейки. |
| [GetRow](../../aspose.cells/cells/getrow/)(int) | (**Obsolete.**) Получает элемент [`Row`](../row/) по указанному индексу строки ячейки. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator/)() | (**Obsolete.**) Получает перечислитель строк. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight)(int) | Получает высоту указанной строки в пунктах. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight_1)(int, bool, CellsUnitType) | Получает высоту строки. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch/)(int) | Получает высоту указанной строки в дюймах. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel/)(int) | Получает высоту указанной строки в пикселях. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint/)(int) | (**Obsolete.**) Получает исходную высоту строки в пунктах, если строка скрыта |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel/)(int) | Получает ширину в разных типах представления. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight/)(int) | Получает высоту указанной строки. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch/)(int) | Получает высоту указанной строки в дюймах. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns)(int, int) | Группирует столбцы. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns_1)(int, int, bool) | Группирует столбцы. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows)(int, int) | Группирует строки. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows_1)(int, int, bool) | Группирует строки. |
| [HideColumn](../../aspose.cells/cells/hidecolumn/)(int) | Скрывает столбец. |
| [HideColumns](../../aspose.cells/cells/hidecolumns/)(int, int) | Скрывает несколько столбцов. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail/)(bool, int) | Сворачивает сгруппированные строки/столбцы. |
| [HideRow](../../aspose.cells/cells/hiderow/)(int) | Скрывает строку. |
| [HideRows](../../aspose.cells/cells/hiderows/)(int, int) | Скрывает несколько строк. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_1)(double[], int, int, bool) | Импортирует массив double в рабочий лист. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_3)(int[], int, int, bool) | Импортирует массив integer в рабочий лист. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_5)(string[], int, int, bool) | Импортирует массив string в рабочий лист. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist/)(ArrayList, int, int, bool) | Импортирует ArrayList данных в рабочий лист. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv)(Stream, TxtLoadOptions, int, int) | Импортирует CSV‑файл в ячейки. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_2)(string, TxtLoadOptions, int, int) | Импортирует CSV‑файл в ячейки. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_1)(Stream, string, bool, int, int) | Импортирует CSV‑файл в ячейки. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_3)(string, string, bool, int, int) | Импортирует CSV‑файл в ячейки. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Импортирует пользовательские объекты. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Импортирует пользовательские объекты. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_3)(IDataReader, int, int) | Импортирует данные из объекта IDataReader. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_1)(DataTable, int, int, ImportTableOptions) | Импортирует данные из пользовательской таблицы данных. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_2)(DataView, int, int, ImportTableOptions) | Импортирует данные из представления данных. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Импортирует данные из пользовательской таблицы данных. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_4)(IDataReader, int, int, ImportTableOptions) | Импортирует данные из объекта IDataReader. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid)(DataGrid, int, int, bool) | Импортирует DataGrid в рабочий лист. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Импортирует DataGrid в рабочий лист. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Импортирует DataGrid в рабочий лист. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring/)(DataGrid, int, int, bool) | Импортирует DataGrid в рабочий лист. Этот метод не пытается преобразовать текст в числовые значения. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow/)(DataRow, int, int) | Импортирует DataRow в файл Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview/)(DataView, int, int) | Импортирует DataView в рабочий лист. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray/)(string[], int, int, bool) | Импортирует массив формул в рабочий лист. |
| [ImportGridView](../../aspose.cells/cells/importgridview/)(GridView, int, int, ImportTableOptions) | Импортирует представление сетки в эти ячейки. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray)(object[], int, int, bool) | Импортирует массив данных в лист. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray_1)(object[], int, int, bool, int) | Импортирует массив данных в лист. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn)(int) | Вставляет новый столбец в лист. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn_1)(int, bool) | Вставляет новый столбец в лист. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns)(int, int) | Вставляет несколько столбцов в лист. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_2)(int, int, bool) | Вставляет несколько столбцов в лист. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_1)(int, int, InsertOptions) | Вставляет несколько столбцов в лист. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells/)(Range, int, int, ShiftType) | Вставить вырезанный диапазон. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange)(CellArea, ShiftType) | Вставляет диапазон ячеек и смещает ячейки в соответствии с параметром смещения. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_1)(CellArea, int, ShiftType) | Вставляет диапазон ячеек и смещает ячейки в соответствии с параметром смещения. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_2)(CellArea, int, ShiftType, bool) | Вставляет диапазон ячеек и смещает ячейки в соответствии с параметром смещения. |
| [InsertRow](../../aspose.cells/cells/insertrow/)(int) | Вставляет новую строку в лист. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows)(int, int) | Вставляет несколько строк в лист. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_2)(int, int, bool) | Вставляет несколько строк в лист. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_1)(int, int, InsertOptions) | Вставляет несколько строк в лист. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn/)(int) | Проверяет, является ли указанный столбец пустым (не содержит данных). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden/)(int) | Проверяет, скрыт ли столбец с указанным индексом. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled/)(int, int, int, int) | Проверьте, можно ли удалить диапазон. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden/)(int) | Проверяет, скрыта ли строка с указанным индексом. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap/)(string, int, int, string) | Ссылка на XML-карту. |
| [Merge](../../aspose.cells/cells/merge/#merge)(int, int, int, int) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [Merge](../../aspose.cells/cells/merge/#merge_1)(int, int, int, int, bool) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [Merge](../../aspose.cells/cells/merge/#merge_2)(int, int, int, int, bool, bool) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [MoveRange](../../aspose.cells/cells/moverange/)(CellArea, int, int) | Перемещает диапазон. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates)() | Удаляет дублирующиеся строки в листе. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_1)(int, int, int, int) | Удаляет дублирующиеся значения в диапазоне. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_2)(int, int, int, int, bool, int[]) | Удаляет дублирующиеся данные диапазона. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas/)() | Удаляет все формулы и заменяет их значением формулы. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting/)(CellArea) | Получает настройки промежуточных итогов диапазона. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth/)(int, double) | Устанавливает ширину указанного столбца в обычном виде. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch/)(int, double) | Устанавливает ширину столбца в дюймах в обычном виде. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel/)(int, int) | Устанавливает ширину столбца в пикселях в обычном виде. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight/)(int, double) | Устанавливает высоту указанной строки. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch/)(int, double) | Устанавливает высоту строки в дюймах. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel/)(int, int) | Устанавливает высоту строки в пикселях. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel/)(int, int) | Устанавливает ширину столбца в разных представлениях. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail/)(bool, int) | Разворачивает сгруппированные строки/столбцы. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Создаёт промежуточные итоги для диапазона. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Создаёт промежуточные итоги для диапазона. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns/)(int, int, int, TxtLoadOptions) | Разделяет содержимое указанного столбца на несколько столбцов.. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns/)(int, int) | Разгруппирует столбцы. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows)(int, int) | Разгруппирует строки. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows_1)(int, int, bool) | Разгруппирует строки. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn/)(int, double) | Отображает скрытый столбец |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns/)(int, int, double) | Отображает несколько скрытых столбцов. |
| [UnhideRow](../../aspose.cells/cells/unhiderow/)(int, double) | Отображает скрытую строку. |
| [UnhideRows](../../aspose.cells/cells/unhiderows/)(int, int, double) | Отображает скрытые строки. |
| [UnMerge](../../aspose.cells/cells/unmerge/)(int, int, int, int) | Разъединяет указанный диапазон объединённых ячеек. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDemo
    {
        public static void CellsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить высоту строки по умолчанию
            cells.StandardHeight = 20;
            // Установить высоту строки
            cells.SetRowHeight(2, 20.5);

            // Установить ширину столбца по умолчанию
            cells.StandardWidth = 15;
            // Установить ширину столбца
            cells.SetColumnWidth(3, 12.57);

            // Объединить ячейки
            cells.Merge(5, 4, 2, 2);

            // Записать значения в ячейки
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue("abc");

            // Экспортировать данные
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // Продемонстрировать некоторые свойства
            Console.WriteLine("Total Cells Count: " + cells.Count);
            Console.WriteLine("Total Cells Count (Large): " + cells.CountLarge);
            Console.WriteLine("Min Row with Data: " + cells.MinDataRow);
            Console.WriteLine("Max Row with Data: " + cells.MaxDataRow);
            Console.WriteLine("Min Column with Data: " + cells.MinDataColumn);
            Console.WriteLine("Max Column with Data: " + cells.MaxDataColumn);

            // Перебрать ячейки
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Сохраните книгу
            workbook.Save("CellsExample.xlsx");
            workbook.Save("CellsExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


