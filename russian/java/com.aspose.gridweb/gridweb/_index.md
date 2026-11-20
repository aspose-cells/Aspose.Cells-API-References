---
title: "GridWeb"
second_title: "Справочник API Aspose.Cells for Java"
description: "Базовый класс элемента управления GridWeb."
type: docs
url: /ru/java/com.aspose.gridweb/gridweb/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWeb extends MainWeb
```

Базовый класс элемента управления GridWeb.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridWeb()](#GridWeb--) |  |
## Поля

| Поле | Описание |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | Происходит после фильтрации столбца. |
| [AjaxCallFinished](#AjaxCallFinished) | Срабатывает, когда ajax‑обновление элемента управления завершилось. |
| [BeforeColumnFilter](#BeforeColumnFilter) | Происходит перед тем, как столбец будет отфильтрован. |
| [CellClickOnAjax](#CellClickOnAjax) | Происходит, когда ячейка нажата, и необходимо выполнить ajaxcallback для этого события. |
| [CellClientUpdate](#CellClientUpdate) | Происходит, когда происходит обновление ячейки на клиенте. |
| [CellCommand](#CellCommand) | Происходит, когда ссылка команды ячейки нажата. |
| [CellDoubleClick](#CellDoubleClick) | Происходит, когда ячейка двойным щелчком. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | Происходит, когда ячейка изменяется в ajaxcall. |
| [ColumnDeleted](#ColumnDeleted) | Происходит, когда пользователь удаляет столбец из клиентского меню. |
| [ColumnDeleting](#ColumnDeleting) | Происходит, когда пользователь пытается удалить столбец из клиентского меню. |
| [ColumnDoubleClick](#ColumnDoubleClick) | Происходит, когда заголовок столбца двойным щелчком. |
| [ColumnInserted](#ColumnInserted) | Происходит, когда пользователь вставляет столбец из клиентского меню. |
| [CustomCommand](#CustomCommand) | Происходит, когда пользователь нажимает кнопку пользовательской команды. |
| [LoadCustomData](#LoadCustomData) | Срабатывает, когда свойство SessionMode элемента управления установлено в Custom и требуется загрузить данные листа. |
| [PageIndexChanged](#PageIndexChanged) | Происходит, когда изменяется индекс страницы листа элемента управления. |
| [RowDeleted](#RowDeleted) | Происходит, когда пользователь удалил строку из клиентского меню. |
| [RowDeleting](#RowDeleting) | Происходит, когда пользователь пытается удалить строку из клиентского меню. |
| [RowDoubleClick](#RowDoubleClick) | Происходит, когда заголовок строки двойным щелчком. |
| [RowInserted](#RowInserted) | Происходит, когда пользователь вставляет строку из клиентского меню. |
| [SaveCommand](#SaveCommand) | Происходит, когда нажата кнопка "save". |
| [SheetAdded](#SheetAdded) | Происходит, когда пользователь добавляет лист из меню панели инструментов. |
| [SheetTabClick](#SheetTabClick) | Происходит, когда нажата вкладка листа. |
| [SubmitCommand](#SubmitCommand) | Происходит, когда нажата кнопка "submit". |
| [UndoCommand](#UndoCommand) | Происходит, когда нажата кнопка "undo". |
## Методы

| Метод | Описание |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Вычисляет результат формул. |
| [createChildControls()](#createChildControls--) | Реализует CreateChildControls из WebControl, используется только внутри. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | Возвращает веб‑путь к файлам скриптов/изображений элемента управления. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | Возвращает веб‑URL языкового файла элемента управления. |
| [getActiveCell()](#getActiveCell--) | Возвращает активную ячейку текущего листа. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Задает цвет фона активной ячейки. |
| [getActiveCellColor()](#getActiveCellColor--) | Задает цвет активной ячейки. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Задает цвет фона активного заголовка строки/столбца. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Задает цвет активного заголовка строки/столбца. |
| [getActiveSheet()](#getActiveSheet--) | Возвращает активный лист |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Возвращает индекс активного листа. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Задает стиль активной вкладки. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | Возвращает, обновляется ли изображение диаграммы при изменении значения ячейки. По умолчанию true. |
| [getBackColor()](#getBackColor--) | Получает BackColor в WebControl |
| [getBorderColor()](#getBorderColor--) | Получает BorderColor в WebControl |
| [getBorderStyle()](#getBorderStyle--) | Получает BorderStyle в WebControl |
| [getBorderWidth()](#getBorderWidth--) | Получает BorderWidth в WebControl |
| [getBottomTableStyle()](#getBottomTableStyle--) | Возвращает стиль нижней панели элемента управления. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Получает CssClass в WebControl |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | Возвращает текущий индекс страницы в режиме постраничного отображения. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Представляет пользовательский движок вычислений для расширения движка вычислений по умолчанию в Aspose.Cells. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | Получает коллекцию пользовательских кнопок команд |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | Получает имя файла пользовательского стиля. |
| [getDPI()](#getDPI--) | Получает/устанавливает DPI устройства. |
| [getDefaultFontName()](#getDefaultFontName--) | Получает имя шрифта по умолчанию для элемента управления. |
| [getDefaultFontSize()](#getDefaultFontSize--) | Получает размер шрифта по умолчанию элемента управления. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | Получает цвет линии сетки по умолчанию. |
| [getDisplayCellTip()](#getDisplayCellTip--) | Получает, показывать ли подсказки. значение по умолчанию — true. |
| [getEditMode()](#getEditMode--) | Получает режим редактирования элемента управления. |
| [getEnableAJAX()](#getEnableAJAX--) | Получает, использовать ли вызов AJAX. значение по умолчанию — true. |
| [getEnableAsync()](#getEnableAsync--) | Получает, загружать ли данные ячеек асинхронно, рекомендуется использовать для листа с более чем 10000 ячейками |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | Получает, включены ли клиентские операции с колонками. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | Получает, включены ли клиентские операции заморозки. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | Получает, включены ли клиентские операции слияния. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | Получает, включено ли изменение размера колонок и строк на клиенте. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | Получает, включены ли клиентские операции со строками. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | Получает, включено ли событие двойного щелчка со стороны клиента. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | Получает, применять ли металлический световой эффект. |
| [getEnablePaging()](#getEnablePaging--) | Получает, включен ли режим постраничного отображения элемента управления. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | Получает, включено ли диалоговое окно стилей на клиенте. |
| [getEnabled()](#getEnabled--) | Получает Enabled в WebControl |
| [getFilteredPaging()](#getFilteredPaging--) | Получает, включать ли постраничный вывод после фильтрации данных, будет применяться, когда EnablePaging равно true |
| [getFont()](#getFont--) | Получает Font в WebControl |
| [getForceValidation()](#getForceValidation--) | Получает, принудительно ли выполнять проверку на стороне клиента. |
| [getForeColor()](#getForeColor--) | Получает ForeColor в WebControl |
| [getFrameTableStyle()](#getFrameTableStyle--) | Получает стиль рамки элемента управления. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | Получает, будет ли GridWeb выполнять операцию сохранения по умолчанию, значение по умолчанию — true. |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | Получает высоту (System.Web.UI.WebControl.Unit) верхней панели заголовка элемента управления. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | Получает стиль панели заголовка. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | Получает стиль панели заголовка элемента управления. |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | Получает ширину ( System.Web.UI.WebControl.Unit ) или левую панель заголовка элемента управления. |
| [getHeight()](#getHeight--) | Получает высоту ( System.Web.UI.WebControl.Unit ) элемента управления. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | Получает, игнорирует ли GridWeb отображение строк или столбцов, не содержащих значения ячеек, но имеющих стиль. |
| [getLoadOptions()](#getLoadOptions--) | Представляет параметры загрузки для GridWeb. |
| [getMaxColumn()](#getMaxColumn--) | Получает максимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. |
| [getMaxRow()](#getMaxRow--) | Получает максимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. |
| [getMessage()](#getMessage--) | Получает сообщение для сетки. |
| [getMinColumn()](#getMinColumn--) | Получает минимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. |
| [getMinRow()](#getMinRow--) | Получает минимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. |
| [getModifiedCells()](#getModifiedCells--) | Получает коллекцию ячеек, изменённых клиентом. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | Получает, следует ли отображать групповые строки. |
| [getNoHScroll()](#getNoHScroll--) | Получает значение, указывающее, скрыта ли горизонтальная полоса прокрутки. |
| [getNoScroll()](#getNoScroll--) | Получает, следует ли отображать полосу прокрутки. |
| [getNoVScroll()](#getNoVScroll--) | Получает значение, указывающее, скрыта ли вертикальная полоса прокрутки. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | Получает имя клиентской функции, вызываемой после завершения ajax‑вызова. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | Получает имя клиентской функции, вызываемой при неудачной проверке ячейки. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | Получает клиентскую функцию, вызываемую при выборе ячейки. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | Получает клиентскую функцию, вызываемую при выборе ячейки. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | Получает клиентскую функцию, вызываемую при отмене выбора ячейки. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | Получает имя клиентской функции, вызываемой при обновлении значения ячейки. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | Получает клиентскую функцию, вызываемую при отображении контекстного меню. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | Получает клиентскую функцию, вызываемую при двойном щелчке по ячейке. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | Получает клиентскую функцию, вызываемую при двойном щелчке по строке. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | Получает имя клиентской функции, вызываемой при инициализации сетки. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | Получает клиентскую функцию, вызываемую после изменения индекса страницы. Действует только при EnablePaging = true. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | Получает клиентскую функцию, вызываемую перед отправкой страницы на клиенте. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | Получает клиентскую функцию, вызываемую при выборе фигуры. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | Получает клиентскую функцию, вызываемую перед отправкой управления на клиенте. |
| [getOnlyAuto()](#getOnlyAuto--) | Получает, следует ли подгонять только строки, высота которых не задана пользователем; значение по умолчанию — false. |
| [getPageSize()](#getPageSize--) | Получает размер страницы в режиме постраничного вывода. |
| [getPictureCachePath()](#getPictureCachePath--) | Получает путь хранения изображений для рабочей книги; все фигуры и изображения будут сохраняться в этом каталоге, путь по умолчанию — acwcache в базовом каталоге текущего приложения. Пользователи должны реализовать плановый сервис для очистки файлов, вышедших за пределы времени сессии. |
| [getPresetStyle()](#getPresetStyle--) | Получает предустановленный стиль. |
| [getRefreshValidation()](#getRefreshValidation--) | Получает, следует ли обновлять значение проверки после изменения значения ячейки. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | Получает, отображается ли скрытая строка в GridControl; значение по умолчанию — false. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | Получает значение высоты строки в пунктах для CSV‑файла; значение по умолчанию — 14,5. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Указывает цвет кнопки‑стрелки полосы прокрутки. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Указывает цвет полосы прокрутки элемента управления. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Указывает цвет фона выбранных ячеек в диапазоне множественного выбора. |
| [getSelectCellColor()](#getSelectCellColor--) | Указывает цвет выбранных ячеек в диапазоне множественного выбора. |
| [getSelectCells()](#getSelectCells--) | Получает коллекцию выбранных ячеек. |
| [getSessionStorePath()](#getSessionStorePath--) | Получает путь к хранилищу кэша сеанса, когда режим сеанса — File или ViewState и т.д.: gridweb.SessionStorePath="c:/mytempdir/session"; тогда данные сеанса будут сохраняться в c:/mytempdir/session. |
| [getSettings()](#getSettings--) | Представляет настройки рабочей книги. |
| [getShowAddButton()](#getShowAddButton--) | Получает, отображать ли кнопку добавления листа. |
| [getShowBottomBar()](#getShowBottomBar--) | Указывает, показывать ли панель команд (включая панель команд и вкладок) в нижней части элемента управления. |
| [getShowCellEditBox()](#getShowCellEditBox--) | Определяет, отображает ли Gridweb панель инструментов редактирования, как в MS‑EXCEL. Если включено, для текущей ячейки будет отображаться поле редактирования в Gridweb. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Указывает, показывать ли панель команд (включая панель команд и вкладок) в верхней части элемента управления. |
| [getShowContextMenu()](#getShowContextMenu--) | Получает, отображать ли контекстное меню; значение по умолчанию — true. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | Получает, отображать ли стандартные линии сетки ячеек. |
| [getShowHeaderBar()](#getShowHeaderBar--) | Получает, отображать ли строку заголовка. |
| [getShowLoading()](#getShowLoading--) | Указывает, показывать ли диалоговое окно загрузки во время обратного вызова на сервер. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Указывает левую и верхнюю позицию (в пикселях) для отображения диалогового окна загрузки во время обратного вызова на сервер и т.д. 100,200 означает, что левый верхний угол окна загрузки находится на 100 px, 200 px. |
| [getShowSaveButton()](#getShowSaveButton--) | Получает, отображать ли кнопку сохранения. |
| [getShowSubmitButton()](#getShowSubmitButton--) | Получает, показывать ли кнопку отправки. |
| [getShowTabBar()](#getShowTabBar--) | Получает, показывать ли панель вкладок. |
| [getShowTabNavigation()](#getShowTabNavigation--) | Получает, отображается ли кнопка навигации по вкладкам, значение по умолчанию — true. |
| [getShowUndoButton()](#getShowUndoButton--) | Получает, показывать ли кнопку отмены. |
| [getSpanWrap()](#getSpanWrap--) | Указывает, переносить ли содержимое в диапазоне ячеек, значение по умолчанию — true. |
| [getTabIndex()](#getTabIndex--) | Получает TabIndex в WebControl |
| [getTabStyle()](#getTabStyle--) | Получает стиль панели вкладок. |
| [getToolTip()](#getToolTip--) | Получает ToolTip в WebControl |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | Получает, использует ли GridWeb высоту клиентской страницы в качестве высоты элемента управления, подходит, когда установлено Height=\"100%\", значение по умолчанию — false. |
| [getVersion()](#getVersion--) | Получить версию релиза. |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | Получает положение полосы прокрутки панели просмотра сетки. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | Получает положение полосы прокрутки панели просмотра сетки. |
| [getViewTableStyle()](#getViewTableStyle--) | Получает стиль панели просмотра данных. |
| [getWidth()](#getWidth--) | Получает ширину (System.Web.UI.WebControl.Unit) элемента управления. |
| [getWorkSheets()](#getWorkSheets--) | Получает коллекцию листов. |
| [getXhtmlMode()](#getXhtmlMode--) | Получает, использовать ли стиль XHTML, значение по умолчанию — true. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Импортирует из потока Excel‑файла, включая поток файлового диска или поток памяти. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Импортирует из потока Excel‑файла, включая поток файлового диска или поток памяти. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Импортирует из Excel‑файла. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Импортирует из Excel‑файла. |
| [isCalculateFormula()](#isCalculateFormula--) | Получает, вычислять ли формулы после изменения значения ячейки или после импорта файла. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | Загружает данные из потока CSV‑файла. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | Загружает данные из CSV‑файла. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | Загружает данные из потока HTML‑файла. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | Загружает данные из HTML‑файла. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | Загружает данные из потока файла SpreadSheetML. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | Загружает данные из файла SpreadSheetML. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshChartShape()](#refreshChartShape--) | Обновляет все изображения диаграмм для активного листа. |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | Сохраняет данные в поток CSV‑файла. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | Сохраняет данные в CSV‑файл. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | Сохраняет текущие данные стиля элемента управления в XML‑файл. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | Сохраняет данные в поток HTML‑файла. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | Сохраняет данные в HTML‑файл. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | Сохраняет данные в поток файла SpreadSheetML. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | Сохраняет данные в файл SpreadSheetML. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Сохраняет листы в файл Excel. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | Сохраняет листы в файл Excel. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | Сохраняет листы в файл Excel. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | Сохраняет листы в файл Excel в формате Excel 2003. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | Сохраняет листы в файл Excel. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | Сохраняет листы в файл Excel. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | Устанавливает веб‑путь к скриптам/изображениям элемента управления. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | Устанавливает веб‑URL языкового файла элемента управления. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | Устанавливает активную ячейку текущего листа. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Задает цвет фона активной ячейки. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Задает цвет активной ячейки. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Задает цвет фона активного заголовка строки/столбца. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Задает цвет активного заголовка строки/столбца. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Устанавливает индекс активного листа. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Задает стиль активной вкладки. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | Устанавливает, обновляется ли изображение диаграммы при изменении значения ячейки. По умолчанию true. |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Устанавливает BackColor в WebControl |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Устанавливает BorderColor в WebControl |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Устанавливает BorderStyle в WebControl |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Устанавливает BorderWidth в WebControl |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | Устанавливает стиль нижней панели элемента управления. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Устанавливает, вычислять ли формулы после изменения значения ячейки или после импорта файла. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Устанавливает CssClass в WebControl |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | Устанавливает индекс текущей страницы в режиме постраничного вывода. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | Представляет пользовательский движок вычислений для расширения движка вычислений по умолчанию в Aspose.Cells. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | Устанавливает пользовательский файл стилей из потока, включая файловый поток диска или поток памяти. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | Устанавливает имя пользовательского файла стилей. |
| [setDPI(double value)](#setDPI-double-) | Получает/устанавливает DPI устройства. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Устанавливает имя шрифта по умолчанию для элемента управления. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | Устанавливает размер шрифта по умолчанию для элемента управления. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | Устанавливает цвет линий сетки по умолчанию. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | Устанавливает, показывать ли подсказки. Значение по умолчанию — true. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | Устанавливает режим редактирования элемента управления. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | Устанавливает, использовать ли AJAX‑вызов. Значение по умолчанию — true. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | Устанавливает, загружать ли данные ячеек асинхронно, рекомендуется для листа с более чем 10000 ячейками. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | Устанавливает, включать ли клиентские операции со столбцами. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | Устанавливает, включать ли клиентские операции заморозки. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | Устанавливает, включать ли клиентские операции объединения. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | Устанавливает, включено ли изменение размера столбцов и строк на клиенте. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | Устанавливает, включены ли операции со строками на клиенте. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | Устанавливает, включено ли событие двойного щелчка на клиенте. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | Устанавливает, применять ли эффект металлического света. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | Устанавливает, включён ли режим постраничного отображения управления. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | Устанавливает, включён ли диалог стилей на клиенте. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Устанавливает Enabled в WebControl |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | Устанавливает, включено ли постраничное отображение после фильтрации данных, будет применяться, когда EnablePaging равно true. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Устанавливает папку шрифтов |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Устанавливает папки шрифтов |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | Устанавливает, принудительно ли выполнять проверку на клиенте. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Устанавливает ForeColor в WebControl |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | Устанавливает стиль рамки управления. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | Устанавливает, будет ли GridWeb выполнять операцию сохранения по умолчанию, значение по умолчанию — true. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | Устанавливает высоту (System.Web.UI.WebControl.Unit) верхней панели заголовка управления. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | Устанавливает стиль панели заголовка. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | Устанавливает стиль панели заголовка управления. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | Устанавливает ширину (System.Web.UI.WebControl.Unit) или левую панель заголовка управления. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Устанавливает высоту (System.Web.UI.WebControl.Unit) управления. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | Устанавливает, игнорирует ли GridWeb отображение строк или столбцов без значений ячеек, но со стилем. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | Представляет параметры загрузки для GridWeb. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | Устанавливает максимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. |
| [setMaxRow(int value)](#setMaxRow-int-) | Устанавливает максимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. |
| [setMessage(String value)](#setMessage-java.lang.String-) | Устанавливает сообщение для сетки. |
| [setMinColumn(int value)](#setMinColumn-int-) | Устанавливает минимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. |
| [setMinRow(int value)](#setMinRow-int-) | Устанавливает минимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | Устанавливает, показывать ли группы строк. |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | Устанавливает значение, указывающее, скрыта ли горизонтальная полоса прокрутки. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | Устанавливает, показывать ли полосу прокрутки. |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | Устанавливает значение, указывающее, скрыта ли вертикальная полоса прокрутки. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | Устанавливает имя функции на клиентской стороне, вызываемой после завершения ajax‑вызова. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | Устанавливает имя функции на клиентской стороне, вызываемой при провале проверки ячейки. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую при выборе ячейки. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую при выборе ячейки. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую при снятии выделения с ячейки. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | Устанавливает имя функции на клиентской стороне, вызываемой при обновлении значения ячейки. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую при отображении контекстного меню. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую при двойном щелчке по ячейке. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую при двойном щелчке по строке. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | Устанавливает имя функции на клиентской стороне, вызываемой при инициализации сетки. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую после изменения индекса страницы. Действует только при включённом EnablePaging. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую перед отправкой страницы. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую при выборе фигуры. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | Устанавливает функцию на клиентской стороне, вызываемую перед отправкой управления. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Устанавливает, следует ли подгонять только строки, высота которых не задана вручную; значение по умолчанию — false. |
| [setPageSize(int value)](#setPageSize-int-) | Устанавливает размер страницы в режиме постраничного отображения. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | Устанавливает путь хранения изображений для рабочей книги; все фигуры и изображения будут сохраняться в этом каталоге. Путь по умолчанию — acwcache в базовом каталоге текущего приложения. Пользователям необходимо реализовать плановый сервис для очистки файлов, срок действия которых истёк. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Устанавливает предустановленный стиль. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | Устанавливает, следует ли обновлять значение проверки после изменения значения ячейки. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | Устанавливает, будет ли скрытая строка отрисовываться в GridControl; значение по умолчанию — false. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | Устанавливает значение высоты строки в пунктах для CSV‑файла; значение по умолчанию — 14,5. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | Указывает цвет кнопки‑стрелки полосы прокрутки. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | Указывает цвет полосы прокрутки элемента управления. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Указывает цвет фона выбранных ячеек в диапазоне множественного выбора. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Указывает цвет выбранных ячеек в диапазоне множественного выбора. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | Устанавливает путь хранения кэша сеанса, когда режим сеанса — File или ViewState и т.д.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; тогда данные сеанса будут сохраняться в c:/mytempdir/session. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | Представляет настройки рабочей книги. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | Устанавливает, отображать ли кнопку добавления листа. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | Указывает, показывать ли панель команд (включая панель команд и вкладок) в нижней части элемента управления. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | Определяет, отображает ли Gridweb панель инструментов редактирования, как в MS‑EXCEL. Если включено, для текущей ячейки будет отображаться поле редактирования в Gridweb. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | Указывает, показывать ли панель команд (включая панель команд и вкладок) в верхней части элемента управления. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | Устанавливает, отображать ли контекстное меню; значение по умолчанию — true. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | Устанавливает, отображать ли стандартные линии сетки ячеек. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | Устанавливает, отображать ли строку заголовка. |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | Указывает, показывать ли диалоговое окно загрузки во время обратного вызова на сервер. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | Указывает левую и верхнюю позицию (в пикселях) для отображения диалогового окна загрузки во время обратного вызова на сервер и т.д. 100,200 означает, что левый верхний угол окна загрузки находится на 100 px, 200 px. |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | Устанавливает, показывать ли кнопку сохранения. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | Устанавливает, показывать ли кнопку отправки. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | Устанавливает, показывать ли панель вкладок. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | Устанавливает, показывается ли кнопка навигации по вкладкам, значение по умолчанию — true. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | Устанавливает, показывать ли кнопку отмены. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | Указывает, переносить ли содержимое в диапазоне ячеек, значение по умолчанию — true. |
| [setTabIndex(short value)](#setTabIndex-short-) | Устанавливает TabIndex в WebControl |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Устанавливает стиль панели вкладок. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Устанавливает ToolTip в WebControl |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | Устанавливает, использовать ли GridWeb высоту клиентской страницы в качестве высоты элемента управления, подходит, когда Height=\"100%\", значение по умолчанию — false. |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | Устанавливает положение полосы прокрутки панели просмотра сетки. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | Устанавливает положение полосы прокрутки панели просмотра сетки. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | Устанавливает стиль панели просмотра данных. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Устанавливает ширину (System.Web.UI.WebControl.Unit) элемента управления. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | Устанавливает, использовать ли стиль XHTML, значение по умолчанию — true. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWeb() {#GridWeb--}
```
public GridWeb()
```


### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```


