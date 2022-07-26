---
title: GridDesktop
second_title: Справочник по Aspose.Cells для .NET API
description: Aspose GridDesktop class Представляет корневой объект для создания элемента управления GridDesktop. Чтобы использовать этот элемент управления просто перетащите его из панели инструментов в форму или пользовательский элемент управления.
type: docs
weight: 840
url: /ru/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Aspose GridDesktop class Представляет корневой объект для создания элемента управления GridDesktop. Чтобы использовать этот элемент управления, просто перетащите его из панели инструментов в форму или пользовательский элемент управления.

```csharp
public class GridDesktop : UserControl
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridDesktop](griddesktop)() | Класс Aspose GridDesktop |

## Характеристики

| Имя | Описание |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex) { get; set; } | Получает или задает индекс выбранного листа. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont) { get; set; } | Получает или задает активный лист, отображающий шрифт панели листа. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas) { get; set; } | Получает или задает значение, указывающее, нужно ли нам запускать все формулы, например, когда мы запускаем все формулы, при обновлении значения одной ячейки, и это влияет на другие, а другие влияют на другие, все больше и больше, вызывают необходимость пересчета всех ячеек , как и эффект бабочки, требуется много операций со стеком, он получит очень низкую производительность, как и в CELLSNET-41921, этот выпуск содержит тот самый файл, который может показать этот сценарий нам лучше просто запустить все формулы, , так как при запуске всех формул у нас может быть некоторая оптимизация. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle) { get; set; } | Указывает стиль границы элемента управления. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible) { get; set; } | Получает или задает значение, указывающее, виден ли заголовок столбца. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont) { get; set; } | Получает или задает отображаемый по умолчанию шрифт текста комментария. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager) { get; } | Получает экземпляр ContextMenuManager. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont) { get; set; } | Получает или задает шрифт по умолчанию для ячейки |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor) { get; set; } | Получает или задает цвет шрифта по умолчанию для ячейки. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste) { get; set; } | Указывает, следует ли копировать/вставлять на основе буфера обмена, чтобы можно было копировать/вставлять с помощью MS-EXCEL. Копируется/вставляется только значение ячейки, не копируются никакие другие настройки ячейки, такие как формат, стиль границы и т. д. Значение по умолчанию — false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension) { get; set; } | Получает или задает значение, указывающее, будет ли операция копирования увеличивать количество строк или столбцов. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption) { get; set; } | Получает или задает значение, указывающее, будет ли операция копирования копировать значение атрибута CellLocked стиля ячейки. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo) { get; set; } | Получает или задает значение, указывающее, включена ли функция отмены. Значение по умолчанию — false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting) { get; set; } | Получает или устанавливает параметр памяти. |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible) { get; set; } | Устанавливает видимую статую для горизонтальной полосы прокрутки. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible) { get; set; } | Устанавливает видимую статую для вертикальной полосы прокрутки. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names) { get; } | Получает коллекцию всех объектов Name в электронной таблице. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows) { get; set; } | Задает или получает размер строки для разбивки на страницы. Максимальное количество поддерживаемых PageRows – 100 000, максимальное количество поддерживаемых страниц – 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype) { get; set; } | Указывает, какой тип вставки при выполнении действия вставки，доступно, только если EnableClipboardCopyPaste имеет значение false . |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1) { get; set; } | Получает или задает значение, указывающее, использует ли элемент управления стиль ссылки R1C1. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas) { get; set; } | Получает или задает значение, указывающее, следует ли пересчитывать формулу всех ячеек при изменении значения ячейки. Значение по умолчанию — true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible) { get; set; } | Получает или задает значение, указывающее, виден ли заголовок строки. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont) { get; set; } | Получает или задает отображаемый по умолчанию шрифт панели листа. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible) { get; set; } | Получает или задает значение, указывающее, видима ли полоса листа. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth) { get; set; } | Устанавливает/получает ширину вкладки листа. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu) { get; set; } | Получает или задает значение, указывающее, может ли элемент управления отображать контекстное меню. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus) { get; set; } | Получает или задает значение, указывающее, следует ли отображать вычисление status Значение по умолчанию — true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager) { get; } | Получает экземпляр UndoManager. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets) { get; } | Получает рабочие листы. |

## Методы

| Имя | Описание |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear)() | Очищает элемент управления GridDesktop. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy)() | Копирует содержимое ячейки в буфер обмена. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut)() | Вырезает содержимое ячейки в буфер обмена. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit)() | Устанавливает разделенный вид. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter)() | Уведомляет GridDesktop о завершении FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile)(Stream) | Экспорт в файловый поток Excel, включая поток дискового ввода-вывода или поток памяти. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_2)(string) | Экспорт в файл Excel. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_1)(Stream, FileFormatType) | Экспорт в файловый поток Excel, включая поток дискового ввода-вывода или поток памяти. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_3)(string, FileFormatType) | Экспорт в файл Excel. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet)() | Получает текущий активный рабочий лист. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar)() | вернуть горизонтальную полосу прокрутки |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar)() | вернуть вертикальную полосу прокрутки |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile)(Stream) | Импорт из потока файлов Excel, включая поток файлов на диске или поток памяти. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_3)(string) | Импорт из файла Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_1)(Stream, bool) | Импорт из потока файлов Excel, включая поток файлов на диске или поток памяти. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_4)(string, bool) | Импорт из файла Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_5)(string, int) | Импорт рабочего листа из файла Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_2)(Stream, string, string, bool, bool) | Импорт из файла Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_6)(string, string, string, bool, bool) | Импорт из файла Excel. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog)(bool) | Открывает диалоговое окно FindReplace для поиска или замены ячеек. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste)() | Вставляет содержимое буфера обмена в выбранную ячейку. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol)() | Обновить элемент управления GridDesktop. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas)() | Запускает формулу всех ячеек. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible)() | Делает все полосы прокрутки видимыми. |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog)() | Открывает диалоговое окно стиля для установки стиля ячеек, шрифта, цветов и т. д. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter)(bool) | Уведомляет GridDesktop о запуске FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit)() | Отключить разделенный вид. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion)() | Получить релизную версию. |

## Поля

| Имя | Описание |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter) | параметры фильтрации данных при загрузке книги из шаблона. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage) | нужно ли показывать окно сообщения, когда не удается импортировать файл, значение по умолчанию — true |

## События

| Имя | Описание |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns) | Происходит после удаления столбца. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows) | Происходит после удаления строки. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns) | Происходит после вставки нового столбца. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows) | Происходит после вставки новой строки. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate) | Происходит перед вычислением формулы в книге. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile) | Происходит перед загрузкой книги из файла. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick) | Происходит при нажатии кнопки ячейки. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged) | Происходит при изменении свойства флажка ячейки Checked. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick) | Происходит при нажатии ячейки сетки. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy) | Происходит при копировании ComboBox ячейки сетки. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged) | Происходит при изменении свойства данных ячейки сетки. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick) | Происходит при двойном щелчке ячейки сетки. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged) | Происходит при изменении формата ячейки в диалоговом окне «Формат ячеек». |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed) | Происходит при нажатии клавиши, когда фокус находится на ячейке. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged) | Происходит при изменении свойства SelectedIndex поля со списком ячеек. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging) | Возникает при вводе символов в ячейку сетки. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed) | Происходит, когда проверка ячейки сетки не удалась. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick) | Происходит при щелчке заголовка столбца. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick) | Происходит при двойном щелчке заголовка столбца. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged) | Происходит при изменении данных комментария. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate) | Происходит после расчета формулы в книге. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile) | Происходит при загрузке книги. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged) | Происходит при изменении ячейки в фокусе. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged) | Происходит при изменении состояния скрытия строки/столбца. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent) | Происходит после выбора элемента фильтра строки. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick) | Происходит при щелчке заголовка строки. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick) | Происходит при двойном щелчке заголовка строки. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged) | Происходит при изменении выбранного диапазона ячеек. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged) | Происходит при изменении свойства SelectedSheetIndex. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick) | Происходит при нажатии на фигуру. |

### Примечания

Дополнительные сведения о System.Windows.Forms.UserControl. см. в документе .NET SDK.

### Примеры

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### Смотрите также

* пространство имен [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
