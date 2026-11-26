---
title: "Класс GridWeb"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.GridWeb. Базовый класс управления GridWeb"
type: docs
url: /ru/net/aspose.cells.gridweb/gridweb/
---
## GridWeb class

Базовый класс управления GridWeb.

```csharp
public class GridWeb : MainWeb
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridWeb](gridweb/)() | этот конструктор. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Получает или задаёт активную ячейку текущего листа. Изменено, чтобы быть доступным для записи, начиная с версии 1.9.0.1.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Указывает цвет фона активной ячейки.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Указывает цвет активной ячейки.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Указывает цвет фона активного заголовка строки/столбца.(Inherited from [`MainWeb`](../mainweb/).) |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Указывает цвет активного заголовка строки/столбца.(Inherited from [`MainWeb`](../mainweb/).) |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Получает активный лист(Inherited from [`MainWeb`](../mainweb/).) |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Получает или задает индекс активного листа. Эквивалентно WebWorksheets.ActiveSheetIndex.(Inherited from [`MainWeb`](../mainweb/).) |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Указывает стиль активной вкладки.(Inherited from [`MainWeb`](../mainweb/).) |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Получает или задает веб‑путь к файлам скриптов/изображений элемента управления. Например: "http://localhost/acw_client". Вы также можете задать это значение в файле web.config. Добавьте этот раздел в раздел `<configuration>`:`<appSettings>``<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />``</appSettings>`(Inherited from [`MainWeb`](../mainweb/).) |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Получает или задает веб‑URL файла языка элемента управления. Например: "/acw_client/lang_en.js". По умолчанию используется встроенный английский файл.(Inherited from [`MainWeb`](../mainweb/).) |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Получает или задает, обновляется ли изображение диаграммы при изменении значения ячейки. По умолчанию true(Inherited from [`MainWeb`](../mainweb/).) |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Получает или задает стиль нижней панели элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Получает или задает текущий индекс страницы в режиме постраничного вывода.(Inherited from [`MainWeb`](../mainweb/).) |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Представляет пользовательский движок вычислений для расширения движка вычислений по умолчанию Aspose.Cells.(Inherited from [`MainWeb`](../mainweb/).) |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Получает коллекцию пользовательских кнопок команд(Inherited from [`MainWeb`](../mainweb/).) |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Получает или задает имя файла пользовательского стиля.(Inherited from [`MainWeb`](../mainweb/).) |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Получает или задает имя шрифта по умолчанию элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Получает или задает размер шрифта по умолчанию элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Получает или задает цвет линий сетки по умолчанию.(Inherited from [`MainWeb`](../mainweb/).) |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | Получает или задает, показывать ли подсказки. Значение по умолчанию true.(Inherited from [`MainWeb`](../mainweb/).) |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Получает или задает режим редактирования элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | Получает или задает, использовать ли AJAX‑вызов. Значение по умолчанию true.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Получает или задает, загружать ли данные ячеек асинхронно, рекомендуется для листа с более чем 10000 ячейками.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | Получает или задает, включить ли клиентские операции со столбцами.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | Получает или задает, включить ли клиентские операции заморозки.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | Получает или задает, включить ли клиентские операции объединения.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | Получает или задает, включить ли клиентское изменение размеров столбцов и строк.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | Получает или задает, включить ли клиентские операции со строками.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Получает или задает, включено ли событие двойного щелчка на стороне клиента.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Получает или задает, применять ли металлический световой эффект.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Получает или задает, включен ли режим постраничного отображения элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | Получает или задает, включен ли диалог стилей на стороне клиента.(Inherited from [`MainWeb`](../mainweb/).) |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Получает или задает, включено ли постраничное отображение после фильтрации данных, будет применяться, когда EnablePaging равно true.(Inherited from [`MainWeb`](../mainweb/).) |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Получает или задает, принудительно ли выполнять проверку на стороне клиента.(Inherited from [`MainWeb`](../mainweb/).) |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Получает или задает стиль рамки элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | Получает или задает, будет ли GridWeb выполнять операцию сохранения по умолчанию, значение по умолчанию — true.(Inherited from [`MainWeb`](../mainweb/).) |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Получает или задает высоту (System.Web.UI.WebControl.Unit) верхней панели заголовка элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Получает или задает стиль панели заголовка.(Inherited from [`MainWeb`](../mainweb/).) |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Получает или задает стиль панели заголовка элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Получает или задает ширину (System.Web.UI.WebControl.Unit) левой панели заголовка элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Получает или задает высоту (System.Web.UI.WebControl.Unit) элемента управления.(Inherited from [`MainWeb`](../mainweb/).) |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | Получает или задает, игнорирует ли GridWeb отображение строк или столбцов, не содержащих значения ячеек, но имеющих стиль. Если установить значение true, производительность будет лучше. Значение по умолчанию — false, что означает, что если последняя последовательная строка/столбец не содержит значений ячеек, но имеет стиль, они всё равно будут отображаться. Эта опция действительна только когда EnableAsync равно false. Эта опция не влияет, когда EnableAsync равно true, что означает, что GridWeb будет показывать все строки/столбцы со стилем.(Inherited from [`MainWeb`](../mainweb/).) |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Получает или задает, вычислять ли формулы после изменения значения ячейки или после импорта файла. Значение по умолчанию — true.(Inherited from [`MainWeb`](../mainweb/).) |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | Получает значение, указывающее, загружается ли GridWeb в ответ на постбэк клиента или загружается и используется впервые.(Inherited from [`MainWeb`](../mainweb/).) |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | Представляет параметры загрузки для GridWeb.(Inherited from [`MainWeb`](../mainweb/).) |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Получает или задает максимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. Элемент управления использует большее значение из MaxColumn и максимального столбца данных листа.(Inherited from [`MainWeb`](../mainweb/).) |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Получает или задает максимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Элемент управления использует большее значение из MaxRow и максимальной строки данных листа.(Inherited from [`MainWeb`](../mainweb/).) |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Получает или задает сообщение для сетки.(Inherited from [`MainWeb`](../mainweb/).) |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Получает или задает минимальный индекс отображаемого столбца (нумерация с нуля) веб‑листа. Элемент управления использует меньшее значение из MinColumn и минимального столбца данных листа.(Inherited from [`MainWeb`](../mainweb/).) |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Получает или задает минимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Элемент управления использует меньшее значение из MinRow и минимальной строки данных листа.(Inherited from [`MainWeb`](../mainweb/).) |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | Получает коллекцию ячеек, изменённых клиентом.(Inherited from [`MainWeb`](../mainweb/).) |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Получает или задает, отображать ли групповые строки.(Inherited from [`MainWeb`](../mainweb/).) |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Получает или задает значение, указывающее, скрыта ли горизонтальная полоса прокрутки.(Inherited from [`MainWeb`](../mainweb/).) |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Получает или задает, отображать ли полосу прокрутки. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Получает или задает значение, указывающее, скрыта ли вертикальная полоса прокрутки. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Получает или задает имя клиентской функции, вызываемой после завершения ajax‑вызова. Клиентская функция должна быть объявлена так: function GridAjaxcallFinished() { alert(this.id+" ajaxcall finished "); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Получает или задает имя клиентской функции, вызываемой при ошибке проверки ячейки. Клиентская функция должна быть объявлена так: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при выборе ячейки. Клиентская функция должна быть объявлена так: function MyOnSelectCellAjaxCallBack(cell,customerdata) { } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при выборе ячейки. Клиентская функция должна быть объявлена так: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при снятии выделения с ячейки. Клиентская функция должна быть объявлена так: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, "test"); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Получает или задает имя клиентской функции, вызываемой при обновлении значения ячейки. Клиентская функция должна быть объявлена так: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при отображении контекстного меню. Клиентская функция должна быть объявлена так: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при двойном щелчке по ячейке. Клиентская функция должна быть объявлена так: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при двойном щелчке по строке. Клиентская функция должна быть объявлена так: function MyOnRowDoubleClick(row) { alert(row); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Получает или задает имя клиентской функции, вызываемой при инициализации сетки. Клиентская функция должна быть объявлена так: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Получает или задает, подгонять ли только строки, высота которых не задана вручную; значение по умолчанию — false (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую после изменения индекса страницы. Действует только когда EnablePaging равно true. Клиентская функция должна быть объявлена так: function MyOnPageChange(index) { console.log("current page is:"+index); } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую перед отправкой страницы на клиенте. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую при выборе фигуры. Клиентская функция должна быть объявлена так: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") } Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | Получает или задает клиентскую функцию, вызываемую перед отправкой элемента управления на клиенте. Клиентская функция должна быть объявлена так: function MyOnSubmit(arg, cancelEdit) { return true;} Параметр arg – аргумент отправки, содержит команду, которая будет передана на сервер. Параметр cancelEdit – логическое значение, указывающее, отменил ли элемент управления ввод пользователя перед отправкой. Элемент управления продолжит отправку, если функция вернёт true. Примечание: Вы можете использовать указатель "this" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Получает или задает размер страницы в режиме постраничного отображения. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Получает или задает предустановленный стиль. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Получает или задает, следует ли обновлять значение проверки после изменения значения ячейки. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Получает или задает, отображается ли скрытая строка в GridControl, значение по умолчанию — false. Если позже понадобится показать скрытую строку, установите значение true. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | Получает или задает высоту строки в пунктах для CSV‑файла, значение по умолчанию — 14,5. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Указывает цвет кнопки‑стрелки полосы прокрутки. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Указывает цвет полосы прокрутки элемента управления. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Указывает цвет фона выбранных ячеек в диапазоне множественного выбора. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Указывает цвет выбранных ячеек в диапазоне множественного выбора. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [SelectCells](../../aspose.cells.gridweb/gridweb/selectcells/) { get; } | Получает коллекцию выбранных ячеек. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Получает или задает режим сеанса сетки. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Получает или задает путь к хранилищу кэша сеанса, когда режим сеанса — File или ViewState и т.д.: gridweb.SessionStorePath="c:/mytempdir/session"; тогда данные сеанса будут сохраняться в c:/mytempdir/session. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Представляет настройки рабочей книги. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Получает или задает, отображать ли кнопку добавления листа. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Указывает, показывать ли панель команд (включая панель команд и вкладок) в нижней части элемента управления. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | Отображать ли Gridweb панель инструментов редактирования, как в MS‑EXCEL. Если включено, для текущей ячейки будет отображаться поле редактирования в Gridweb. При включении этой функции необходимо подключить библиотеку jquery js в ваши файлы aspx для поддержки новой возможности. Подойдёт любая актуальная версия jquery и т.п. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Указывает, показывать ли панель команд (включая панель команд и вкладок) в верхней части элемента управления. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Получает или задает, отображать ли контекстное меню. Значение по умолчанию — true. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Получает или задает, отображать ли стандартные линии сетки ячеек. (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Получает или задает, отображать ли строку заголовка(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Указывает, отображать ли диалоговое окно загрузки во время обратного вызова к серверу.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Указывает левую и верхнюю позицию (в пикселях) для отображения диалогового окна загрузки во время обратного вызова к серверу и т.д. 100,200 означает, что левая и верхняя позиция диалогового окна загрузки находятся на 100px,200px .(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Получает или задает, отображать ли кнопку сохранения.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Получает или задает, отображать ли кнопку отправки.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Получает или задает, отображать ли панель вкладок.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Получает или задает, отображается ли кнопка навигации по вкладкам, значение по умолчанию — true.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Получает или задает, отображать ли кнопку отмены действий.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Указывает, переносить ли содержимое в диапазон ячеек, значение по умолчанию — true.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Получает или задает стиль панели вкладок.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | Получает или задает, использовать ли gridweb высоту клиентской страницы в качестве высоты элемента управления, подходит при установке Height="100%", значение по умолчанию — false(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Получает или задает позицию полосы прокрутки панели просмотра сетки.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Получает или задает позицию полосы прокрутки панели просмотра сетки.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Получает или задает стиль панели просмотра данных.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } | (Унаследовано от [`MainWeb`](../mainweb/).) |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Получает или задает ширину (System.Web.UI.WebControl.Unit) элемента управления.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Получает или задает коллекцию листов рабочей книги.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | Получает или задает, использовать ли стиль XHTML, значение по умолчанию — true.(Унаследовано от [`MainWeb`](../mainweb/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Вычисляет результат формул.(Унаследовано от [`MainWeb`](../mainweb/).) |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Привязывает элемент управления и все его дочерние контролы к его источнику данных.(Унаследовано от [`MainWeb`](../mainweb/).) |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() | (Унаследовано от [`MainWeb`](../mainweb/).) |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/)(Stream) | Импортирует из потока Excel‑файла, включая поток файлового диска или поток памяти.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/)(string) | Импортирует из Excel‑файла.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/)(Stream, string) | Импортирует из потока Excel‑файла, включая поток файлового диска или поток памяти.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/)(string, string) | Импортирует из Excel‑файла.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/)(Stream) | Загружает данные из потока CSV‑файла.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/)(string) | Загружает данные из CSV‑файла.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/)(Stream) | Загружает данные из потока HTML‑файла.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/)(string) | Загружает данные из HTML‑файла.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/)(Stream) | Загружает данные из потока файла SpreadSheetML.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/)(string) | Загружает данные из файла SpreadSheetML.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | Обновляет все изображения диаграмм для активного листа .(Унаследовано от [`MainWeb`](../mainweb/).) |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) | (Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/)(Stream) | Сохраняет данные в поток файла CSV.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/)(string) | Сохраняет данные в файл CSV.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/gridweb/savecustomstylefile/#savecustomstylefile)(string) | Сохраняет текущие данные стиля элемента управления в файл XML. Может использоваться для создания вашего пользовательского файла стиля. (2 метода) |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/)(Stream) | Сохраняет данные в поток файла HTML.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/)(string) | Сохраняет данные в файл HTML.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/)(Stream) | Сохраняет данные в поток файла SpreadSheetML.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/)(string) | Сохраняет данные в файл SpreadSheetML.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/)(Stream) | Сохраняет листы в файл Excel.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/)(string) | Сохраняет листы в файл Excel в формате Excel 2003.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/)(Stream, GridSaveFormat) | Сохраняет листы в файл Excel.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/)(Stream, GridSaveOptions) | Сохраняет листы в файл Excel.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/)(string, GridSaveFormat) | Сохраняет листы в файл Excel.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/)(string, GridSaveOptions) | Сохраняет листы в файл Excel.(Унаследовано от [`MainWeb`](../mainweb/).) |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | Устанавливает пользовательский файл стиля из потока, включая поток файлов на диске или поток памяти.(Унаследовано от [`MainWeb`](../mainweb/).) |
| static [GetVersion](../../aspose.cells.gridweb/gridweb/getversion/)() | Получить версию выпуска. |
| static [SetFontFolder](../../aspose.cells.gridweb/gridweb/setfontfolder/)(string, bool) | Устанавливает папку шрифтов |
| static [SetFontFolders](../../aspose.cells.gridweb/gridweb/setfontfolders/)(string[], bool) | Устанавливает папки шрифтов |

## События

| Имя | Описание |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Происходит после фильтрации столбца.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Срабатывает, когда обновление ajax элемента управления завершено.(EnableAJAX должен быть установлен в true)(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Происходит перед тем, как столбец будет отфильтрован.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Происходит, когда ячейка нажата, и требуется выполнить ajaxcallback для этого события.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | Происходит, когда происходит обновление ячейки клиента . Когда это событие срабатывает, его параметр e.Argument содержит имя команды.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Происходит, когда гиперссылка команды ячейки нажата. Когда это событие срабатывает, его параметр e.Argument содержит имя команды.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Происходит, когда ячейка двойным щелчком.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Происходит, когда ввод значения ячейки содержит ошибку.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Происходит, когда ячейка изменена в ajaxcall.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Происходит, когда пользователь удаляет столбец из контекстного меню клиента.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Происходит, когда пользователь пытается удалить столбец из контекстного меню клиента. Вы можете обработать это событие и установить параметр cancel в True, чтобы отменить операцию удаления.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Происходит, когда заголовок столбца двойным щелчком.(Унаследовано от [`MainWeb`](../mainweb/).) |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Происходит, когда пользователь вставляет столбец из клиентского меню. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Происходит, когда пользователь нажимает кнопку пользовательской команды. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Срабатывает, когда SessionMode элемента управления установлен в Custom и необходимо загрузить данные листа. Вы можете обработать это событие в режиме Custom Session, чтобы загрузить данные листа из файла или базы данных. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Происходит, когда изменился индекс страницы листа элемента управления. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Происходит, когда пользователь удалил строку из клиентского меню. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Происходит, когда пользователь пытается удалить строку из клиентского меню. Вы можете обработать это событие и вызвать исключение RejectDeleteException, чтобы отменить операцию удаления. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Происходит, когда заголовок строки двойным щелчком мыши. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Происходит, когда пользователь вставляет строку из клиентского меню. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | Происходит, когда нажата кнопка "save". (Наследовано от [`MainWeb`](../mainweb/).) |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Происходит, когда пользователь добавляет лист из меню панели инструментов. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Происходит, когда элемент управления загрузил отправленные данные и обновил данные листа. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Происходит, когда нажата вкладка листа. (Наследовано от [`MainWeb`](../mainweb/).) |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | Происходит, когда нажата кнопка "submit". (Наследовано от [`MainWeb`](../mainweb/).) |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | Происходит, когда нажата кнопка "undo". (Наследовано от [`MainWeb`](../mainweb/).) |

### См. также

* class [MainWeb](../mainweb/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