Происходит после фильтрации столбца.

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


Срабатывает, когда AJAX‑обновление элемента управления завершено (EnableAJAX должно быть установлено в true).

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


Происходит перед тем, как столбец будет отфильтрован.

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


Происходит, когда ячейка нажата, и необходимо выполнить ajaxcallback для этого события.

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


Происходит, когда происходит обновление ячейки на клиенте. Когда это событие срабатывает, его параметр e.Argument содержит имя команды.

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


Происходит, когда нажата гиперссылка команды ячейки. При срабатывании этого события его параметр e.Argument содержит имя команды.

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


Происходит, когда ячейка двойным щелчком.

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


Происходит, когда ячейка изменяется в ajaxcall.

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


Происходит, когда пользователь удаляет столбец из клиентского меню.

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


Происходит, когда пользователь пытается удалить столбец из контекстного меню на клиенте. Вы можете обработать это событие и установить параметр cancel в True, чтобы отменить операцию удаления.

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


Происходит, когда заголовок столбца двойным щелчком.

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


Происходит, когда пользователь вставляет столбец из клиентского меню.

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


Происходит, когда пользователь нажимает кнопку пользовательской команды.

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


Срабатывает, когда SessionMode элемента управления установлен в Custom и требуется загрузить данные листа. Вы можете обработать это событие в режиме Custom Session для загрузки данных листа из файла или базы данных.

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


