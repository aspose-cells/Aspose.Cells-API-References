---
title: MainWeb
second_title: Справочник по Aspose.Cells для .NET API
description: Родительский класс элемента управления GridWeb. Только для внутреннего использования.
type: docs
weight: 850
url: /ru/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Родительский класс элемента управления GridWeb. Только для внутреннего использования.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MainWeb](mainweb)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell) { get; set; } | Получает или задает активную ячейку текущего листа. Изменено, чтобы быть доступным для записи, начиная с версии 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor) { get; set; } | Указывает цвет фона активной ячейки. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor) { get; set; } | Указывает цвет активной ячейки. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor) { get; set; } | Указывает цвет фона активного заголовка строки/столбца. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor) { get; set; } | Определяет цвет заголовка активной строки/столбца. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet) { get; } | Получает активный лист |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex) { get; set; } | Получает или задает индекс активного листа. Равен WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle) { get; set; } | Определяет стиль активной вкладки. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath) { get; set; } | Получает или задает веб-путь к файлам сценариев/изображений элемента управления. Например: "http://localhost/acw_client". Вы также можете установить это значение в файле web.config. Добавьте этот раздел в раздел &lt;configuration&gt;: &lt;Настройки приложения&gt;&lt;add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" /&gt;&lt;/Настройки приложения&gt; |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl) { get; set; } | Получает или задает URL-адрес языкового файла элемента управления. Например: "/acw_client/lang_en.js". По умолчанию используется встроенный английский файл. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart) { get; set; } | Получает или задает, обновляется ли изображение диаграммы при обновлении значения ячейки. Значение по умолчанию — true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle) { get; set; } | Получает или задает стиль нижней панели элемента управления. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex) { get; set; } |  |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine) { get; set; } | Представляет пользовательский механизм расчета для расширения механизма расчета по умолчанию Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons) { get; } |  |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename) { get; set; } | Получает или задает имя файла пользовательского стиля. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname) { get; set; } | Получает или задает имя шрифта элемента управления по умолчанию. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize) { get; set; } | Получает или задает размер шрифта элемента управления по умолчанию. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor) { get; set; } | Получает или задает цвет линии сетки по умолчанию. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip) { get; set; } |  |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode) { get; set; } | Получает или задает режим редактирования элемента управления. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax) { get; set; } |  |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync) { get; set; } | Получает или задает данные ячеек нагрузки асинхронным способом, предлагает применить для одного листа с более чем 10000 ячеек. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations) { get; set; } | Получает или задает, следует ли включить операции со столбцами на стороне клиента. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze) { get; set; } | Получает или задает, следует ли включить операции заморозки на стороне клиента. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations) { get; set; } | Получает или задает, следует ли включить операции слияния на стороне клиента. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow) { get; set; } | Получает или задает, следует ли включить изменение размера столбца и строки на стороне клиента. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations) { get; set; } | Получает или задает, следует ли включить операции со строками на стороне клиента. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent) { get; set; } | Получает или задает, следует ли включить событие двойного щелчка на стороне клиента. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect) { get; set; } | Получает или задает применение эффекта металлического света. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging) { get; set; } | Получает или задает, следует ли включить режим пейджинга элемента управления. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox) { get; set; } | Получает или задает, следует ли включить диалоговое окно стиля на стороне клиента. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging) { get; set; } | Получает или задает, следует ли включить разбиение по страницам после фильтрации данных, вступит в силу, когда EnablePaging имеет значение true. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation) { get; set; } | Получает или задает необходимость принудительной проверки на стороне клиента. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle) { get; set; } | Получает или задает стиль рамки элемента управления. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation) { get; set; } | Получает или задает, будет ли GridWeb выполнять операцию сохранения по умолчанию, значение по умолчанию — true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight) { get; set; } | Получает или задает высоту ( System.Web.UI.WebControl.Unit ) верхней панели заголовка элемента управления. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle) { get; set; } | Получает или задает стиль панели заголовка. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle) { get; set; } | Получает или задает стиль панели заголовка элемента управления. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth) { get; set; } | Получает или задает ширину ( System.Web.UI.WebControl.Unit ) или левый заголовок элемента управления. |
| override [Height](../../aspose.cells.gridweb/mainweb/height) { get; set; } | Получает или задает высоту ( System.Web.UI.WebControl.Unit ) элемента управления. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula) { get; set; } | Получает или задает, следует ли вычислять формулу после изменения значения ячейки или после импорта файла. Значение по умолчанию — true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback) { get; } | Получает значение, указывающее, загружается ли gridweb в ответ на клиентскую обратную передачу, или загружается и к ней обращаются в первый раз. |
| [LinksTable](../../aspose.cells.gridweb/mainweb/linkstable) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn) { get; set; } | Получает или задает максимальный индекс отображаемого столбца (начиная с нуля) веб-листа. Элемент управления использует большее значение MaxColumn и максимального столбца данных листа. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow) { get; set; } | Получает или задает максимальный индекс отображаемой строки (начиная с нуля) веб-листа. Элемент управления использует большее значение MaxRow и максимальную строку данных листа. |
| [Message](../../aspose.cells.gridweb/mainweb/message) { get; set; } |  |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn) { get; set; } |  |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow) { get; set; } | Получает или задает минимальный индекс отображаемой строки (начиная с нуля) веб-листа. Элемент управления использует меньшее значение MinRow и минимальную строку данных листа. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells) { get; } | Получает коллекцию ячеек, измененных клиентом. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows) { get; set; } | Получает или задает, показывать ли групповые строки . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll) { get; set; } | Получает или задает значение, указывающее, скрыта ли горизонтальная полоса прокрутки. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll) { get; set; } |  |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll) { get; set; } | Получает или задает значение, указывающее, скрыта ли вертикальная полоса прокрутки. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction) { get; set; } | Получает или задает имя функции на стороне клиента, которая будет вызываться после завершения ajaxcall. Функция клиента должна быть объявлена следующим образом: функция GridAjaxcallFinished() { alert(this.id+"вызов ajax завершен"); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction) { get; set; } | Получает или задает имя функции на стороне клиента, которая будет вызываться, когда проверка ячейки не пройдена. Функция клиента должна быть объявлена следующим образом: функция MyOnCellError (ячейка) { оповещение (GridWeb1.getCellValueByCell (ячейка)); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction) { get; set; } | Получает или задает функцию на стороне клиента, которая будет вызываться при выборе ячейки. Функция клиента должна быть объявлена следующим образом: функция MyOnSelectCellAjaxCallBack (ячейка, данные клиента) { } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction) { get; set; } | Получает или задает функцию на стороне клиента, которая будет вызываться при выборе ячейки. Функция клиента должна быть объявлена следующим образом: функция MyOnSelectCell (ячейка) { GridWeb1.setCellValueByCell (ячейка, «тест»); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction) { get; set; } | Получает или задает функцию на стороне клиента, которая будет вызываться, когда ячейка не выбрана. Функция клиента должна быть объявлена следующим образом: функция MyOnUnselectCell (ячейка) { GridWeb1.setCellValueByCell (ячейка, «тест»); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction) { get; set; } | Получает или задает имя функции на стороне клиента, которая будет вызываться при обновлении значения ячейки. Функция клиента должна быть объявлена следующим образом: функция MyOnCellUpdated (ячейка) { оповещение (this.getCellValueByCell (ячейка)); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction) { get; set; } | Получает или задает функцию на стороне клиента, которая будет вызываться при отображении контекстного меню. Функция клиента должна быть объявлена следующим образом: функция onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Удалить", "блокировать"); menu.setItemVisibility ("Обновить", "нет"); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction) { get; set; } | Получает или задает функцию на стороне клиента, которая будет вызываться при двойном щелчке по ячейке. Функция клиента должна быть объявлена следующим образом: функция MyOnDoubleClickCell (ячейка) { GridWeb1.setCellValueByCell (ячейка, «тест»); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction) { get; set; } | Получает или задает функцию на стороне клиента, которая будет вызываться при двойном щелчке строки. Функция клиента должна быть объявлена следующим образом: функция MyOnRowDoubleClick(строка) { предупреждение (строка); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction) { get; set; } | Получает или задает имя функции на стороне клиента, которая будет вызываться при инициализации сетки. Функция клиента должна быть объявлена следующим образом: функция MyOnGridInit(сетка) { alert("Сетка инициализирована: " + grid.id); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto) { get; set; } | Получает или задает, подходят ли только строки, высота которых не настроена пользователем, значение по умолчанию — false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction) { get; set; } | Получает или задает функцию на стороне клиента, которая будет вызываться после изменения индекса страницы. Действует, только если EnablePaging имеет значение true. Функция клиента должна быть объявлена следующим образом: функция MyOnPageChange (индекс) { console.log("текущая страница:"+index); } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction) { get; set; } | Получает или задает функцию клиента, которая будет вызываться перед отправкой страницы на стороне клиента. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction) { get; set; } | Получает или задает функцию на стороне клиента, которая будет вызываться при выборе фигуры. Функция клиента должна быть объявлена следующим образом: функция MyOnSelectShape (форма) { var name=shape.getAttribute("имязначение") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") } Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction) { get; set; } | Получает или задает клиентскую функцию, которая будет вызываться перед отправкой элемента управления на стороне клиента. Клиентская функция должна быть объявлена следующим образом: функция MyOnSubmit(arg, cancelEdit) { вернуть истину;} Аргумент — это аргумент отправки, содержащий команду для отправки на сервер. Значение cancelEdit — логическое значение, указывающее, отклонил ли элемент управления пользовательский ввод перед отправкой. Элемент управления продолжит отправку, если функция возвращает значение true.  Примечание. Вы можете использовать указатель «this» в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize) { get; set; } | Получает или задает размер страницы в режиме подкачки. |
| [PicturesTable](../../aspose.cells.gridweb/mainweb/picturestable) { get; } |  |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle) { get; set; } | Получает или задает предустановленный стиль. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation) { get; set; } | Получает или задает, следует ли обновлять значение проверки после изменения значения ячейки. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow) { get; set; } | Получает или задает, отображается ли скрытая строка в GridControl, значение по умолчанию — false. , если вам нужно отобразить скрытую строку позже, вы должны установить ее как true |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor) { get; set; } | Определяет цвет кнопки со стрелкой полосы прокрутки. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor) { get; set; } | Определяет цвет полосы прокрутки элемента управления. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor) { get; set; } | Указывает цвет фона выбранных ячеек в диапазоне множественного выбора. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor) { get; set; } | Указывает цвет выбранных ячеек в диапазоне множественного выбора. |
| [SessionLoaded](../../aspose.cells.gridweb/mainweb/sessionloaded) { get; set; } |  |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode) { get; set; } | Получает или устанавливает режим сеанса сетки. Существует 4 типа режима сеанса: 1. Сеанс (по умолчанию): Используйте системный сеанс для хранения данных листа. Обычно asp.net использует состояние сеанса InProc. Сетка также поддерживает состояние сеанса State процесса StateServer и состояние сеанса SQLServer. 2. ViewState: используйте состояние просмотра страницы для хранения данных листа. 3. Пользовательский: используйте события LoadCustomData и SheetDataUpdated для сохранения/восстановления данных листа. 4. Файл: сохранение/восстановление данных листа в SessionStorePath. |
| [SessionSaved](../../aspose.cells.gridweb/mainweb/sessionsaved) { get; set; } |  |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath) { get; set; } | Получает или задает путь к хранилищу кэша сеанса, когда режим сеанса — File или ViewState, и т. д.: gridweb.SessionStorePath="c:/mytempdir/session"; , тогда он будет хранить данные сеанса в c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings) { get; set; } | Представляет параметры книги. |
| [ShapesTable](../../aspose.cells.gridweb/mainweb/shapestable) { get; } |  |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton) { get; set; } | Получает или задает, показывать ли кнопку добавления рабочего листа. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar) { get; set; } |  |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox) { get; set; } | показывает ли Gridweb панель инструментов поля редактирования, как в MS-EXCEL. Если включено, поле редактирования для текущей ячейки будет отображаться в Gridweb. если мы включим эту функцию, нам нужно импортировать библиотеку jquery js в ваши файлы aspx для поддержки этой новой функции. все последние версии jquery в порядке. и т.п. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop) { get; set; } | Указывает, показывать ли панель команд (включая панель команд и панель вкладок) в верхней части элемента управления. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu) { get; set; } |  |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline) { get; set; } | Получает или задает, отображать ли линии сетки ячеек по умолчанию. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar) { get; set; } |  |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading) { get; set; } | Указывает, показывать ли диалоговое окно загрузки при обратной передаче на сервер. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition) { get; set; } | Указывает левое, верхнее положение (в пикселях) для отображения диалогового окна загрузки при обратной передаче на сервер и т. д. 100 200 означает, что диалоговое окно загрузки находится слева, верхняя позиция находится на уровне 100 пикселей, 200 пикселей . |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton) { get; set; } | Получает или задает, показывать ли кнопку сохранения. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton) { get; set; } | Получает или задает, показывать ли кнопку отправки. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar) { get; set; } |  |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation) { get; set; } | Получает или задает, отображается ли кнопка навигации по вкладкам, значение по умолчанию — true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton) { get; set; } | Получает или задает, показывать ли кнопку отмены. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap) { get; set; } | Указывает, следует ли переносить содержимое в диапазон ячеек. Значение по умолчанию — true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle) { get; set; } | Получает или задает стиль панели вкладок. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight) { get; set; } | Получает или задает, будет ли gridweb использовать высоту клиентской страницы в качестве высоты элемента управления, подходит, когда установлено значение Height = "100%", значение по умолчанию — false |
| [ValidationsTable](../../aspose.cells.gridweb/mainweb/validationstable) { get; } |  |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft) { get; set; } | Получает или задает положение полосы прокрутки панели просмотра сетки. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop) { get; set; } | Получает или задает положение полосы прокрутки панели просмотра сетки. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle) { get; set; } | Получает или задает стиль панели просмотра данных. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width) { get; set; } | Получает или задает ширину ( System.Web.UI.WebControl.Unit ) элемента управления. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets) { get; } |  |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode) { get; set; } |  |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath) { get; set; } | Получает или задает путь хранения изображений для книги, все фигуры и изображения будут храниться в этом каталоге, путь по умолчанию — acwcache в текущем базовом каталоге приложения. пользователям необходимо внедрить службу расписания для очистки отсутствующих файлов. времени сеанса. |

