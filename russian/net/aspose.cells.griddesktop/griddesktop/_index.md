---
title: "Класс GridDesktop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridDesktop.GridDesktop. Класс Aspose GridDesktop представляет корневой объект для создания элемента управления GridDesktop. Чтобы использовать этот элемент управления, просто перетащите его из панели инструментов на форму или пользовательский элемент управления."
type: docs
url: /ru/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Класс Aspose GridDesktop представляет корневой объект для создания элемента управления GridDesktop. Чтобы использовать этот элемент управления, просто перетащите его из панели инструментов на форму или пользовательский элемент управления.

```csharp
public class GridDesktop : UserControl
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridDesktop](griddesktop/)() | Класс Aspose GridDesktop |

## Свойства

| Имя | Описание |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | Получает или задает индекс выбранного листа. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | Получает или задает шрифт отображения активного листа в строке листов. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | Получает или задает значение, указывающее, нужно ли выполнять все формулы, так как при выполнении всех формул при обновлении значения одной ячейки оно влияет на другие, а те влияют на другие, и так далее, вызывая необходимость пересчёта всех ячеек, подобно эффекту бабочки; это требует множества стековых операций, что приводит к очень низкой производительности, как в CELLSNET-41921; эта проблема содержит файл, демонстрирующий данный сценарий. Лучше просто выполнять все формулы, так как при их выполнении мы можем применить некоторую оптимизацию. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | Указывает стиль границы для элемента управления. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | Получает или задает значение, указывающее, видим ли заголовок столбца. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | Получает или задает шрифт отображения текста комментария по умолчанию. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | Получает экземпляр ContextMenuManager. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | Получает или задает шрифт ячейки по умолчанию. |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | Получает или задает цвет шрифта ячейки по умолчанию. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | Указывает, следует ли копировать/вставлять на основе буфера обмена, чтобы обеспечить совместимость с MS-EXCEL. Копируются/вставляются только значения ячеек, другие настройки ячеек, такие как формат, стиль границы и т.д., не копируются. Значение по умолчанию — false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | Получает или задает значение, указывающее, будет ли операция копирования расширять количество строк или столбцов. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | Получает или задает значение, указывающее, будет ли операция копирования копировать значение атрибута CellLocked стиля ячейки. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | Получает или задает значение, указывающее, включена ли функция отмены. Значение по умолчанию — false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | Получает или задает параметр памяти, значение по умолчанию — GridMemorySetting.Normal |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | Устанавливает видимость для горизонтальной полосы прокрутки. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | Устанавливает видимость для вертикальной полосы прокрутки. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | Получает коллекцию всех объектов Name в таблице. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | Устанавливает или получает размер строки для пагинации. Максимальное поддерживаемое значение PageRows — 100000, максимальное количество страниц — 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | Указывает тип вставки при выполнении действия вставки, доступно только когда EnableClipboardCopyPaste равно false. Значение по умолчанию — GridPasteType.Default; |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | Получает или задает значение, указывающее, использует ли элемент управления стиль ссылок R1C1. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | Получает или задает значение, указывающее, следует ли пересчитывать формулы всех ячеек при изменении значения ячейки. Значение по умолчанию — true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | Получает или задает значение, указывающее, видим ли заголовок строки. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | Получает или задает шрифт отображения по умолчанию для панели листов. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | Получает или задает значение, указывающее, видима ли панель листов. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | Устанавливает/получает ширину вкладки листа. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | Получает или задает значение, указывающее, может ли элемент управления показывать контекстное меню. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | Устанавливает/получает, показывать ли сообщение об ошибке или предупреждении при установке значения формулы ячейки, значение по умолчанию — true. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | Устанавливает/получает, показывать ли треугольный символ для ячейки, содержащей числовую строку, но сохранённой в текстовом формате |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | Получает или задает значение, указывающее, показывать ли статус вычисления. Значение по умолчанию — true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | Получает экземпляр UndoManager. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | Получает листы Worksheets. |

## Методы

| Имя | Описание |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | Очищает элемент управления GridDesktop. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | Копирует содержимое выбранной ячейки в буфер обмена. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | Вырезает содержимое выбранной ячейки в буфер обмена. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | Устанавливает разделённый вид. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | Уведомляет GridDesktop о завершении FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | Экспортирует в поток Excel‑файла, включая поток ввода‑вывода диска или поток памяти. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | Экспортирует в Excel‑файл. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | Экспортирует в поток Excel‑файла, включая поток ввода‑вывода диска или поток памяти. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | Экспортирует в файл Excel. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | Экспортирует в поток PDF‑файла, включая поток ввода‑вывода диска или поток памяти. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | Экспортирует в поток PDF‑файла, включая поток ввода‑вывода диска или поток памяти. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | Получает текущий активный лист. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | возвращает горизонтальную полосу прокрутки |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | возвращает вертикальную полосу прокрутки |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | Импортирует из потока Excel‑файла, включая поток с диска или поток памяти. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | Импортирует из Excel‑файла. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | Импортирует из потока Excel‑файла, включая поток с диска или поток памяти. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | Импортирует из Excel‑файла. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | Импортирует лист из файла Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | Импортирует из Excel‑файла. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | Импортирует из Excel‑файла. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | Переопределить инвалидизацию. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | Открывает диалоговое окно FindReplace для поиска или замены ячеек. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | Вставляет содержимое буфера обмена в выбранную ячейку. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | Обновить элемент управления GridDesktop. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | Выполняет формулы всех ячеек. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | Устанавливает видимость всех полос прокрутки. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | Установить пользовательский менеджер ресурсов для реализации пользовательской локализации |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | Открывает диалог стилей, чтобы установить стиль ячеек, шрифт, цвета и т.д. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | Уведомляет GridDesktop о запуске FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | Отключить разделённый вид. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | Получить версию выпуска. |

## Поля

| Имя | Описание |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | опции для фильтрации данных при загрузке книги из шаблона. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | показывать ли сообщение при ошибке импорта файла, значение по умолчанию — true |

## События

| Имя | Описание |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | Событие происходит после удаления столбца. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | Событие происходит после удаления строки. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | Событие происходит после вставки нового столбца. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | Событие происходит после вставки новой строки. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | Событие происходит перед вычислением формулы в книге. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | Событие происходит перед загрузкой книги из файла. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | Событие происходит при нажатии кнопки ячейки. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | Событие происходит при изменении свойства Checked у флажка ячейки. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | Происходит, когда щелкают по gridcell. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | Происходит, когда ComboBox ячейки сетки копируется. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | Происходит, когда свойство данных ячейки сетки изменяется. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | Происходит, когда gridcell дважды щелкают. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | Происходит, когда формат ячейки изменяется через диалоговое окно Формат ячеек. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | Происходит, когда нажата клавиша, пока ячейка в фокусе. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | Происходит, когда свойство SelectedIndex комбобокса ячейки изменилось. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | Происходит, когда вводятся символы в ячейку сетки. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | Происходит, когда проверка ячейки сетки не удалась. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | Происходит, когда щелкают по заголовку столбца. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | Происходит, когда заголовок столбца дважды щелкают. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | Происходит, когда данные комментария изменились. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | Происходит после вычисления формулы в рабочей книге. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | Происходит, когда рабочая книга загружена. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | Происходит, когда меняется сфокусированная ячейка. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | Происходит, когда щелкают по фигуре. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | Происходит, когда статус скрытия строки/столбца изменяется. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | Происходит после выбора элемента фильтра строки. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | Происходит, когда щелкают по заголовку строки. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | Происходит, когда заголовок строки дважды щелкают. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | Происходит, когда выбранный диапазон ячеек изменяется. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | Происходит, когда свойство SelectedSheetIndex изменяется. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | Происходит, когда щелкают по фигуре. |

### Примечания

Пожалуйста, обратитесь к документу .NET SDK для получения дополнительной информации о System.Windows.Forms.UserControl.

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

### См. также

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