Происходит, когда изменяется индекс страницы листа элемента управления.

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


Происходит, когда пользователь удалил строку из клиентского меню.

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


Происходит, когда пользователь пытается удалить строку из контекстного меню на клиенте. Вы можете обработать это событие и бросить исключение RejectDeleteException, чтобы отменить операцию удаления.

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


Происходит, когда заголовок строки двойным щелчком.

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


Происходит, когда пользователь вставляет строку из клиентского меню.

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


Происходит, когда нажата кнопка "save".

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


Происходит, когда пользователь добавляет лист из меню панели инструментов.

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


Происходит, когда нажата вкладка листа.

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


Происходит, когда нажата кнопка "submit".

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


Происходит, когда нажата кнопка "undo".

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Вычисляет результат формул.

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


Реализует CreateChildControls из WebControl, используется только внутри.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


Получает веб‑путь к скриптам/изображениям элемента управления. Например: \"http://localhost/acw\\_client\". Вы также можете задать это значение в файле web.config. Добавьте этот раздел в раздел `<configuration>`:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


Получает веб‑URL файла локализации элемента управления. Например: \"/acw\\_client/lang\\_en.js\".
По умолчанию используется встроенный английский файл.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


Получает активную ячейку текущего листа. С версии 1.9.0.1 стала доступна для записи.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