## Методы

| Имя | Описание |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula)() | Вычисляет результат формул. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind)() | Привязать элемент управления и все его дочерние элементы управления к его источнику данных. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile)(Stream) | Импорт из потока файлов Excel, включая поток файлов на диске или поток памяти. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile_1)(string) | Импорт из файла Excel. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile)(Stream) | Загружает данные из потока файла CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile_1)(string) | Загружает данные из файла CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile)(Stream) | Загружает данные из потока файла HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile_1)(string) | Загружает данные из файла HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile)(Stream) | Загружает данные из файлового потока SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile_1)(string) | Загружает данные из файла SpreadSheetML. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape)() | обновить все изображения диаграммы для активного листа . |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile)(Stream) | Сохраняет данные в поток файла CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile_1)(string) | Сохраняет данные в файл CSV. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile)(string) | Сохраняет данные текущего стиля элемента управления в XML-файл. Может использоваться для создания файла пользовательского стиля. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile)(Stream) | Сохраняет данные в файловый поток HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile_1)(string) | Сохраняет данные в файл HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile)(Stream) | Сохраняет данные в файловый поток SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile_1)(string) | Сохраняет данные в файл SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile)(Stream) | Сохраняет рабочие листы в файл Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_3)(string) | Сохраняет листы в файл Excel в формате Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_1)(Stream, GridSaveFormat) | Сохраняет рабочие листы в файл Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_2)(Stream, GridSaveOptions) | Сохраняет рабочие листы в файл Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_4)(string, GridSaveFormat) | Сохраняет рабочие листы в файл Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_5)(string, GridSaveOptions) | Сохраняет рабочие листы в файл Excel. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle)(Stream) | задает файл пользовательского стиля из потока, включая поток файлов на диске или поток памяти. |

### Смотрите также

* class [ExtWebControl](../extwebcontrol)
* пространство имен [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* сборка [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
