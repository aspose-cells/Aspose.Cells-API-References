---
title: "Класс PivotTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotTable. Краткое описание PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Краткое описание PivotTable.

```csharp
public class PivotTable : IDisposable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AllowMultipleFiltersPerField](../../aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/) { get; set; } | Указывает логическое значение, которое определяет, могут ли поля PivotTable иметь несколько установленных фильтров. |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription/) { get; set; } | Получает описание альтернативного текста. |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle/) { get; set; } | Получает и задает заголовок изменённого текста. |
| [AutofitColumnWidthOnUpdate](../../aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/) { get; set; } | Указывает, следует ли автоматически подгонять ширину столбца при обновлении |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype/) { get; set; } | Получает и задает тип автоматического форматирования PivotTable. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields/) { get; } | Возвращает все базовые поля сводной таблицы в PivotTable. |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields/) { get; } | Возвращает объект PivotFields, который в данный момент отображается как столбцовые поля. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand/) { get; set; } | (**Obsolete.**) Указывает, отображает ли отчет PivotTable общие итоги по столбцам. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption/) { get; set; } | Получает и задает пользовательскую подпись заголовка столбца PivotTable. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange/) { get; } | Возвращает объект CellArea, представляющий диапазон, содержащий область столбцов в отчете PivotTable. Только для чтения. |
| [ConditionalFormats](../../aspose.cells.pivot/pivottable/conditionalformats/) { get; } | Получает условные форматы сводной таблицы. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort/) { get; set; } | Указывает, следует ли учитывать встроенный пользовательский список при сортировке данных |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange/) { get; } | Возвращает объект [`CellArea`](../../aspose.cells/cellarea/), представляющий диапазон, содержащий область данных в списке между строкой заголовка и строкой вставки. Только для чтения. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield/) { get; } | (**Obsolete.**) Получает объект [`PivotField`](../pivotfield/), представляющий все поля данных в PivotTable. Только для чтения. Он будет создан только когда в области данных присутствует два или более полей данных. По умолчанию он находится в строковой области. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea(). |
| [DataFieldHeaderName](../../aspose.cells.pivot/pivottable/datafieldheadername/) { get; set; } | Получает и задает имя заголовка поля области значений в PivotTable. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields/) { get; } | Получает [`PivotFieldCollection`](../pivotfieldcollection/), представляющую все поля данных в PivotTable. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource/) { get; set; } | Получает и задает источник данных сводной таблицы. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring/) { get; set; } | Указывает, отображает ли отчет PivotTable пользовательскую строку в ячейках, содержащих ошибки. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems/) { get; set; } | Указывает, видимы ли элементы в областях строк и столбцов, когда область данных PivotTable пуста. Значение по умолчанию — true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring/) { get; set; } | Указывает, отображает ли отчет PivotTable пользовательскую строку, если значение равно null. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting/) { get; set; } | Указывает логическое значение, определяющее, разрешено ли пользователю редактировать ячейки в области данных pivottable. Значение по умолчанию — false. |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown/) { get; set; } | Указывает, включено ли раскрытие (drilldown). |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog/) { get; set; } | Указывает, доступно ли диалоговое окно поля сводной таблицы, когда пользователь дважды щёлкает поле сводной таблицы. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist/) { get; set; } | Указывает, доступен ли список полей для сводной таблицы в представлении Excel. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard/) { get; set; } | Указывает, доступен ли мастер сводных таблиц. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring/) { get; set; } | Получает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString равно true. Значение по умолчанию — пустая строка. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource/) { get; } | (**Obsolete.**) Получает внешний источник данных соединения. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending/) { get; set; } | Указывает, отсортированы ли поля в сводной таблице в порядке, отличном от стандартного, в списке полей. |
| [FilterArea](../../aspose.cells.pivot/pivottable/filterarea/) { get; } | Получает область региона фильтра. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname/) { get; set; } | Возвращает метку, отображаемую в заголовке столбца или строки общей суммы. Значение по умолчанию — строка "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows/) { get; set; } | (**Obsolete.**) Указывает, следует ли добавлять пустые строки. Это свойство применяется только к типам автоформатирования сводных таблиц, которым необходимо добавлять пустые строки. |
| [Indent](../../aspose.cells.pivot/pivottable/indent/) { get; set; } | Задает шаг отступа для компактной оси и может использоваться для установки макета отчёта в компактную форму. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat/) { get; set; } | Указывает, автоматически ли форматируется отчёт сводной таблицы. Флажок "autoformat table", который находится в параметрах сводной таблицы для Excel 2003. |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible/) { get; set; } | Указывает, совместима ли сводная таблица с Excel2003 при её обновлении; если true, строка должна быть длиной не более 255 символов, иначе будет усечена. Если false, ограничение не применяется. Значение по умолчанию — true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones/) { get; set; } | Указывает, отображает ли отчёт сводной таблицы классический макет сводной таблицы. (включает перетаскивание полей в сетке) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters/) { get; set; } | (**Obsolete.**) Задает логическое значение, указывающее, могут ли поля сводной таблицы иметь несколько фильтров. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected/) { get; set; } | Указывает, выбрана ли эта сводная таблица. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles/) { get; set; } | (**Obsolete.**) Указывает, должны ли имена PivotItem повторяться в верхней части каждой печатной страницы. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate/) { get; set; } | Указывает, пересчитывается ли отчёт сводной таблицы только по запросу пользователя. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels/) { get; set; } | Получает или задаёт, следует ли объединять подписи полей строк/столбцов, охватывающие несколько ячеек. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit/) { get; set; } | (**Obsolete.**) Задает логическое значение, указывающее, могут ли поля сводной таблицы иметь несколько фильтров. |
| [Name](../../aspose.cells.pivot/pivottable/name/) { get; set; } | Получает имя сводной таблицы |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring/) { get; set; } | Получает строку, отображаемую в ячейках, содержащих null‑значения, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder/) { get; set; } | Получает и задаёт порядок, в котором поля страниц добавляются в макет отчёта сводной таблицы. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields/) { get; } | Возвращает [`PivotFieldCollection`](../pivotfieldcollection/), которые в данный момент отображаются как поля страниц. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount/) { get; set; } | Получает количество полей страниц в каждом столбце или строке отчёта сводной таблицы. |
| [PivotCache](../../aspose.cells.pivot/pivottable/pivotcache/) { get; } | Получает источник данных. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters/) { get; } | Возвращает все фильтры в сводной таблице. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions/) { get; } | (**Obsolete.**) Получает условия форматирования сводной таблицы. |
| [PivotFormats](../../aspose.cells.pivot/pivottable/pivotformats/) { get; } | Получает все форматы ячеек, применённые к этой сводной таблице. |
| [PivotTableStyle](../../aspose.cells.pivot/pivottable/pivottablestyle/) { get; set; } | Получает настройки TableStyle этой сводной таблицы. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename/) { get; set; } | Получает или задаёт имя стиля сводной таблицы. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype/) { get; set; } | Получает и задаёт встроенный стиль сводной таблицы. |
| [PreserveCellFormattingOnUpdate](../../aspose.cells.pivot/pivottable/preservecellformattingonupdate/) { get; set; } | Указывает, следует ли сохранять форматирование ячеек ([`PivotTableFormat`](../pivottableformat/)) при обновлении или перерасчёте сводной таблицы. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting/) { get; set; } | (**Obsolete.**) Указывает, сохраняется ли форматирование ячеек ([`PivotTableFormat`](../pivottableformat/)) при обновлении или перерасчёте PivotTable. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill/) { get; set; } | Задаёт логическое значение, указывающее, следует ли печатать индикаторы drill. Печать кнопок раскрытия/сворачивания при отображении в pivottable. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles/) { get; set; } | Указывает, устанавливаются ли заголовки печати для листа на основе отчёта PivotTable. Значение по умолчанию — false. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile/) { get; set; } | Указывает, следует ли обновлять данные при открытии файла. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate/) { get; } | Получает дату и время последнего обновления PivotTable. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho/) { get; } | Получает имя последнего пользователя, который обновил эту PivotTable. |
| [RepeatItemsOnEachPrintedPage](../../aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/) { get; set; } | Указывает, повторяются ли подписи элементов сводной таблицы в области строк на каждой печатной странице для полей сводной таблицы в табличной форме. |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields/) { get; } | Возвращает [`PivotFieldCollection`](../pivotfieldcollection/), которые в настоящее время отображаются как поля строк. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand/) { get; set; } | (**Obsolete.**) Указывает, следует ли показывать общие итоги для строк этой сводной таблицы. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption/) { get; set; } | Получает и задаёт пользовательскую подпись заголовка строки в этой PivotTable. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange/) { get; } | Возвращает объект CellArea, представляющий диапазон, содержащий область строк в отчёте PivotTable. Только для чтения. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata/) { get; set; } | Указывает, сохраняются ли данные отчёта PivotTable вместе с рабочей книгой. |
| [ShowColumnGrandTotals](../../aspose.cells.pivot/pivottable/showcolumngrandtotals/) { get; set; } | Указывает, следует ли показывать общие итоги для столбцов этой сводной таблицы. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips/) { get; set; } | Указывает, следует ли отображать подсказки для ячеек данных PivotTable. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill/) { get; set; } | Получает и задаёт, показывать ли кнопки раскрытия/сворачивания. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol/) { get; set; } | Указывает, включать ли пустые столбцы в таблицу. |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow/) { get; set; } | Указывает, включать ли пустые строки в таблицу. |
| [ShowHeaders](../../aspose.cells.pivot/pivottable/showheaders/) { get; set; } | Показывать ли подписи полей данных и подписи полей сводной таблицы по оси строк и оси столбцов в представлении PivotTable. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips/) { get; set; } | Задаёт логическое значение, указывающее, следует ли опустить информацию о свойствах членов из подсказок PivotTable. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader/) { get; set; } | Указывает, следует ли применять стиль к заголовку столбца в сводной таблице. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/) { get; set; } | Указывает, применяется ли чередующееся форматирование для столбца. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn/) { get; set; } | Указывает, применяется ли форматирование столбца. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader/) { get; set; } | Указывает, следует ли применять стиль к заголовку строки в сводной таблице. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes/) { get; set; } | Указывает, применяется ли чередующееся форматирование строк. |
| [ShowRowGrandTotals](../../aspose.cells.pivot/pivottable/showrowgrandtotals/) { get; set; } | Указывает, показывать ли общие итоги для строк сводной таблицы. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption/) { get; set; } | (**Устарело.**) Указывает, отображается ли подпись заголовка строки в отчете PivotTable. Указывает, отображать ли подписи полей отображения и выпадающие списки фильтров. |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow/) { get; set; } | Указывает, показывать ли строку значений. |
| [SourceType](../../aspose.cells.pivot/pivottable/sourcetype/) { get; } | Получает тип источника данных сводной таблицы. |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems/) { get; set; } | Указывает, включаются ли скрытые элементы полей страниц в отчете PivotTable в промежуточные итоги по строкам и столбцам, блоковые итоги и общие итоги. Значение по умолчанию — False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1/) { get; } | Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет PivotTable, но без полей страниц. Только для чтения. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2/) { get; } | Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет PivotTable, включая поля страниц. Только для чтения. |
| [Tag](../../aspose.cells.pivot/pivottable/tag/) { get; set; } | Получает и задает пользовательскую строку, связанную с этим представлением PivotTable. |
| [TopRightArea](../../aspose.cells.pivot/pivottable/toprightarea/) { get; } | Представляет пустую область в правом верхнем углу PivotTable (в левом верхнем углу для листов RTL). |
| [ValuesField](../../aspose.cells.pivot/pivottable/valuesfield/) { get; } | Получает объект [`PivotField`](../pivotfield/), представляющий все поля данных в PivotTable. Только для чтения. Он будет создан только когда в области данных присутствует два или более полей данных. По умолчанию он находится в области строк. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea(). |

## Методы

| Имя | Описание |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield)(string, string) | Добавляет вычисляемое поле к полю сводной таблицы и перетаскивает его в область данных. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield_1)(string, string, bool) | Добавляет вычисляемое поле к полю сводной таблицы. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_1)(PivotFieldType, int) | Добавляет поле в указанную область. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea)(PivotFieldType, PivotField) | Добавляет поле в указанную область. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_2)(PivotFieldType, string) | Добавляет поле в указанную область. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata_1)() | Вычисляет данные сводной таблицы в ячейки. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata)(PivotTableCalculateOption) | Вычисляет сводную таблицу с параметрами. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange/)() | Вычисляет диапазон сводной таблицы. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource/)(string[]) | Изменить источник данных сводной таблицы. |
| [ClearAll](../../aspose.cells.pivot/pivottable/clearall/)() | Удалить все поля из областей. |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata/)() | Очистить данные и форматирование представления PivotTable. |
| [ClearFilters](../../aspose.cells.pivot/pivottable/clearfilters/)() | Очищает все фильтры этой сводной таблицы. |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle/)(PivotTable) | Копирует именованный стиль из другой сводной таблицы. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExportViewToJson](../../aspose.cells.pivot/pivottable/exportviewtojson/)(PivotViewToJsonOptions) | Экспортирует представление сводной таблицы в формате JSON. |
| [Fields](../../aspose.cells.pivot/pivottable/fields/)(PivotFieldType) | (**Obsolete.**) Получает конкретные поля по типу поля. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format)(CellArea, Style) | Форматирует выбранную область сводной таблицы. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_1)(PivotArea, Style) | Форматирует выбранную область сводной таблицы. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_2)(int, int, Style) | Форматирует ячейку в области сводной таблицы |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall/)(Style) | Форматирует все ячейки в области сводной таблицы |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow/)(int, Style) | Форматирует данные строк в области сводной таблицы |
| [GetButtonArea](../../aspose.cells.pivot/pivottable/getbuttonarea/)(PivotFieldType) | Получает область, содержащую кнопку поля. |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname/)(string) | Получает объект [`Cell`](../../aspose.cells/cell/) по отображаемому имени PivotField. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren/)() | (**Obsolete.**) Получает дочерние сводные таблицы, использующие данные этой сводной таблицы в качестве источника данных. |
| [GetDependentPivotTables](../../aspose.cells.pivot/pivottable/getdependentpivottables/)() | Получает все `PivotTable`s, использующие эту сводную таблицу в качестве источника данных. |
| [GetFields](../../aspose.cells.pivot/pivottable/getfields/)(PivotFieldType) | Получает конкретный список полей сводной таблицы по региону. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks/)() | (**Obsolete.**) Получает список индексов строк сводной таблицы горизонтальных разрывов страниц |
| [GetHorizontalPageBreaks](../../aspose.cells.pivot/pivottable/gethorizontalpagebreaks/)() | Получает горизонтальные разрывы страниц этой сводной таблицы. |
| [GetNamesOfSourceDataConnections](../../aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/)() | Получает имена внешних соединений источников данных. |
| [GetPivotTablesWithSamePivotCache](../../aspose.cells.pivot/pivottable/getpivottableswithsamepivotcache/)() | Получает все сводные таблицы с тем же кэшем сводных данных. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource)() | Получить источник данных этой сводной таблицы. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource_1)(bool) | Получить источник данных этой сводной таблицы. |
| [GetSourceDataConnections](../../aspose.cells.pivot/pivottable/getsourcedataconnections/)() | Получает внешние источники данных соединения. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move_1)(string) | (**Obsolete.**) Перемещает сводную таблицу в другое место листа. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move)(int, int) | (**Obsolete.**) Перемещает сводную таблицу в другое место листа. |
| [MoveItem](../../aspose.cells.pivot/pivottable/moveitem/)(PivotFieldType, string[], bool, int) | Переместить один элемент вверх или вниз. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_2)(string) | Перемещает сводную таблицу в другое место листа. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto)(int, int) | Перемещает сводную таблицу в другое место листа. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_1)(int, int, int) | Перемещает сводную таблицу в другое место листа. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh)() | Обновить [`PivotCache`](./pivotcache/) из источника данных и вычислить данные и стиль для представления сводной таблицы. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh_1)(PivotTableRefreshOption) | Обновить [`PivotCache`](./pivotcache/) из источника данных и вычислить данные и стиль для представления сводной таблицы. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata)() | (**Obsolete.**) Обновляет данные из его источника данных в кэш сводных таблиц. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata_1)(PivotTableRefreshOption) | (**Obsolete.**) Обновляет данные и настройки сводной таблицы из его источника данных с параметрами. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_1)(PivotFieldType, int) | Удаляет поле из конкретного региона сводной таблицы. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield)(PivotFieldType, PivotField) | Удалить поле из конкретной области полей |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_2)(PivotFieldType, string) | Удаляет поле из конкретной области полей |
| [SelectArea](../../aspose.cells.pivot/pivottable/selectarea/)(CellArea) | Выберите область представления сводной таблицы. |
| [ShowDetail](../../aspose.cells.pivot/pivottable/showdetail/)(int, int, bool, int, int) | Покажите детали одного элемента в области данных в новой таблице. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform/)() | Отображает представление сводной таблицы в компактной форме. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform/)() | Отображает сводную таблицу в виде схемы. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform/)() | Отображает сводную таблицу в табличной форме. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage/)(PivotField) | Покажите все страницы фильтра отчёта в соответствии с PivotField, PivotField должен находиться в PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex/)(int) | Покажите все страницы фильтра отчёта в соответствии с индексом позиции в PageFields. |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname/)(string) | Покажите все страницы фильтра отчёта в соответствии с именем PivotField, PivotField должен находиться в PageFields. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotTableDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Установить примерные данные
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Создать сводную таблицу
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];

            // Добавить поля
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Оформить сводную таблицу
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Настроить строковое поле
            PivotField rowField = pivot.RowFields[0];
            rowField.DisplayName = "Fruit Category";

            // Обновить и вычислить данные
            pivot.RefreshData();
            pivot.CalculateData();

            // Сохраните книгу
            book.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


