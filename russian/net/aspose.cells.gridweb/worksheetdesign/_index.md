---
title: "Класс WorksheetDesign"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.WorksheetDesign. Наследуется от WebWorksheet. Используется только во время разработки"
type: docs
url: /ru/net/aspose.cells.gridweb/worksheetdesign/
---
## WorksheetDesign class

Наследуется от WebWorksheet. Используется только во время разработки.

```csharp
public class WorksheetDesign : WebWorksheet
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WorksheetDesign](worksheetdesign/#constructor)() | Конструктор по умолчанию. |
| [WorksheetDesign](worksheetdesign/#constructor_1)(MainWeb, GridWorksheet) | конструктор с параметрами MainWeb и GridWorksheet |

## Свойства

| Имя | Описание |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Коллекция привязанных столбцов.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | Фактический объект источника данных, привязываемый во время выполнения. Это объект DataView, когда свойство DataSource является объектом DataSet, DataTable или DataView.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } | (Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Получает [`WebCells`](../../aspose.cells.gridweb.data/webcells/).(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } | (Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Получает количество привязанных строк в режиме привязки данных.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Получает или задает DataMember из многокомпонентного DataSource. Обычно он представляет объект DataTable из DataSet.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Получает или задает DataSource. Обычно это объект DataSet.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | В режиме привязки данных указывает, следует ли создавать подписи заголовков привязанных столбцов в листе.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Получает коллекцию HyperlinkCollection.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Получает индекс самого себя среди листов.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Получает или задает, защищён ли лист. Когда лист защищён, все ячейки нельзя редактировать, кроме ячейки, у которой свойство IsLocked равно false.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Получает или задает имя листа.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } | (Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Получает коллекцию настроек проверки данных в листе.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Указывает, отображается ли имя этого листа на вкладках листов управления.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int) | Автоподгонка ширины столбца.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int, int, int) | Автоподгонка ширины столбца. Этот метод автоматически подгоняет столбец на основе содержимого в диапазоне ячеек внутри столбца от startRow до endRow. AutoFitColumn — неточная функция.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Отменяет и удаляет только что добавленную связанную строку.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Подтверждает только что добавленную связанную строку и добавляет её в источник данных.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Копирует из другого объекта листа.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | После установки источника данных для листа вызовите этот метод для автоматического создания связанных столбцов.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Создаёт новую связанную строку и привязывает её к источнику данных.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Создаёт промежуточный итог на листе.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Привязывает лист к источнику данных.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Удаляет связанную строку.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Замораживает области на указанной ячейке листа.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int) | Группирует строки.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int, bool) | Группирует строки.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Делает все ячейки редактируемыми. Это расширенный атрибут(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Делает все ячейки только для чтения. Это расширенный атрибут, обратите внимание, что этот атрибут не сохраняется в реальной ячейке; если вы хотите сохранить защиту, пожалуйста, используйте setProtect(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Делает диапазон ячеек редактируемым. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Делает все ячейки только для чтения, вызывая метод SetAllCellsReadonly. Затем вызовите этот метод, чтобы указать диапазон ячеек, которые должны быть редактируемыми(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Делает диапазон ячеек только для чтения. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сначала сделайте все ячейки редактируемыми, вызвав метод SetAllCellsEditable. Затем вызовите этот метод, чтобы указать диапазон ячеек, которые должны быть только для чтения(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Размораживает области на листе.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Разгруппирует строки.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Обновляет значение свойства записи привязанного источника данных в соответствии со значением ячейки.(Унаследовано от [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

### См. также

* class [WebWorksheet](../../aspose.cells.gridweb.data/webworksheet/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


