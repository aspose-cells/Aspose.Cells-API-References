---
title: "Класс MainWeb"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.MainWeb. Родительский класс элемента управления GridWeb. Только для внутреннего использования"
type: docs
url: /ru/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Родительский класс управления GridWeb. Только для внутреннего использования.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MainWeb](mainweb/)() | Конструктор по умолчанию элемента управления MainWeb. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Получает или задает активную ячейку текущего листа. С версии 1.9.0.1 сделано доступным для записи. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Указывает цвет фона активной ячейки. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Указывает цвет активной ячейки. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Указывает цвет фона заголовка активной строки/столбца. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Указывает цвет заголовка активной строки/столбца. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Получает активный лист |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Получает или задает индекс активного листа. Эквивалентно WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Указывает стиль активной вкладки. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Получает или задает веб‑путь к скриптам/изображениям элемента управления. Например: "http://localhost/acw_client". Вы также можете задать это значение в файле web.config. Добавьте следующий раздел в секцию `<configuration>`:`<appSettings>``<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Получает или задает веб‑URL файла локализации элемента управления. Например: "/acw_client/lang_en.js". По умолчанию используется встроенный английский файл. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Получает или задает, обновляется ли изображение диаграммы при изменении значения ячейки. По умолчанию true. |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Получает или задает стиль нижней панели элемента управления. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Получает или задает текущий индекс страницы в режиме постраничного отображения. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Представляет пользовательский движок вычислений, расширяющий движок вычислений по умолчанию в Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Получает коллекцию пользовательских кнопок команд |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Получает или задает имя файла пользовательского стиля. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Получает или задает имя шрифта по умолчанию для элемента управления. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Получает или задает размер шрифта по умолчанию элемента управления. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Получает или задает цвет линии сетки по умолчанию. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | Получает или задает, показывать ли подсказки. значение по умолчанию — true. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Получает или задает режим редактирования элемента управления. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | Получает или задает, использовать ли вызов AJAX. значение по умолчанию — true. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Получает или задает, загружать ли данные ячеек асинхронно, рекомендуется использовать для листа с более чем 10000 ячейками. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | Получает или задает, включать ли операции с колонками на клиентской стороне. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | Получает или задает, включать ли операции заморозки на клиентской стороне. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | Получает или задает, включать ли операции объединения на клиентской стороне. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | Получает или задает, включать ли изменение размеров колонок и строк на клиентской стороне. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | Получает или задает, включать ли операции со строками на клиентской стороне. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Получает или задает, включать ли событие двойного щелчка на клиентской стороне. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Получает или задает, применять ли металлический световой эффект. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Получает или задает, включать ли режим постраничного отображения элемента управления. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | Получает или задает, включать ли диалоговое окно стилей на клиентской стороне. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Получает или задает, включать ли постраничный вывод после фильтрации данных, будет применяться, когда EnablePaging равно true. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Получает или задает, принудительно выполнять проверку на клиентской стороне. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Получает или задает стиль рамки элемента управления. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | Получает или задает, будет ли GridWeb выполнять операцию сохранения по умолчанию, значение по умолчанию — true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Получает или задает высоту (System.Web.UI.WebControl.Unit) верхней панели заголовка элемента управления. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Получает или задает стиль панели заголовка. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Получает или задает стиль панели заголовка элемента управления. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Получает или задает ширину( System.Web.UI.WebControl.Unit ) или левую панель заголовка элемента управления. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Получает или задает высоту( System.Web.UI.WebControl.Unit ) элемента управления. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | Получает или задает, игнорирует ли GridWeb отображение строк или столбцов, которые не содержат значений ячеек, но имеют стиль. Если установить значение true, производительность будет лучше. Значение по умолчанию — false, что означает, что если последняя последовательная строка/столбец не содержит значений ячеек, но имеет стиль, они всё равно будут отображаться. Эта опция действительна только когда EnableAsync равно false. Эта опция не влияет, когда EnableAsync равно true, что означает, что GridWeb будет показывать все строки/столбцы со стилем. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Получает или задает, вычислять ли формулы после изменения значения ячейки или после импорта файла. Значение по умолчанию — true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | Получает значение, указывающее, загружается ли gridweb в ответ на постбэк клиента или загружается и используется впервые. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | Представляет параметры загрузки для GridWeb. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Получает или задает максимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. Элемент управления использует большее значение из MaxColumn и максимального столбца данных листа. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Получает или задает максимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Элемент управления использует большее значение из MaxRow и максимальной строки данных листа. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Получает или задает сообщение для сетки. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Получает или задает минимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. Элемент управления использует меньшее значение из MinColumn и минимального столбца данных листа. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Получает или задает минимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Элемент управления использует меньшее значение из MinRow и минимальной строки данных листа. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | Получает коллекцию ячеек, изменённых клиентом. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Получает или задает, отображать ли grouprows. |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Получает или задает значение, указывающее, скрыта ли горизонтальная полоса прокрутки. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Получает или задает, отображать ли полосу прокрутки. |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Получает или задает значение, указывающее, скрыта ли вертикальная полоса прокрутки. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Получает или задает имя клиентской функции, вызываемой после завершения ajaxcall. Клиентская функция должна быть объявлена так: function GridAjaxcallFinished() { alert(this.id+\" ajaxcall finished \"); } Примечание: вы можете использовать указатель \"this\" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Получает или задает имя клиентской функции, вызываемой при ошибке проверки ячейки. Клиентская функция должна быть объявлена так: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); } Примечание: вы можете использовать указатель \"this\" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при выборе ячейки. Клиентская функция должна быть объявлена так: function MyOnSelectCellAjaxCallBack(cell,customerdata) { } Примечание: вы можете использовать указатель \"this\" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при выборе ячейки. Клиентская функция должна быть объявлена так: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, \"test\"); } Примечание: вы можете использовать указатель \"this\" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при снятии выделения с ячейки. Клиентская функция должна быть объявлена так: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, \"test\"); } Примечание: вы можете использовать указатель \"this\" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Получает или задает имя клиентской функции, вызываемой при обновлении значения ячейки. Клиентская функция должна быть объявлена так: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Примечание: вы можете использовать указатель \"this\" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | Получает или задает клиентскую функцию, которая будет вызываться при отображении контекстного меню. Клиентская функция должна быть объявлена так: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility(\"Delete\", \"block\"); menu.setItemVisibility(\"Update\", \"none\"); }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Получает или задает клиентскую функцию, которая будет вызываться при двойном щелчке по ячейке. Клиентская функция должна быть объявлена так: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, \"test\"); }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Получает или задает клиентскую функцию, которая будет вызываться при двойном щелчке по строке. Клиентская функция должна быть объявлена так: function MyOnRowDoubleClick(row) { alert(row); }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Получает или задает имя клиентской функции, которая будет вызываться при инициализации сетки. Клиентская функция должна быть объявлена так: function MyOnGridInit(grid) { alert(\"The grid is initialized: \" + grid.id); }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Получает или задает, следует ли подгонять только строки, высота которых не задана пользователем; значение по умолчанию — false. |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Получает или задает клиентскую функцию, которая будет вызываться после изменения индекса страницы. Работает только при EnablePaging = true. Клиентская функция должна быть объявлена так: function MyOnPageChange(index) { console.log(\"current page is:\"+index); }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую перед отправкой страницы на клиенте. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Получает или задает клиентскую функцию, которая будет вызываться при выборе фигуры. Клиентская функция должна быть объявлена так: function MyOnSelectShape(shape) { var name=shape.getAttribute(\"namevalue\") var text=shape.getAttribute(\"textvalue\") var value=shape.getAttribute(\"controlvalue\") var type=shape.getAttribute(\"msotype\") }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую перед отправкой управления на клиенте. Клиентская функция должна быть объявлена так: function MyOnSubmit(arg, cancelEdit) { return true;} Параметр arg – аргумент отправки, содержит команду, которая будет передана на сервер. Параметр cancelEdit – логическое значение, указывающее, отменил ли контроль ввод пользователя перед отправкой. Управление продолжит отправку, если функция вернёт true. Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Получает или задает размер страницы в режиме постраничного отображения. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Получает или задает предустановленный стиль. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Получает или задает, следует ли обновлять значение проверки после изменения значения ячейки. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Получает или задает, отображается ли скрытая строка в GridControl; значение по умолчанию — false. Если позже потребуется показать скрытую строку, установите значение true. |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | Получает или задает высоту строки в пунктах для CSV‑файла; значение по умолчанию — 14,5. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Указывает цвет кнопки‑стрелки полосы прокрутки. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Указывает цвет полосы прокрутки элемента управления. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Указывает цвет фона выбранных ячеек в диапазоне множественного выбора. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Указывает цвет выбранных ячеек в диапазоне множественного выбора. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Получает или задает режим сеанса сетки. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Получает или задает путь к хранилищу кэша сеанса, когда режим сеанса установлен в File или ViewState и т.д.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; тогда данные сеанса будут сохраняться в c:/mytempdir/session. |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Представляет настройки рабочей книги. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Получает или задает, отображать ли кнопку добавления листа. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Указывает, показывать ли панель команд (включая панель команд и вкладок) в нижней части элемента управления. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | Отображает ли Gridweb панель инструментов редактирования, как в MS‑EXCEL. Если включено, для текущей ячейки будет отображаться поле редактирования в Gridweb. При включении этой функции необходимо импортировать библиотеку jquery js в ваши файлы aspx для поддержки новой возможности; подходит любая актуальная версия jquery и т.п. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Указывает, следует ли отображать панель команд (включает панель команд и панель вкладок) в верхней части элемента управления. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Получает или задает, следует ли отображать контекстное меню. Значение по умолчанию — true. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Получает или задает, следует ли отображать стандартные линии сетки ячеек. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Получает или задает, следует ли отображать строку заголовка. |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Указывает, следует ли показывать диалоговое окно загрузки во время обратного вызова на сервер. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Указывает левую и верхнюю позицию (в пикселях) для отображения диалогового окна загрузки во время обратного вызова на сервер и т.д. 100,200 означает, что левая и верхняя позиция диалогового окна загрузки находятся на 100 px и 200 px. |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Получает или задает, следует ли отображать кнопку сохранения. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Получает или задает, следует ли отображать кнопку отправки. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Получает или задает, следует ли отображать панель вкладок. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Получает или задает, отображается ли кнопка навигации по вкладкам; значение по умолчанию — true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Получает или задает, следует ли отображать кнопку отмены. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Указывает, следует ли переносить содержимое в диапазоне ячеек. Значение по умолчанию — true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Получает или задает стиль панели вкладок. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | Получает или задает, использовать ли GridWeb высоту клиентской страницы в качестве высоты элемента управления; подходит, когда установлено Height="100%", значение по умолчанию — false. |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Получает или задает позицию полосы прокрутки панели просмотра сетки. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Получает или задает позицию полосы прокрутки панели просмотра сетки. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Получает или задает стиль панели просмотра данных. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Получает или задает ширину (System.Web.UI.WebControl.Unit) элемента управления. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Получает или задает коллекцию листов. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | Получает или задает, использовать ли стиль XHTML; значение по умолчанию — true. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | Получает/устанавливает DPI устройства. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | Получает или задает путь хранения изображений для рабочей книги; все фигуры и изображения будут сохраняться в этом каталоге, путь по умолчанию — acwcache в базовом каталоге текущего приложения. Пользователи должны реализовать плановый сервис для очистки файлов, срок действия которых истёк. |

## Методы

| Имя | Описание |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Вычисляет результат формул. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Привязывает элемент управления и все его дочерние элементы к его источнику данных. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | Импортирует из потока Excel‑файла, включая поток с диска или поток памяти. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | Импортирует из Excel‑файла. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | Импортирует из потока Excel‑файла, включая поток с диска или поток памяти. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | Импортирует из Excel‑файла. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | Загружает данные из потока CSV‑файла. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | Загружает данные из CSV‑файла. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | Загружает данные из потока HTML‑файла. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | Загружает данные из HTML‑файла. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Загружает данные из потока файла SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Загружает данные из файла SpreadSheetML. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | Обновляет все изображения диаграмм для активного листа. |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | Сохраняет данные в поток CSV‑файла. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | Сохраняет данные в CSV‑файл. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | Сохраняет текущие данные стиля элемента управления в XML‑файл. Может использоваться для создания пользовательского файла стиля. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | Сохраняет данные в поток HTML‑файла. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | Сохраняет данные в HTML‑файл. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Сохраняет данные в поток файла SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Сохраняет данные в файл SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | Сохраняет листы в Excel‑файл. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | Сохраняет листы в Excel‑файл в формате Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Сохраняет листы в Excel‑файл. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | Сохраняет листы в Excel‑файл. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | Сохраняет листы в Excel‑файл. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | Сохраняет листы в Excel‑файл. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | Устанавливает пользовательский файл стиля из потока, включая поток файлов с диска или поток памяти. |

## События

| Имя | Описание |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Происходит после фильтрации столбца. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Срабатывает, когда обновление ajax элемента управления завершено (необходимо установить EnableAJAX в значение true). |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Происходит перед фильтрацией столбца. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Происходит при щелчке по ячейке, и необходимо выполнить ajaxcallback для этого события. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | Происходит, когда происходит обновление ячейки на клиенте. Когда это событие срабатывает, его параметр e.Argument содержит имя команды. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Происходит, когда нажата гиперссылка команды ячейки. Когда это событие срабатывает, его параметр e.Argument содержит имя команды. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Происходит при двойном щелчке по ячейке. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Происходит, когда ввод значения в ячейке содержит ошибку. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Происходит, когда ячейка изменяется в ajax‑вызове. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Происходит, когда пользователь удаляет столбец из контекстного меню на клиенте. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Происходит, когда пользователь пытается удалить столбец из контекстного меню на клиенте. Вы можете обработать это событие и установить параметр cancel в значение True, чтобы отменить операцию удаления. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Происходит при двойном щелчке по заголовку столбца. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Происходит, когда пользователь вставляет столбец из контекстного меню на клиенте. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Происходит, когда пользователь нажимает кнопку пользовательской команды. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Срабатывает, когда свойство SessionMode элемента управления установлено в Custom и требуется загрузить данные листа. Вы можете обработать это событие в режиме Custom Session для загрузки данных листа из файла или базы данных. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Происходит, когда изменяется индекс страницы листа элемента управления. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Происходит, когда пользователь удалил строку из контекстного меню на клиенте. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Происходит, когда пользователь пытается удалить строку из контекстного меню на клиенте. Вы можете обработать это событие и бросить исключение RejectDeleteException, чтобы отменить операцию удаления. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Происходит при двойном щелчке по заголовку строки. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Происходит, когда пользователь вставляет строку из контекстного меню на клиенте. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | Происходит, когда нажата кнопка "save". |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Происходит, когда пользователь добавляет лист из меню панели инструментов. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Происходит, когда элемент управления загрузил отправленные данные и обновил данные листа. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Происходит, когда нажата вкладка листа. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | Происходит, когда нажата кнопка "submit". |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | Происходит, когда нажата кнопка "undo". |

### Примеры

```csharp
[C#]
	GridWeb GridWeb1 = new GridWeb();
//выполняйте свою работу
```

### См. также

* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