Задает цвет фона активной ячейки.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


Задает цвет активной ячейки.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


Задает цвет фона активного заголовка строки/столбца.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


Задает цвет активного заголовка строки/столбца.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


Возвращает активный лист

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Получает индекс активного листа. Эквивалентно WebWorksheets.ActiveSheetIndex.

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


Задает стиль активной вкладки.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


Возвращает, обновляется ли изображение диаграммы при изменении значения ячейки. По умолчанию true.

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Получает BackColor в WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Получает BorderColor в WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Получает BorderStyle в WebControl

Смотрите [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Получает BorderWidth в WebControl

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


Возвращает стиль нижней панели элемента управления.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Получает CssClass в WebControl

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


Возвращает текущий индекс страницы в режиме постраничного отображения.

**Remarks**

В режиме постраничного отображения контрол будет отображать PageSize строк данных один раз, и отображать элемент выбора страницы на панели вкладок.

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


Представляет пользовательский движок вычислений для расширения движка вычислений по умолчанию в Aspose.Cells.

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


Получает коллекцию пользовательских кнопок команд

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


Получает имя файла пользовательского стиля.

**Remarks**

Пользовательский файл стиля является XML‑файлом. При установке имени файла он будет загружен немедленно. Ниже содержимое "standard preset style" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Example**

```
         		GridWeb1.setCustomStyleFileName("c:\\style\\mystyle.xml");
```

**Returns:**
java.lang.String
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Получает/устанавливает DPI устройства.

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Получает имя шрифта по умолчанию для элемента управления.

**Example**

```
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


Получает размер шрифта по умолчанию элемента управления.

**Example**

```
         		GridWeb1.setDefaultFontSize(new FontUnit("10pt"));
```

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```


Получает цвет линии сетки по умолчанию.

**Example**

```
         		GridWeb1.setDefaultGridLineColor(Color.getRed());
```

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getDisplayCellTip() {#getDisplayCellTip--}
```
public boolean getDisplayCellTip()
```


Получает, показывать ли подсказки. значение по умолчанию — true.

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


Получает режим редактирования элемента управления.

**Remarks**

Когда установлено значение true, ячейки управления редактируемы, и значки "save" и "undo" отображаются. Когда установлено значение false, ячейки управления только для чтения, и значки "save" и "undo" не отображаются.

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


Получает, использовать ли вызов AJAX. значение по умолчанию — true.

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


Получает, загружать ли данные ячеек асинхронно, рекомендуется использовать для листа с более чем 10000 ячейками

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


Получает, включены ли клиентские операции с колонками.

**Remarks**

Когда установлено значение true, пользователь может использовать контекстное меню правой кнопки мыши для добавления/удаления столбцов.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


Получает, включены ли клиентские операции заморозки.

**Remarks**

Когда установлено значение true, пользователь может использовать контекстное меню правой кнопки мыши для закрепления/открепления областей.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


Получает, включены ли клиентские операции слияния.

**Remarks**

Когда установлено значение true, пользователь может использовать контекстное меню правой кнопки мыши для объединения/разъединения ячеек.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


Получает, включено ли изменение размера колонок и строк на клиенте.

**Remarks**

Когда установлено значение true, пользователь может изменять размер столбцов и строк на клиенте.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


Получает, включены ли клиентские операции со строками.

**Remarks**

Когда установлено значение true, пользователь может использовать контекстное меню правой кнопки мыши для добавления/удаления строк.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


Получает, включено ли событие двойного щелчка со стороны клиента.

**Remarks**

Когда установлено значение true, элемент управления будет получать события двойного щелчка на стороне клиента, и вы можете обрабатывать эти события на сервере. В противном случае элемент управления будет игнорировать любые события двойного щелчка.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


Получает, применять ли металлический световой эффект.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


Получает, включен ли режим постраничного отображения элемента управления.

**Remarks**

Когда установлено значение true, элемент управления отобразит PageSize строк данных за один раз и покажет элемент выбора страницы на панели вкладок.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


Получает, включено ли диалоговое окно стилей на клиенте.

**Remarks**

Когда установлено значение true, пользователь может использовать диалоговое окно стилей для установки стиля ячейки, выбрав "Format Cell..." в всплывающем меню.

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


Получает Enabled в WebControl

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


Получает, включать ли постраничный вывод после фильтрации данных, будет применяться, когда EnablePaging равно true

**Remarks**

Когда установлено значение true, элемент управления будет выполнять постраничный вывод на основе отфильтрованных данных, значение по умолчанию — false.

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Получает Font в WebControl

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


Получает, принудительно ли выполнять проверку на стороне клиента.

**Remarks**

Когда установлено значение true, данные не будут отправляться на сервер, пока все поля ввода не станут валидными.

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Получает ForeColor в WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


Получает стиль рамки элемента управления.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


Получает, будет ли GridWeb выполнять операцию сохранения по умолчанию, значение по умолчанию — true.

**Returns:**
boolean
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


Получает высоту (System.Web.UI.WebControl.Unit) верхней панели заголовка элемента управления.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```


Получает стиль панели заголовка.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


Получает стиль панели заголовка элемента управления.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


Получает ширину ( System.Web.UI.WebControl.Unit ) или левую панель заголовка элемента управления.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Получает высоту ( System.Web.UI.WebControl.Unit ) элемента управления.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getIgnoreStyleWithNoData() {#getIgnoreStyleWithNoData--}
```
public boolean getIgnoreStyleWithNoData()
```


Получает, игнорирует ли GridWeb отображение строк или столбцов, которые не содержат значений ячеек, но имеют стиль. Если установлено значение true, производительность будет лучше. Значение по умолчанию — false, что означает, что если последняя последовательная строка/столбец не содержит значений ячеек, но имеет стиль, они всё равно будут отображаться. Эта опция действительна только когда EnableAsync равно false. Эта опция не влияет, когда EnableAsync равно true, что означает, что GridWeb покажет все строки/столбцы со стилем.

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


Представляет параметры загрузки для GridWeb.

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Получает максимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. Элемент управления использует большее значение из MaxColumn и максимального столбца данных листа.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Получает максимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Элемент управления использует большее значение из MaxRow и максимальной строки данных листа.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMessage() {#getMessage--}
```
public String getMessage()
```


Получает сообщение для сетки.

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Получает минимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. Элемент управления использует меньшее значение из MinColumn и минимального столбца данных листа.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Получает минимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Элемент управления использует меньшее значение из MinRow и минимальной строки данных листа.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getModifiedCells() {#getModifiedCells--}
```
public ArrayList getModifiedCells()
```


Получает коллекцию ячеек, изменённых клиентом.

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


Получает, следует ли отображать групповые строки.

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


Получает значение, указывающее, скрыта ли горизонтальная полоса прокрутки.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


Получает, следует ли отображать полосу прокрутки.

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


Получает значение, указывающее, скрыта ли вертикальная полоса прокрутки.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


Получает имя функции на клиенте, которая будет вызвана после завершения ajaxcall. Клиентская функция должна быть объявлена следующим образом:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


Получает имя функции на клиенте, которая будет вызвана при ошибке проверки ячейки. Клиентская функция должна быть объявлена следующим образом:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


Получает клиентскую функцию, которая будет вызвана, когда ячейка выбрана. Клиентскую функцию следует объявить следующим образом:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


Получает клиентскую функцию, которая будет вызвана, когда ячейка выбрана. Клиентскую функцию следует объявить следующим образом:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


Получает клиентскую функцию, которая будет вызвана, когда ячейка отменяет выбор. Клиентскую функцию следует объявить следующим образом:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


Получает имя клиентской функции, которая будет вызвана, когда значение ячейки обновляется. Клиентскую функцию следует объявить следующим образом:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


Получает клиентскую функцию, которая будет вызвана, когда будет показано контекстное меню. Клиентскую функцию следует объявить следующим образом:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


Получает клиентскую функцию, которая будет вызвана, когда ячейка двойным щелчком. Клиентскую функцию следует объявить следующим образом:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


Получает клиентскую функцию, которая будет вызвана, когда строка двойным щелчком. Клиентскую функцию следует объявить следующим образом:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


Получает имя клиентской функции, которая будет вызвана, когда сетка инициализируется. Клиентскую функцию следует объявить следующим образом:
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


Получает клиентскую функцию, которая будет вызвана после изменения индекса страницы. Действует только когда EnablePaging равно true. Клиентскую функцию следует объявить следующим образом:
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


Получает клиентскую функцию, вызываемую перед отправкой страницы на клиенте.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


Получает клиентскую функцию, которая будет вызвана при выборе фигуры. Клиентскую функцию следует объявить следующим образом:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


Получает клиентскую функцию, которая будет вызвана перед отправкой управления на клиенте. Клиентскую функцию следует объявить следующим образом:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
Параметр arg — это аргумент отправки, содержащий команду, которая будет передана на сервер. Параметр cancelEdit — булево значение, указывающее, отменил ли контроль ввод пользователя перед отправкой. Управление продолжит отправку, если функция вернёт true.
Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Получает, следует ли подгонять только строки, высота которых не задана пользователем; значение по умолчанию — false.

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


Получает размер страницы в режиме постраничного вывода.

**Remarks**

В режиме постраничного отображения контрол будет отображать PageSize строк данных один раз, и отображать элемент выбора страницы на панели вкладок.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


Получает путь хранения изображений для рабочей книги; все фигуры и изображения будут сохраняться в этом каталоге, путь по умолчанию — acwcache в базовом каталоге текущего приложения. Пользователи должны реализовать плановый сервис для очистки файлов, вышедших за пределы времени сессии.

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Получает предустановленный стиль.

Смотрите [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Example**

```
         		GridWeb1.setPresetStyle(PresetStyle.TRADITIONAL_1);
```

**Returns:**
int
### getRefreshValidation() {#getRefreshValidation--}
```
public boolean getRefreshValidation()
```


Получает, следует ли обновлять значение проверки после изменения значения ячейки.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


Получает, отображается ли скрытая строка в GridControl, значение по умолчанию — false. Если позже понадобится показать скрытую строку, установите значение true.

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


Получает значение высоты строки в пунктах для CSV‑файла; значение по умолчанию — 14,5.

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


Указывает цвет кнопки‑стрелки полосы прокрутки.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


Указывает цвет полосы прокрутки элемента управления.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


Указывает цвет фона выбранных ячеек в диапазоне множественного выбора.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


Указывает цвет выбранных ячеек в диапазоне множественного выбора.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCells() {#getSelectCells--}
```
public ArrayList getSelectCells()
```


Получает коллекцию выбранных ячеек.

**Returns:**
java.util.ArrayList
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


Получает путь к хранилищу кэша сеанса, когда режим сеанса — File или ViewState и т.д.: gridweb.SessionStorePath="c:/mytempdir/session"; тогда данные сеанса будут сохраняться в c:/mytempdir/session.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Представляет настройки рабочей книги.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


Получает, отображать ли кнопку добавления листа.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


Указывает, показывать ли панель команд (включая панель команд и вкладок) в нижней части элемента управления.

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


Определяет, отображает ли Gridweb панель инструментов редактирования, как в MS-EXCEL. Если включено, для текущей ячейки будет отображаться поле редактирования в Gridweb. При включении этой функции необходимо импортировать библиотеку jquery js в ваши файлы aspx для поддержки новой возможности. Подойдёт любая последняя версия jquery и т.д.

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


Указывает, показывать ли панель команд (включая панель команд и вкладок) в верхней части элемента управления.

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


Получает, отображать ли контекстное меню; значение по умолчанию — true.

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


Получает, отображать ли стандартные линии сетки ячеек.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


Получает, отображать ли строку заголовка.

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


Указывает, показывать ли диалоговое окно загрузки во время обратного вызова на сервер.

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


Указывает левую и верхнюю позицию (в пикселях) для отображения диалогового окна загрузки во время обратного вызова на сервер и т.д. 100,200 означает, что левый верхний угол окна загрузки находится на 100 px, 200 px.

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


Получает, отображать ли кнопку сохранения.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


Получает, показывать ли кнопку отправки.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


Получает, показывать ли панель вкладок.

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


Получает, отображается ли кнопка навигации по вкладкам, значение по умолчанию — true.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


Получает, показывать ли кнопку отмены.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


Указывает, переносить ли содержимое в диапазоне ячеек, значение по умолчанию — true.

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


Получает TabIndex в WebControl

**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


Получает стиль панели вкладок.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Получает ToolTip в WebControl

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


Получает, использует ли GridWeb высоту клиентской страницы в качестве высоты элемента управления, подходит, когда установлено Height=\"100%\", значение по умолчанию — false.

**Returns:**
boolean
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Получить версию релиза.

**Returns:**
java.lang.String - Версия выпуска.
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


Получает положение полосы прокрутки панели просмотра сетки.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


Получает положение полосы прокрутки панели просмотра сетки.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


Получает стиль панели просмотра данных.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Получает ширину (System.Web.UI.WebControl.Unit) элемента управления.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWorkSheets() {#getWorkSheets--}
```
public GridWorksheetCollection getWorkSheets()
```


Получает коллекцию листов.

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


Получает, использовать ли стиль XHTML, значение по умолчанию — true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream stream) {#importExcelFile-java.io.InputStream-}
```
public void importExcelFile(InputStream stream)
```


Импортирует из потока Excel‑файла, включая поток файлового диска или поток памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток Excel‑файла, включая поток с диска или поток в памяти. |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


Импортирует из потока Excel‑файла, включая поток файлового диска или поток памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток Excel‑файла, включая поток с диска или поток в памяти. |
| passwordtoOpen | java.lang.String | пароль для открытия зашифрованного файла. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Импортирует из Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя Excel‑файла. |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


Импортирует из Excel‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя Excel‑файла. |
| passwordtoOpen | java.lang.String | пароль для открытия зашифрованного файла. |

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


Получает, следует ли вычислять формулы после изменения значения ячейки или после импорта файла. Значение по умолчанию — true.

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


Загружает данные из потока CSV‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток файла. |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


Загружает данные из CSV‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла. |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


Загружает данные из потока HTML‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток файла. |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


Загружает данные из HTML‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла. |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


Загружает данные из потока файла SpreadSheetML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток файла. |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


Загружает данные из файла SpreadSheetML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```


Обновляет все изображения диаграмм для активного листа.

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


Сохраняет данные в поток CSV‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток файла. |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


Сохраняет данные в CSV‑файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| targetFile | java.lang.String | Имя файла. |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


Сохраняет текущие данные стиля управления в XML‑файл. Может использоваться для создания пользовательского файла стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла стиля. |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


Сохраняет данные в поток HTML‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток файла. |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


Сохраняет данные в HTML‑файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| targetFile | java.lang.String | Имя файла. |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


Сохраняет данные в поток файла SpreadSheetML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток файла. |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


Сохраняет данные в файл SpreadSheetML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| targetFile | java.lang.String | Имя файла. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Сохраняет листы в файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток для записи. |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


Сохраняет листы в файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток для записи. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Параметры сохранения. |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


Сохраняет листы в файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток для записи. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Формат файла (Excel2003, Excel2007, CSV, SpreadsheetML) |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


Сохраняет листы в файл Excel в формате Excel 2003.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| targetFile | java.lang.String | Имя целевого файла для записи. |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


Сохраняет листы в файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| targetFile | java.lang.String | Имя целевого файла для записи. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Параметры сохранения. |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


Сохраняет листы в файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| targetFile | java.lang.String | Имя целевого файла для записи. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Формат файла (Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


Устанавливает веб‑путь к скриптам/изображениям управления. Например: "http://localhost/acw\_client". Вы также можете задать это значение в файле web.config. Добавьте этот раздел в раздел `<configuration>`:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


Устанавливает веб‑URL файла языка управления. Например: "/acw\_client/lang\_en.js".
По умолчанию используется встроенный английский файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


Устанавливает активную ячейку текущего листа. Изменено, чтобы быть доступным для записи, начиная с версии 1.9.0.1.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


Задает цвет фона активной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


Задает цвет активной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


Задает цвет фона активного заголовка строки/столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


Задает цвет активного заголовка строки/столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Устанавливает индекс активного листа. Эквивалентно WebWorksheets.ActiveSheetIndex.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


Задает стиль активной вкладки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


Устанавливает, обновляется ли изображение диаграммы при изменении значения ячейки. По умолчанию true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Устанавливает BackColor в WebControl

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Устанавливает BorderColor в WebControl

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Устанавливает BorderStyle в WebControl

Смотрите [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Устанавливает BorderWidth в WebControl

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


Устанавливает стиль нижней панели элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Устанавливает, следует ли вычислять формулы после изменения значения ячейки или после импорта файла. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Устанавливает CssClass в WebControl

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


Устанавливает индекс текущей страницы в режиме постраничного вывода.

**Remarks**

В режиме постраничного отображения контрол будет отображать PageSize строк данных один раз, и отображать элемент выбора страницы на панели вкладок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


Представляет пользовательский движок вычислений для расширения движка вычислений по умолчанию в Aspose.Cells.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


Устанавливает пользовательский файл стилей из потока, включая файловый поток диска или поток памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток файла, включая поток с диска или поток в памяти. |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


Устанавливает имя пользовательского файла стилей.

**Remarks**

Пользовательский файл стиля является XML‑файлом. При установке имени файла он будет загружен немедленно. Ниже содержимое "standard preset style" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Получает/устанавливает DPI устройства.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Устанавливает имя шрифта по умолчанию для элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


Устанавливает размер шрифта по умолчанию для элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


Устанавливает цвет линий сетки по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


Устанавливает, показывать ли подсказки. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


Устанавливает режим редактирования элемента управления.

**Remarks**

Когда установлено значение true, ячейки управления редактируемы, и значки "save" и "undo" отображаются. Когда установлено значение false, ячейки управления только для чтения, и значки "save" и "undo" не отображаются.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


Устанавливает, использовать ли AJAX‑вызов. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


Устанавливает, загружать ли данные ячеек асинхронно, рекомендуется для листа с более чем 10000 ячейками.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


Устанавливает, включать ли клиентские операции со столбцами.

**Remarks**

Когда установлено значение true, пользователь может использовать контекстное меню правой кнопки мыши для добавления/удаления столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


Устанавливает, включать ли клиентские операции заморозки.

**Remarks**

Когда установлено значение true, пользователь может использовать контекстное меню правой кнопки мыши для закрепления/открепления областей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


Устанавливает, включать ли клиентские операции объединения.

**Remarks**

Когда установлено значение true, пользователь может использовать контекстное меню правой кнопки мыши для объединения/разъединения ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


Устанавливает, включено ли изменение размера столбцов и строк на клиенте.

**Remarks**

Когда установлено значение true, пользователь может изменять размер столбцов и строк на клиенте.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


Устанавливает, включены ли операции со строками на клиенте.

**Remarks**

Когда установлено значение true, пользователь может использовать контекстное меню правой кнопки мыши для добавления/удаления строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


Устанавливает, включено ли событие двойного щелчка на клиенте.

**Remarks**

Когда установлено значение true, элемент управления будет получать события двойного щелчка на стороне клиента, и вы можете обрабатывать эти события на сервере. В противном случае элемент управления будет игнорировать любые события двойного щелчка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


Устанавливает, применять ли эффект металлического света.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


Устанавливает, включён ли режим постраничного отображения управления.

**Remarks**

Когда установлено значение true, элемент управления отобразит PageSize строк данных за один раз и покажет элемент выбора страницы на панели вкладок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


Устанавливает, включён ли диалог стилей на клиенте.

**Remarks**

Когда установлено значение true, пользователь может использовать диалоговое окно стилей для установки стиля ячейки, выбрав "Format Cell..." в всплывающем меню.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Устанавливает Enabled в WebControl

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


Устанавливает, включено ли постраничное отображение после фильтрации данных, будет применяться, когда EnablePaging равно true.

**Remarks**

Когда установлено значение true, элемент управления будет выполнять постраничный вывод на основе отфильтрованных данных, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Устанавливает папку шрифтов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolder | java.lang.String | Папка, содержащая TrueType шрифты. |
| recursive | boolean | Определяет, сканировать ли подпапки. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Устанавливает папки шрифтов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Папки, содержащие TrueType шрифты. |
| recursive | boolean | Определяет, сканировать ли подпапки. |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


Устанавливает, принудительно ли выполнять проверку на клиенте.

**Remarks**

Когда установлено значение true, данные не будут отправляться на сервер, пока все поля ввода не станут валидными.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Устанавливает ForeColor в WebControl

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


Устанавливает стиль рамки управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


Устанавливает, будет ли GridWeb выполнять операцию сохранения по умолчанию, значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


Устанавливает высоту (System.Web.UI.WebControl.Unit) верхней панели заголовка управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


Устанавливает стиль панели заголовка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


Устанавливает стиль панели заголовка управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


Устанавливает ширину (System.Web.UI.WebControl.Unit) или левую панель заголовка управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Устанавливает высоту (System.Web.UI.WebControl.Unit) управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


Устанавливает, будет ли GridWeb игнорировать отображение строк или столбцов, не содержащих значения ячеек, но имеющих стиль. Если установить true, производительность будет лучше. Значение по умолчанию — false, что означает, что если последняя последовательная строка/столбец не имеет значений ячеек, но стилизована, мы всё равно отобразим её. Эта опция действительна только когда EnableAsync равно false. Эта опция не имеет эффекта, когда EnableAsync равно true, что означает, что GridWeb покажет все строки/столбцы со стилем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


Представляет параметры загрузки для GridWeb.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


Устанавливает максимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. Управление использует большее значение из MaxColumn и максимального столбца данных листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


Устанавливает максимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Управление использует большее значение из MaxRow и максимальной строки данных листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


Устанавливает сообщение для сетки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


Устанавливает минимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. Управление использует меньшее значение из MinColumn и минимального столбца данных листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


Устанавливает минимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Управление использует меньшее значение из MinRow и минимальной строки данных листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


Устанавливает, показывать ли группы строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


Устанавливает значение, указывающее, скрыта ли горизонтальная полоса прокрутки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


Устанавливает, показывать ли полосу прокрутки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


Устанавливает значение, указывающее, скрыта ли вертикальная полоса прокрутки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


Устанавливает имя функции на стороне клиента, вызываемой после завершения ajax‑вызова. Функцию клиента следует объявить следующим образом:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


Устанавливает имя функции на стороне клиента, вызываемой при ошибке проверки ячейки. Функцию клиента следует объявить следующим образом:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


Устанавливает функцию на стороне клиента, вызываемую при выборе ячейки. Функцию клиента следует объявить следующим образом:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


Устанавливает функцию на стороне клиента, вызываемую при выборе ячейки. Функцию клиента следует объявить следующим образом:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


Устанавливает функцию на стороне клиента, вызываемую при снятии выбора с ячейки. Функцию клиента следует объявить следующим образом:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


Устанавливает имя функции на стороне клиента, вызываемой при обновлении значения ячейки. Функцию клиента следует объявить следующим образом:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


Устанавливает функцию на стороне клиента, вызываемую при отображении контекстного меню. Функцию клиента следует объявить следующим образом:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


Устанавливает функцию на стороне клиента, вызываемую при двойном щелчке по ячейке. Функцию клиента следует объявить следующим образом:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


Устанавливает функцию на стороне клиента, вызываемую при двойном щелчке по строке. Функцию клиента следует объявить следующим образом:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


Устанавливает имя функции на стороне клиента, вызываемой при инициализации сетки. Функцию клиента следует объявить следующим образом:
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


Устанавливает функцию на стороне клиента, вызываемую после изменения индекса страницы. Действует только при EnablePaging = true. Функцию клиента следует объявить следующим образом:
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


Устанавливает функцию на клиентской стороне, вызываемую перед отправкой страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


Устанавливает функцию на стороне клиента, вызываемую при выборе фигуры. Функцию клиента следует объявить следующим образом:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


Устанавливает функцию клиента, вызываемую перед отправкой управления на стороне клиента. Функцию клиента следует объявить следующим образом:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
Параметр arg — это аргумент отправки, содержащий команду, которая будет передана на сервер. Параметр cancelEdit — булево значение, указывающее, отменил ли контроль ввод пользователя перед отправкой. Управление продолжит отправку, если функция вернёт true.
Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Устанавливает, следует ли подгонять только строки, высота которых не задана вручную; значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


Устанавливает размер страницы в режиме постраничного отображения.

**Remarks**

В режиме постраничного отображения контрол будет отображать PageSize строк данных один раз, и отображать элемент выбора страницы на панели вкладок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


Устанавливает путь хранения изображений для рабочей книги; все фигуры и изображения будут сохраняться в этом каталоге. Путь по умолчанию — acwcache в базовом каталоге текущего приложения. Пользователям необходимо реализовать плановый сервис для очистки файлов, срок действия которых истёк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Устанавливает предустановленный стиль.

Смотрите [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


Устанавливает, следует ли обновлять значение проверки после изменения значения ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


Устанавливает, будет ли скрытая строка отображаться в GridControl; значение по умолчанию — false. Если позже понадобится показать скрытую строку, установите значение true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


Устанавливает значение высоты строки в пунктах для CSV‑файла; значение по умолчанию — 14,5.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


Указывает цвет кнопки‑стрелки полосы прокрутки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


Указывает цвет полосы прокрутки элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


Указывает цвет фона выбранных ячеек в диапазоне множественного выбора.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


Указывает цвет выбранных ячеек в диапазоне множественного выбора.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


Устанавливает путь хранения кэша сеанса, когда режим сеанса — File или ViewState и т.д.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; тогда данные сеанса будут сохраняться в c:/mytempdir/session.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Представляет настройки рабочей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


Устанавливает, отображать ли кнопку добавления листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


Указывает, показывать ли панель команд (включая панель команд и вкладок) в нижней части элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


Определяет, отображает ли Gridweb панель инструментов редактирования, как в MS-EXCEL. Если включено, для текущей ячейки будет отображаться поле редактирования в Gridweb. При включении этой функции необходимо импортировать библиотеку jquery js в ваши файлы aspx для поддержки новой возможности. Подойдёт любая последняя версия jquery и т.д.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


Указывает, показывать ли панель команд (включая панель команд и вкладок) в верхней части элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


Устанавливает, отображать ли контекстное меню; значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


Устанавливает, отображать ли стандартные линии сетки ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


Устанавливает, отображать ли строку заголовка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


Указывает, показывать ли диалоговое окно загрузки во время обратного вызова на сервер.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


Указывает левую и верхнюю позицию (в пикселях) для отображения диалогового окна загрузки во время обратного вызова на сервер и т.д. 100,200 означает, что левый верхний угол окна загрузки находится на 100 px, 200 px.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


Устанавливает, показывать ли кнопку сохранения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


Устанавливает, показывать ли кнопку отправки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


Устанавливает, показывать ли панель вкладок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


Устанавливает, показывается ли кнопка навигации по вкладкам, значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


Устанавливает, показывать ли кнопку отмены.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


Указывает, переносить ли содержимое в диапазоне ячеек, значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


Устанавливает TabIndex в WebControl

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | short |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


Устанавливает стиль панели вкладок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Устанавливает ToolTip в WebControl

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


Устанавливает, использовать ли GridWeb высоту клиентской страницы в качестве высоты элемента управления, подходит, когда Height=\"100%\", значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


Устанавливает положение полосы прокрутки панели просмотра сетки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


Устанавливает положение полосы прокрутки панели просмотра сетки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


Устанавливает стиль панели просмотра данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Устанавливает ширину (System.Web.UI.WebControl.Unit) элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


Устанавливает, использовать ли стиль XHTML, значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

