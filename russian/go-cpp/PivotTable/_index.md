---
title: "PivotTable Класс"
linktitle: "PivotTable"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "PivotTable класс. Инкапсулирует объект, представляющий pivottable в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivottable/
---

## PivotTable class

Краткое описание PivotTable.

```go

type PivotTable struct  {
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
| [Dispose](./dispose/) | Выполняет задачи, определённые приложением, связанные с освобождением, выпуском или сбросом неуправляемых ресурсов. |
| [GetPivotCache](./getpivotcache/) | Получает источник данных. |
| [IsExcel2003Compatible](./isexcel2003compatible/) | Указывает, совместима ли PivotTable с Excel2003 при обновлении PivotTable; если true, строка должна быть длиной не более 255 символов, поэтому если строка превышает 255 символов, она будет усечена. Если false, строка не будет иметь указанного ограничения. Значение по умолчанию — true. |
| [SetIsExcel2003Compatible](./setisexcel2003compatible/) | Указывает, совместима ли PivotTable с Excel2003 при обновлении PivotTable; если true, строка должна быть длиной не более 255 символов, поэтому если строка превышает 255 символов, она будет усечена. Если false, строка не будет иметь указанного ограничения. Значение по умолчанию — true. |
| [GetRefreshedByWho](./getrefreshedbywho/) | Получает имя последнего пользователя, который обновил эту PivotTable |
| [GetRefreshDate](./getrefreshdate/) | Получает дату и время последнего обновления PivotTable. |
| [GetPivotTableStyle](./getpivottablestyle/) | Получает настройки TableStyle этой сводной таблицы. |
| [SetPivotTableStyle](./setpivottablestyle/) | Получает настройки TableStyle этой сводной таблицы. |
| [GetPivotTableStyleName](./getpivottablestylename/) | Получает или задает имя стиля сводной таблицы. |
| [SetPivotTableStyleName](./setpivottablestylename/) | Получает или задает имя стиля сводной таблицы. |
| [GetPivotTableStyleType](./getpivottablestyletype/) | Получает и задает встроенный стиль сводной таблицы. |
| [SetPivotTableStyleType](./setpivottablestyletype/) | Получает и задает встроенный стиль сводной таблицы. |
| [CopyStyle](./copystyle/) | Копирует именованный стиль из другой сводной таблицы. |
| [ShowReportFilterPage](./showreportfilterpage/) | Отображает все страницы фильтра отчёта в соответствии с PivotField; PivotField должен находиться в PageFields. |
| [ShowReportFilterPageByName](./showreportfilterpagebyname/) | Отображает все страницы фильтра отчёта в соответствии с именем PivotField; PivotField должен находиться в PageFields. |
| [ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | Отображает все страницы фильтра отчёта в соответствии с индексом позиции в PageFields. |
| [RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | Удаляет поле из указанной области полей. |
| [RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | Удаляет поле из указанного региона сводной таблицы. |
| [RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | Удалить поле из указанной области полей. |
| [AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | Добавляет поле в указанную область. |
| [AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | Добавляет поле в указанную область. |
| [AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | Добавляет поле в указанную область. |
| [AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | Добавляет вычисляемое поле в PivotField. |
| [AddCalculatedField_String_String](./addcalculatedfield_string_string/) | Добавляет вычисляемое поле в PivotField и перетаскивает его в область данных. |
| [GetFields](./getfields/) | Получает список конкретных полей PivotField по региону. |
| [GetColumnFields](./getcolumnfields/) | Возвращает объект PivotFields, который в данный момент отображается как столбцовые поля. |
| [GetRowFields](./getrowfields/) | Возвращает объект PivotFields, который в данный момент отображается как строковые поля. |
| [GetPageFields](./getpagefields/) | Возвращает объект PivotFields, который в данный момент отображается как page fields. |
| [GetDataFields](./getdatafields/) | Получает объект PivotField, представляющий все поля данных в PivotTable. Только для чтения. Инициализируется только когда в DataPiovtFiels присутствует два или более поля данных. Используется исключительно для добавления DataPivotField в область строк/столбцов PivotTable. По умолчанию находится в области строк. |
| [GetValuesField](./getvaluesfield/) | Получает объект PivotField, представляющий все поля данных в PivotTable. Только для чтения. Создаётся только когда в регионе Data присутствует два или более полей данных. По умолчанию находится в строковой области. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea(). |
| [GetBaseFields](./getbasefields/) | Возвращает все базовые поля PivotTable. |
| [GetPivotFilters](./getpivotfilters/) | Возвращает все фильтры pivot fields в PivotTable. |
| [GetButtonArea](./getbuttonarea/) | Получает область, содержащую кнопку поля. |
| [GetTopRightArea](./gettoprightarea/) | Представляет пустую область в правом верхнем углу PivotTable (в левом верхнем для листов RTL). |
| [GetFilterArea](./getfilterarea/) | Получает область региона фильтра. |
| [GetColumnRange](./getcolumnrange/) | Возвращает объект CellArea, который представляет диапазон, содержащий область столбцов в отчете сводной таблицы. Только для чтения. |
| [GetRowRange](./getrowrange/) | Возвращает объект CellArea, который представляет диапазон, содержащий область строк в отчете сводной таблицы. Только для чтения. |
| [GetDataBodyRange](./getdatabodyrange/) | Возвращает объект CellArea, который представляет диапазон, содержащий область данных в списке между строкой заголовка и строкой вставки. Только для чтения. |
| [GetTableRange1](./gettablerange1/) | Возвращает объект CellArea, который представляет диапазон, содержащий весь отчет сводной таблицы, но не включает поля страниц. Только для чтения. |
| [GetTableRange2](./gettablerange2/) | Возвращает объект CellArea, который представляет диапазон, содержащий весь отчет сводной таблицы, включая поля страниц. Только для чтения. |
| [MoveTo_Int_Int](./moveto_int_int/) | Перемещает сводную таблицу в другое место листа. |
| [MoveTo_Int_Int_Int](./moveto_int_int_int/) | Перемещает сводную таблицу в другое место листа. |
| [MoveTo_String](./moveto_string/) | Перемещает сводную таблицу в другое место листа. |
| [IsGridDropZones](./isgriddropzones/) | Указывает, отображает ли отчет сводной таблицы классический макет сводной таблицы (включает перетаскивание полей в сетке). |
| [SetIsGridDropZones](./setisgriddropzones/) | Указывает, отображает ли отчет сводной таблицы классический макет сводной таблицы (включает перетаскивание полей в сетке). |
| [GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | Указывает, показывать ли общие итоги для столбцов этой сводной таблицы. |
| [SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | Указывает, показывать ли общие итоги для столбцов этой сводной таблицы. |
| [GetShowRowGrandTotals](./getshowrowgrandtotals/) | Указывает, показывать ли общие итоги для строк сводной таблицы. |
| [SetShowRowGrandTotals](./setshowrowgrandtotals/) | Указывает, показывать ли общие итоги для строк сводной таблицы. |
| [GetDisplayNullString](./getdisplaynullstring/) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку, если значение равно null. |
| [SetDisplayNullString](./setdisplaynullstring/) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку, если значение равно null. |
| [GetNullString](./getnullstring/) | Получает строку, отображаемую в ячейках, содержащих null‑значения, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка. |
| [SetNullString](./setnullstring/) | Получает строку, отображаемую в ячейках, содержащих null‑значения, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка. |
| [GetDisplayErrorString](./getdisplayerrorstring/) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих ошибки. |
| [SetDisplayErrorString](./setdisplayerrorstring/) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих ошибки. |
| [GetDataFieldHeaderName](./getdatafieldheadername/) | Получает и задает имя заголовка поля области значений в сводной таблице. |
| [SetDataFieldHeaderName](./setdatafieldheadername/) | Получает и задает имя заголовка поля области значений в сводной таблице. |
| [GetErrorString](./geterrorstring/) | Получает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString равно true. Значение по умолчанию — пустая строка. |
| [SetErrorString](./seterrorstring/) | Получает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString равно true. Значение по умолчанию — пустая строка. |
| [IsAutoFormat](./isautoformat/) | Указывает, автоматически ли форматируется отчет сводной таблицы. Флажок "autoformat table " , который находится в параметрах сводной таблицы для Excel 2003. |
| [SetIsAutoFormat](./setisautoformat/) | Указывает, автоматически ли форматируется отчет сводной таблицы. Флажок "autoformat table " , который находится в параметрах сводной таблицы для Excel 2003. |
| [GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | Указывает, автоматически подгонять ли ширину столбцов при обновлении. |
| [SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | Указывает, автоматически подгонять ли ширину столбцов при обновлении. |
| [GetAutoFormatType](./getautoformattype/) | Получает и задает тип автформатирования сводной таблицы. |
| [SetAutoFormatType](./setautoformattype/) | Получает и задает тип автформатирования сводной таблицы. |
| [GetMergeLabels](./getmergelabels/) | Указывает, следует ли объединять заголовки строк или столбцов, охватывающие несколько ячеек, в одну ячейку. |
| [SetMergeLabels](./setmergelabels/) | Указывает, следует ли объединять заголовки строк или столбцов, охватывающие несколько ячеек, в одну ячейку. |
| [GetPreserveCellFormattingOnUpdate](./getpreservecellformattingonupdate/) | Указывает, сохранять ли форматирование ячеек (PivotTableFormat) при обновлении или перерасчете сводной таблицы. |
| [SetPreserveCellFormattingOnUpdate](./setpreservecellformattingonupdate/) | Указывает, сохранять ли форматирование ячеек (PivotTableFormat) при обновлении или перерасчете сводной таблицы. |
| [GetShowDrill](./getshowdrill/) | Получает и задает отображение кнопок развертывания/сворачивания. |
| [SetShowDrill](./setshowdrill/) | Получает и задает отображение кнопок развертывания/сворачивания. |
| [GetEnableDrilldown](./getenabledrilldown/) | Указывает, включено ли углубление (drilldown). |
| [SetEnableDrilldown](./setenabledrilldown/) | Указывает, включено ли углубление (drilldown). |
| [GetEnableFieldDialog](./getenablefielddialog/) | Указывает, доступен ли диалоговое окно полей сводной таблицы при двойном щелчке пользователя по полю сводной таблицы. |
| [SetEnableFieldDialog](./setenablefielddialog/) | Указывает, доступен ли диалоговое окно полей сводной таблицы при двойном щелчке пользователя по полю сводной таблицы. |
| [GetEnableFieldList](./getenablefieldlist/) | Указывает, доступен ли список полей сводной таблицы в представлении Excel. |
| [SetEnableFieldList](./setenablefieldlist/) | Указывает, доступен ли список полей сводной таблицы в представлении Excel. |
| [GetEnableWizard](./getenablewizard/) | Указывает, доступен ли мастер сводной таблицы. |
| [SetEnableWizard](./setenablewizard/) | Указывает, доступен ли мастер сводной таблицы. |
| [GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | Указывает, включаются ли скрытые элементы полей страниц в отчете сводной таблицы в промежуточные итоги строк и столбцов, блоковые итоги и общие итоги. Значение по умолчанию — False. |
| [SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | Указывает, включаются ли скрытые элементы полей страниц в отчете сводной таблицы в промежуточные итоги строк и столбцов, блоковые итоги и общие итоги. Значение по умолчанию — False. |
| [GetGrandTotalName](./getgrandtotalname/) | Возвращает метку, отображаемую в заголовке столбца или строки общего итога. Значение по умолчанию — строка "Grand Total". |
| [SetGrandTotalName](./setgrandtotalname/) | Возвращает метку, отображаемую в заголовке столбца или строки общего итога. Значение по умолчанию — строка "Grand Total". |
| [GetManualUpdate](./getmanualupdate/) | Указывает, пересчитывается ли отчет сводной таблицы только по запросу пользователя. |
| [SetManualUpdate](./setmanualupdate/) | Указывает, пересчитывается ли отчет сводной таблицы только по запросу пользователя. |
| [GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | Задает логическое значение, указывающее, могут ли поля сводной таблицы иметь несколько фильтров. |
| [SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | Задает логическое значение, указывающее, могут ли поля сводной таблицы иметь несколько фильтров. |
| [GetEnableDataValueEditing](./getenabledatavalueediting/) | Задает логическое значение, указывающее, разрешено ли пользователю редактировать ячейки в области данных сводной таблицы. Включить редактирование ячеек в области значений |
| [SetEnableDataValueEditing](./setenabledatavalueediting/) | Задает логическое значение, указывающее, разрешено ли пользователю редактировать ячейки в области данных сводной таблицы. Включить редактирование ячеек в области значений |
| [GetShowDataTips](./getshowdatatips/) | Указывает, должны ли отображаться подсказки для ячеек данных сводной таблицы. |
| [SetShowDataTips](./setshowdatatips/) | Указывает, должны ли отображаться подсказки для ячеек данных сводной таблицы. |
| [GetShowMemberPropertyTips](./getshowmemberpropertytips/) | Задает логическое значение, указывающее, следует ли исключать информацию о свойствах элементов из подсказок сводной таблицы. |
| [SetShowMemberPropertyTips](./setshowmemberpropertytips/) | Задает логическое значение, указывающее, следует ли исключать информацию о свойствах элементов из подсказок сводной таблицы. |
| [GetShowValuesRow](./getshowvaluesrow/) | Указывает, отображать ли строку значений. |
| [SetShowValuesRow](./setshowvaluesrow/) | Указывает, отображать ли строку значений. |
| [GetShowEmptyCol](./getshowemptycol/) | Указывает, включать ли пустые столбцы в таблицу. |
| [SetShowEmptyCol](./setshowemptycol/) | Указывает, включать ли пустые столбцы в таблицу. |
| [GetShowEmptyRow](./getshowemptyrow/) | Указывает, включать ли пустые строки в таблицу. |
| [SetShowEmptyRow](./setshowemptyrow/) | Указывает, включать ли пустые строки в таблицу. |
| [GetFieldListSortAscending](./getfieldlistsortascending/) | Указывает, отсортированы ли поля сводной таблицы в нестандартном порядке в списке полей. |
| [SetFieldListSortAscending](./setfieldlistsortascending/) | Указывает, отсортированы ли поля сводной таблицы в нестандартном порядке в списке полей. |
| [GetPrintDrill](./getprintdrill/) | Задает логическое значение, указывающее, следует ли печатать индикаторы детализации. Печатать кнопки раскрытия/сворачивания при отображении в сводной таблице. |
| [SetPrintDrill](./setprintdrill/) | Задает логическое значение, указывающее, следует ли печатать индикаторы детализации. Печатать кнопки раскрытия/сворачивания при отображении в сводной таблице. |
| [GetAltTextTitle](./getalttexttitle/) | Получает и задает заголовок альтернативного текста. |
| [SetAltTextTitle](./setalttexttitle/) | Получает и задает заголовок альтернативного текста. |
| [GetAltTextDescription](./getalttextdescription/) | Получает описание альтернативного текста. |
| [SetAltTextDescription](./setalttextdescription/) | Получает описание альтернативного текста. |
| [GetName](./getname/) | Получает имя сводной таблицы. |
| [SetName](./setname/) | Получает имя сводной таблицы. |
| [GetColumnHeaderCaption](./getcolumnheadercaption/) | Получает и задает пользовательскую подпись заголовка столбца сводной таблицы. |
| [SetColumnHeaderCaption](./setcolumnheadercaption/) | Получает и задает пользовательскую подпись заголовка столбца сводной таблицы. |
| [GetIndent](./getindent/) | Задает шаг отступа для компактной оси и может использоваться для установки макета отчета в компактную форму. |
| [SetIndent](./setindent/) | Задает шаг отступа для компактной оси и может использоваться для установки макета отчета в компактную форму. |
| [GetRowHeaderCaption](./getrowheadercaption/) | Получает и задает пользовательскую подпись заголовка строки в этой сводной таблице. |
| [SetRowHeaderCaption](./setrowheadercaption/) | Получает и задает пользовательскую подпись заголовка строки в этой сводной таблице. |
| [GetShowHeaders](./getshowheaders/) | Отображать ли подписи полей данных и подписи полей сводной таблицы по оси строк и оси столбцов в представлении сводной таблицы. |
| [SetShowHeaders](./setshowheaders/) | Отображать ли подписи полей данных и подписи полей сводной таблицы по оси строк и оси столбцов в представлении сводной таблицы. |
| [GetCustomListSort](./getcustomlistsort/) | Указывает, учитывать ли встроенный пользовательский список при сортировке данных. |
| [SetCustomListSort](./setcustomlistsort/) | Указывает, учитывать ли встроенный пользовательский список при сортировке данных. |
| [GetConditionalFormats](./getconditionalformats/) | Получает условные форматы сводной таблицы. |
| [GetPageFieldOrder](./getpagefieldorder/) | Получает и задает порядок, в котором поля страниц добавляются в макет отчета сводной таблицы. |
| [SetPageFieldOrder](./setpagefieldorder/) | Получает и задает порядок, в котором поля страниц добавляются в макет отчета сводной таблицы. |
| [GetPageFieldWrapCount](./getpagefieldwrapcount/) | Получает количество полей страниц в каждом столбце или строке отчета сводной таблицы. |
| [SetPageFieldWrapCount](./setpagefieldwrapcount/) | Получает количество полей страниц в каждом столбце или строке отчета сводной таблицы. |
| [GetTag](./gettag/) | Получает и задает пользовательскую строку, связанную с этим представлением сводной таблицы. |
| [SetTag](./settag/) | Получает и задает пользовательскую строку, связанную с этим представлением сводной таблицы. |
| [GetSaveData](./getsavedata/) | Указывает, сохраняются ли данные отчета сводной таблицы вместе с книгой. |
| [SetSaveData](./setsavedata/) | Указывает, сохраняются ли данные отчета сводной таблицы вместе с книгой. |
| [GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | Указывает, обновлять ли данные при открытии файла. |
| [SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | Указывает, обновлять ли данные при открытии файла. |
| [GetSourceType](./getsourcetype/) | Получает тип источника данных сводной таблицы. |
| [GetSourceDataConnections](./getsourcedataconnections/) | Получает внешние источники данных соединения. |
| [GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | Получает имена внешних соединений источников данных. |
| [GetDataSource](./getdatasource/) | Получает и задает источник данных сводной таблицы. |
| [SetDataSource](./setdatasource/) | Получает и задает источник данных сводной таблицы. |
| [ChangeDataSource](./changedatasource/) | Изменить источник данных сводной таблицы. |
| [GetSource](./getsource/) | Получить источник данных этой сводной таблицы. |
| [GetSource_Bool](./getsource_bool/) | Получить источник данных этой сводной таблицы. |
| [Refresh](./refresh/) | Обновить PivotCache из источника данных и вычислить данные и стиль для представления сводной таблицы. |
| [CalculateData](./calculatedata/) | Вычисляет данные сводной таблицы в ячейки. |
| [CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | Вычисляет сводную таблицу с параметрами. |
| [GetPivotTablesWithSamePivotCache](./getpivottableswithsamepivotcache/) | Получает все сводные таблицы с одинаковым кэшем сводных данных. |
| [ClearData](./cleardata/) | Очистить данные и форматирование представления сводной таблицы. |
| [ClearFilters](./clearfilters/) | Снимает все фильтры этой сводной таблицы. |
| [ClearAll](./clearall/) | Удалить все поля из областей. |
| [CalculateRange](./calculaterange/) | Вычисляет диапазон сводной таблицы. |
| [FormatAll](./formatall/) | Форматировать все ячейки в области сводной таблицы |
| [FormatRow](./formatrow/) | Форматировать данные строк в области сводной таблицы |
| [Format_PivotArea_Style](./format_pivotarea_style/) | Форматирует выбранную область сводной таблицы. |
| [Format_CellArea_Style](./format_cellarea_style/) | Форматирует выбранную область сводной таблицы. |
| [Format_Int_Int_Style](./format_int_int_style/) | Форматировать ячейку в области сводной таблицы |
| [SelectArea](./selectarea/) | Выбрать область представления сводной таблицы. |
| [ShowDetail](./showdetail/) | Показать детали одного элемента в области данных в новой таблице. |
| [GetPivotFormats](./getpivotformats/) | Получает все форматы, применённые к сводной таблице. |
| [GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | Указывает, повторяются ли подписи элементов сводной таблицы в строковой области на каждой печатной странице для полей сводной таблицы в табличной форме. |
| [SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | Указывает, повторяются ли подписи элементов сводной таблицы в строковой области на каждой печатной странице для полей сводной таблицы в табличной форме. |
| [GetPrintTitles](./getprinttitles/) | Указывает, установлены ли заголовки печати листа на основе отчёта сводной таблицы. Значение по умолчанию — false. |
| [SetPrintTitles](./setprinttitles/) | Указывает, установлены ли заголовки печати листа на основе отчёта сводной таблицы. Значение по умолчанию — false. |
| [GetDisplayImmediateItems](./getdisplayimmediateitems/) | Указывает, видимы ли элементы в строковой и столбцовой областях, когда область данных сводной таблицы пуста. Значение по умолчанию — true. |
| [SetDisplayImmediateItems](./setdisplayimmediateitems/) | Указывает, видимы ли элементы в строковой и столбцовой областях, когда область данных сводной таблицы пуста. Значение по умолчанию — true. |
| [IsSelected](./isselected/) | Указывает, выбрана ли эта сводная таблица. |
| [SetIsSelected](./setisselected/) | Указывает, выбрана ли эта сводная таблица. |
| [GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | Указывает, следует ли применять стиль к заголовку строки в сводной таблице. |
| [SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | Указывает, следует ли применять стиль к заголовку строки в сводной таблице. |
| [GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | Указывает, следует ли применять стиль к заголовку столбца в сводной таблице. |
| [SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | Указывает, следует ли применять стиль к заголовку столбца в сводной таблице. |
| [GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | Указывает, применяется ли чередование строк. |
| [SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | Указывает, применяется ли чередование строк. |
| [GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | Указывает, применяется ли чередование для столбца. |
| [SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | Указывает, применяется ли чередование для столбца. |
| [GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | Указывает, применяется ли форматирование столбца. |
| [SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | Указывает, применяется ли форматирование столбца. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Получает горизонтальные разрывы страниц этой сводной таблицы. |
| [ShowInCompactForm](./showincompactform/) | Отображает представление сводной таблицы в компактной форме. |
| [ShowInOutlineForm](./showinoutlineform/) | Отображает сводную таблицу в виде схемы. |
| [ShowInTabularForm](./showintabularform/) | Отображает сводную таблицу в табличной форме. |
| [GetCellByDisplayName](./getcellbydisplayname/) | Получает объект Cell по отображаемому имени PivotField. |
| [GetDependentPivotTables](./getdependentpivottables/) | Получает все PivotTables, использующие эту PivotTable в качестве источника данных. |
| [ExportViewToJson](./exportviewtojson/) | Экспортирует представление сводной таблицы в формате JSON. |
