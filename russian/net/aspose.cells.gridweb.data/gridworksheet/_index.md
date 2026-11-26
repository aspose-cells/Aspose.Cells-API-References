---
title: "Класс GridWorksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridWeb.Data.GridWorksheet class. Инкапсулирует объект, представляющий отдельный лист"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

Инкапсулирует объект, представляющий отдельный лист.

```csharp
public class GridWorksheet : Control, ISerializable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | Получает или задает активную ячейку в рабочем листе. |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | Получает и задает фоновое изображение рабочего листа. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | Привяжите коллекцию столбцов. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | Фактический объект источника данных, привязываемый во время выполнения. Это объект DataView, когда свойство DataSource является объектом DataSet, DataTable или DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | Получает коллекцию [`GridCell`](../gridcell/). |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | Представляет кодовое имя листа. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | Получает коллекцию [`GridComment`](../gridcomment/). |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | Получает количество привязанных строк в режиме привязки данных. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | Получает или задает DataMember из многокомпонентного DataSource. Обычно он представляет объект DataTable из DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | Получает или задает DataSource. Обычно это объект DataSet. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию false. |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | True, если отображаются нулевые значения. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | В режиме привязки данных указывает, следует ли создавать подписи заголовков привязанных столбцов на листе. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | Представляет индекс первой видимой колонки. |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | Представляет индекс первой видимой строки. |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | Получает или задает активную ячейку в рабочем листе. |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | Получает коллекцию [`GridHyperlinkCollection`](../gridhyperlinkcollection/). |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | Получает индекс листа в коллекции листов. |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | Получает или задает значение, указывающее, видимы ли линии сетки. По умолчанию true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | Указывает, будет ли строка итогов размещена ниже строк деталей в outline. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | Получает или задаёт имя листа. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | Указывает, показывать ли контур. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | Получает коллекцию [`Pictures`](./pictures/). |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | Получает pivotTables в листе. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | Указывает, выбран ли этот лист при открытии книги. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | Получает коллекцию [`Pictures`](./pictures/). |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | Возвращает или задает высоту строки по умолчанию в этом листе, в единицах точек. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | Возвращает или задает высоту строки по умолчанию в этом листе, в единицах пикселей. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | Представляет цвет вкладки листа. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | Получает коллекцию настроек проверки данных в листе. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | Указывает, отображается ли имя этого листа во вкладках листов управления. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | Получает объект [`GridWorkbook`](../gridworkbook/) из коллекции листов. |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | Представляет коэффициент масштабирования в процентах. Должен быть в диапазоне от 10 до 400. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | Устанавливает диапазон, к которому применяется указанный AutoFilter. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | Добавить пользовательский фильтр для указанной строки. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn)(int) | Автоматически подгоняет ширину столбца. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Автоматически подгоняет ширину столбца. |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() |  |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow)(int) | Автоматически подгоняет высоту строки. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_1)(int, int, int) | Автоматически подгоняет высоту строки. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_2)(int, int, int, int) | Автоматически подгоняет высоту строки в прямоугольном диапазоне. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows)() | Автоматически подгоняет все строки в этом листе. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_1)(bool) | Автоматически подгоняет все строки в этом листе. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_2)(int, int) | Автоматически подгоняет высоту строки в диапазоне. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | Вычисляет формулу. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | Отменяет и удаляет только что добавленную привязанную строку. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | Очищает все комментарии в проектируемой таблице. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | Подтверждает только что добавленную привязанную строку и добавляет её в datasource. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | Копирует содержимое и форматы из другого листа. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | После установки datasource для листа вызовите этот метод для автоматического создания привязанных столбцов. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | Создаёт новую привязанную строку и привязывает её к datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Создаёт промежуточный итог на листе. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Создаёт промежуточный итог на листе. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | Привяжите лист к DataSource. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | Привяжите лист к DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | Удаляет привязанную строку. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | Устанавливает фильтр для столбца. Обратите внимание, что перед вызовом filterString необходимо вызвать AddAutoFilter. Строка критериев фильтра. Обратите внимание, что в качестве разделителя используется запятая-&gt;"," , поэтому значение ячейки, которое вы хотите отфильтровать, не должно содержать запятую. filterString(10,"123,456") означает, что столбец 10 должен содержать 123 или 456, filterString(10,"123") означает, что столбец 10 должен содержать 123. Индекс столбца разделяется запятой, например 123,456,789 или abc. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes_1)(string, int, int) | Замораживает области в указанной ячейке листа. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes)(int, int, int, int) | Замораживает области в указанной ячейке листа. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | Получает подпись столбца. Если подпись не задана, возвращает пустую строку. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | Получает текст всплывающей подсказки заголовка столбца. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | Получает, является ли столбец только для чтения. Это расширенный метод GridWeb, который не сохраняется и не влияет на реальный файл Excel. |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | Получает замороженные области. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | Получает, является ли ячейка только для чтения. Это расширенный атрибут GridWeb, который не сохраняется в реальном файле Excel. |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | Получает подпись строки. Если подпись не установлена, возвращает пустую строку. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | Получает текст всплывающей подсказки заголовка строки. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | Получает, является ли строка только для чтения. Это расширенный метод GridWeb, он не сохраняется и не влияет на реальный файл Excel. |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | Группирует строки. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | Указывает, защищён ли лист. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | Перемещает лист в другое место в таблице. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | Обновить автофильтры, чтобы скрыть или показать строки. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | Удалить автофильтр листа. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | Удаляет подытог, созданный методом CreateSubtotal на листе. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | Целочисленное смещение поля, к которому вы хотите применить, основанное на первом столбце фильтра (слева в списке; самый левый столбец имеет индекс 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | Делает все ячейки редактируемыми. Это расширенный атрибут. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | Делает все ячейки только для чтения. Это расширенный атрибут; обратите внимание, что этот атрибут не сохраняется в реальной ячейке, если нужно сохранить защиту, используйте setProtect. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | Устанавливает подпись для столбца. Обратите внимание, что это расширенный атрибут и не сохраняется в файле Excel. |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | Устанавливает текст всплывающей подсказки заголовка столбца. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | Устанавливает столбец только для чтения, чтобы пользователь не мог удалить его на клиенте. Это расширенный метод GridWeb, он не сохраняется и не влияет на реальный файл Excel. |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | Делает диапазон ячеек редактируемым. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сделайте все ячейки только для чтения, вызвав метод SetAllCellsReadonly. Затем вызовите этот метод, чтобы указать диапазон ячеек, который будет редактируемым. |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | Устанавливает, является ли ячейка только для чтения. Это расширенный атрибут GridWeb, он не сохраняется в реальном файле Excel. |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | Защищает лист. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | Делает диапазон ячеек только для чтения. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сначала сделайте все ячейки редактируемыми, вызвав метод SetAllCellsEditable. Затем вызовите этот метод, чтобы указать диапазон ячеек, который будет только для чтения. |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | Устанавливает подпись для строки. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | Устанавливает текст всплывающей подсказки заголовка строки. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | Устанавливает строку только для чтения, чтобы пользователь не мог удалить её на клиенте. Это расширенный метод GridWeb, он не сохраняется и не влияет на реальный файл Excel. |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | Размораживает области в листе. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | Разгруппирует строки. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | Снимает защиту с листа. |

## События

| Имя | Описание |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | Событие происходит, когда лист создает новую связанную строку и требуется её инициализировать. |

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


