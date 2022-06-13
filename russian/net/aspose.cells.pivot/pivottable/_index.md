---
title: PivotTable
second_title: Справочник по Aspose.Cells для .NET API
description: Краткое описание сводной таблицы.
type: docs
weight: 4690
url: /ru/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Краткое описание сводной таблицы.

```csharp
public class PivotTable : IDisposable
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | Получает описание альтернативного текста |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | Получает заголовок альтертекста |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | Получает тип автоматического форматирования сводной таблицы. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | Возвращает объект PivotFields, включающий все поля отчета сводной таблицы |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | Возвращает объект PivotFields, который в данный момент отображается как поля столбца. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | Указывает, отображаются ли в отчете сводной таблицы общие итоги для столбцов. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | Получает заголовок заголовка столбца сводной таблицы. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | Возвращает объект CellArea, который представляет диапазон , содержащий область столбца в отчете сводной таблицы. Только для чтения. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | Указывает, следует ли учитывать встроенный пользовательский список при сортировке данных |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | Возвращает объект CellArea, представляющий диапазон, содержащий область данных в списке между строкой заголовка и строкой вставки. Только для чтения. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | Получает объект PivotField, представляющий все поля данных в сводной таблице. Только для чтения. Он будет инициализирован только при наличии двух или более полей данных в DataPiovtFiels. Он используется только для добавления DataPivotField в область строк/столбцов сводной таблицы. По умолчанию находится в области строк. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | Получает объект PivotField, представляющий все поля данных в сводной таблице. Только для чтения. Он будет инициализирован только при наличии двух или более полей данных в DataPiovtFiels. Он используется только для добавления DataPivotField в область строк/столбцов сводной таблицы. По умолчанию находится в области строк. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | Получает и задает источник данных сводной таблицы. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих ошибки. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | Указывает, видны ли элементы в области строк и столбцов когда область данных сводной таблицы пуста. Значение по умолчанию верно. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих нулевые значения. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | Задает логическое значение, указывающее, разрешено ли пользователю редактировать ячейки в области данных сводной таблицы. Включить редактирование ячеек в области значений |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | Получает, включена ли детализация. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | Указывает, доступно ли диалоговое окно поля сводной таблицы когда пользователь дважды щелкает поле сводной таблицы. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | Получает, включает ли список полей для сводной таблицы. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | Указывает, доступен ли мастер сводных таблиц. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | Получает строку, отображаемую в ячейках, содержащих ошибки , когда свойство DisplayErrorString имеет значение true. Значение по умолчанию — пустая строка. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | Получает источник данных внешнего соединения. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | Задает логическое значение, указывающее, сортируются ли поля в сводной таблице в порядке, отличном от порядка по умолчанию в списке полей. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | Возвращает метку текстовой строки, которая отображается в заголовке столбца общей суммы или строки. Значением по умолчанию является строка "Общий итог". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | Указывает, добавлять ли пустые строки. Это свойство применяется только к типам автоматического форматирования сводной таблицы, которым необходимо добавлять пустые строки. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | Определяет приращение отступа для компактной оси и может использоваться для установки макета отчета в компактную форму. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | Указывает, форматируется ли отчет сводной таблицы автоматически. Флажок "автоформатировать таблицу", который находится в опции сводной таблицы для Excel 2003 Флажок "автоподбор ширины столбца при обновлении", который находится в сводной таблице Параметры:Формат макета для Excel 2007 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | Указывает, совместима ли сводная таблица с Excel2003 при обновлении сводной таблицы, если true, строка должна быть меньше или равна 255 символам, поэтому если строка больше 255 символов, она будет усечена. если false, строка не будет иметь вышеупомянутого ограничения. Значение по умолчанию — true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | Указывает, отображает ли отчет сводной таблицы классический макет сводной таблицы. (позволяет перетаскивать поля в сетке) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | Указывает логическое значение, указывающее, могут ли поля сводной таблицы иметь несколько фильтров, установленных для них. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | Указывает, выбрана ли сводная таблица. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | Бит, указывающий, повторяются ли заголовки элементов сводки на оси строк на каждой печатной странице для полей сводки в табличной форме. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | Указывает, пересчитывается ли отчет сводной таблицы только по запросу пользователя. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | Указывает, используют ли объединенные ячейки элемент внешней строки, элемент столбца, промежуточный итог, и общий итог указанного отчета сводной таблицы. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | Указывает логическое значение, указывающее, могут ли поля сводной таблицы иметь несколько фильтров, установленных для них. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | Получает имя сводной таблицы |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | Получает строку, отображаемую в ячейках, которые содержат нулевые значения , когда свойство DisplayNullString имеет значение true. Значение по умолчанию — пустая строка. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | Получает порядок, в котором поля страницы добавляются в макет отчета сводной таблицы. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | Возвращает объект PivotFields, который в данный момент отображается как поля страницы. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | Получает количество полей страницы в каждом столбце или строке отчета сводной таблицы. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | Возвращает объект PivotFilterCollection. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | Получает условия формата сводной таблицы. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | Получает и задает имя стиля сводной таблицы. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | Получает и задает встроенный стиль сводной таблицы. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | Указывает, сохраняется ли форматирование при обновлении или пересчете сводной таблицы. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | Задает логическое значение, указывающее, следует ли печатать индикаторы детализации. печатать кнопки развертывания/свертывания при отображении в сводной таблице. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | Указывает, установлены ли заголовки печати для рабочего листа на основе отчета сводной таблицы. Значение по умолчанию неверно. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | Указывает, следует ли обновлять данные или нет. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | Указывает, следует ли обновлять данные при открытии файла. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | Получает дату последнего обновления сводной таблицы. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | Получает имя пользователя, который последний раз обновлял сводную таблицу |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | Возвращает объект PivotFields, который в данный момент отображается как поля строк. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | Указывает, отображаются ли в отчете сводной таблицы общие итоги для строк. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | Получает заголовок строки сводной таблицы. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | Возвращает объект CellArea, который представляет диапазон , содержащий область строки в отчете сводной таблицы. Только для чтения. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | Указывает, сохраняются ли данные для отчета сводной таблицы вместе с рабочей книгой. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | Задает логическое значение, указывающее, следует ли отображать всплывающие подсказки для ячеек данных сводной таблицы. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | Получает, отображаются ли кнопки развертывания/свертывания. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | Задает логическое значение, указывающее, следует ли включать пустые столбцы в таблицу |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | Указывает логическое значение, указывающее, следует ли включать пустые строки в таблицу. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | Указывает логическое значение, указывающее, следует ли опускать сведения о свойствах элементов из всплывающих подсказок сводной таблицы. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | Указывает, следует ли применять стиль к заголовку столбца в сводной таблице. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | Указывает, применяется ли форматирование чередования столбцов. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | Указывает, применяется ли форматирование чередования столбцов. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | Указывает, следует ли применять стиль к заголовку строки в сводной таблице. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | Указывает, применяется ли форматирование чередования строк. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | Указывает, отображаются ли заголовки заголовков строк в отчете сводной таблицы Указывает, отображаются ли заголовки полей и раскрывающиеся списки фильтров |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | Указывает логическое значение, указывающее, показывать ли строку значений. показать строку значений |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | Указывает, включены ли элементы поля скрытой страницы в отчет сводной таблицы в промежуточные итоги по строкам и столбцам, итоги по блокам и общие итоги. Значение по умолчанию — False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет сводной таблицы, но не включающий поля страницы. Только для чтения. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет сводной таблицы, включая поля страницы. Только для чтения. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | Получает строку, сохраненную в отчете сводной таблицы. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | Добавляет вычисляемое поле в сводное поле и перетаскивает его в область данных. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | Добавляет вычисляемое поле в сводное поле. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | Добавляет поле в указанную область. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | Добавляет поле в указанную область. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | Добавляет поле в указанную область. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | Вычисляет данные сводной таблицы в ячейки. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | Вычисляет диапазон сводной таблицы. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | Установить исходные данные сводной таблицы. Лист1!$A$1:$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | Очистить данные и форматирование сводной таблицы |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | Копирует именованный стиль из другой сводной таблицы. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | Выполняет определяемые приложением задачи, связанные с освобождением, освобождением или сбросом неуправляемых ресурсов. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | Получает определенные поля по типу поля. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | Отформатировать ячейку в области сводной таблицы |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | Форматировать все ячейки в области сводной таблицы |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | Форматирование данных строки в области сводной таблицы |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | Получает объект Cell по DisplayName PivotField |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | Получает дочерние сводные таблицы, которые используют данные этой сводной таблицы в качестве источника данных. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | получить индекс строки сводной таблицы список горизонтальных разрывов страниц |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | Получить исходные данные сводной таблицы. |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | Перемещает сводную таблицу в другое место на листе. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | Перемещает сводную таблицу в другое место на листе. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | Обновляет данные сводной таблицы и настройки из ее источника данных. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | Удаляет поле из определенной области полей |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | Удалить поле из определенной области поля |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | Удаляет поле из определенной области полей |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | Устанавливает группу автоматических полей по сводной таблице. |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | Устанавливает группу автоматических полей по сводной таблице. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | Устанавливает вручную группу полей сводной таблицы. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | Устанавливает вручную группу полей сводной таблицы. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | Устанавливает вручную группу полей сводной таблицы. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | Устанавливает вручную группу полей сводной таблицы. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | Устанавливает разгруппировку по сводной таблице |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | Устанавливает разгруппировку по сводной таблице |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | Макеты сводной таблицы в компактной форме. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | Макет сводной таблицы в виде схемы. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | Макет сводной таблицы в виде таблицы. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | Показать все страницы фильтра отчета в соответствии с PivotField, PivotField должен находиться в PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | Показать все страницы фильтра отчета в соответствии с индексом позиции в PageFields |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | Показать все страницы фильтров отчетов в соответствии с именем PivotField, PivotField должен находиться в PageFields. |

### Примеры

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

  //Изменить атрибуты PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

  //Добавить PivotFilter
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

  //Добавить PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

  //делай свое дело

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Add PivotFilter
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Add PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Смотрите также

* пространство имен [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
