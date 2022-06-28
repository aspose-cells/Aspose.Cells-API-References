---
title: Worksheet
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий один рабочий лист.
type: docs
weight: 6510
url: /ru/net/aspose.cells/worksheet/
---
## Worksheet class

Инкапсулирует объект, представляющий один рабочий лист.

```csharp
public class Worksheet : IDisposable
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [ActiveCell](../../aspose.cells/worksheet/activecell) { get; set; } | Получает или задает активную ячейку на листе. |
| [AllowEditRanges](../../aspose.cells/worksheet/alloweditranges) { get; } | Получает коллекцию разрешенных диапазонов редактирования на листе. |
| [AutoFilter](../../aspose.cells/worksheet/autofilter) { get; } | Представляет автоматический фильтр для указанного рабочего листа. |
| [BackgroundImage](../../aspose.cells/worksheet/backgroundimage) { get; set; } | Получает и устанавливает фоновое изображение листа. |
| [Cells](../../aspose.cells/worksheet/cells) { get; } | Получает коллекцию[`Cells`](./cells). |
| [CellWatches](../../aspose.cells/worksheet/cellwatches) { get; } | Получает набор ячеек на этом рабочем листе, наблюдаемых в «окне просмотра». |
| [Charts](../../aspose.cells/worksheet/charts) { get; } | Получает[`Chart`](../../aspose.cells.charts/chart)коллекцию |
| [CheckBoxes](../../aspose.cells/worksheet/checkboxes) { get; } | Получает коллекцию[`CheckBox`](../../aspose.cells.drawing/checkbox). |
| [CodeName](../../aspose.cells/worksheet/codename) { get; set; } | Получает кодовое имя листа. |
| [Comments](../../aspose.cells/worksheet/comments) { get; } | Получает коллекцию[`Comment`](../comment). |
| [ConditionalFormattings](../../aspose.cells/worksheet/conditionalformattings) { get; } | Получает условное форматирование на листе. |
| [CustomProperties](../../aspose.cells/worksheet/customproperties) { get; } | Получает объект, представляющий информацию идентификатора, связанную с рабочим листом. |
| [DisplayRightToLeft](../../aspose.cells/worksheet/displayrighttoleft) { get; set; } | Указывает, отображается ли указанный рабочий лист справа налево, а не слева направо. По умолчанию false. |
| [DisplayZeros](../../aspose.cells/worksheet/displayzeros) { get; set; } | Истинно, если отображаются нулевые значения. |
| [ErrorCheckOptions](../../aspose.cells/worksheet/errorcheckoptions) { get; } | Получает настройку проверки ошибок, применяемую к определенным диапазонам. |
| [FirstVisibleColumn](../../aspose.cells/worksheet/firstvisiblecolumn) { get; set; } | Представляет индекс первого видимого столбца. |
| [FirstVisibleRow](../../aspose.cells/worksheet/firstvisiblerow) { get; set; } | Представляет индекс первой видимой строки. |
| [HasAutofilter](../../aspose.cells/worksheet/hasautofilter) { get; } | Указывает, есть ли на этом листе автоматический фильтр. |
| [HorizontalPageBreaks](../../aspose.cells/worksheet/horizontalpagebreaks) { get; } | Получает коллекцию[`HorizontalPageBreakCollection`](../horizontalpagebreakcollection). |
| [Hyperlinks](../../aspose.cells/worksheet/hyperlinks) { get; } | Получает коллекцию[`HyperlinkCollection`](../hyperlinkcollection). |
| [Index](../../aspose.cells/worksheet/index) { get; } | Получает индекс листа в коллекции рабочих листов. |
| [IsGridlinesVisible](../../aspose.cells/worksheet/isgridlinesvisible) { get; set; } | Получает или задает значение, указывающее, видны ли линии сетки. Значение по умолчанию — true. |
| [IsOutlineShown](../../aspose.cells/worksheet/isoutlineshown) { get; set; } | Указывает, показывать ли контур. |
| [IsPageBreakPreview](../../aspose.cells/worksheet/ispagebreakpreview) { get; set; } | Указывает, отображается ли указанный лист в обычном режиме или в предварительном просмотре с разрывом страницы. |
| [IsProtected](../../aspose.cells/worksheet/isprotected) { get; } | Указывает, защищен ли рабочий лист. |
| [IsRowColumnHeadersVisible](../../aspose.cells/worksheet/isrowcolumnheadersvisible) { get; set; } | Получает или задает значение, указывающее, будут ли на листе отображаться заголовки строк и столбцов. Значение по умолчанию — true. |
| [IsRulerVisible](../../aspose.cells/worksheet/isrulervisible) { get; set; } | Указывает, видна ли линейка. Это свойство применяется только для предварительного просмотра разрыва страницы. |
| [IsSelected](../../aspose.cells/worksheet/isselected) { get; set; } | Указывает, выбран ли этот лист при открытии книги. |
| [IsVisible](../../aspose.cells/worksheet/isvisible) { get; set; } | Указывает, виден ли рабочий лист. |
| [ListObjects](../../aspose.cells/worksheet/listobjects) { get; } | Получает все объекты ListObject на этом листе. |
| [Name](../../aspose.cells/worksheet/name) { get; set; } | Получает или задает имя рабочего листа. |
| [OleObjects](../../aspose.cells/worksheet/oleobjects) { get; } | Представляет коллекцию[`OleObject`](../../aspose.cells.drawing/oleobject)на рабочем листе. |
| [Outline](../../aspose.cells/worksheet/outline) { get; } | Получает схему на этом листе. |
| [PageSetup](../../aspose.cells/worksheet/pagesetup) { get; } | Представляет описание настройки страницы на этом листе. |
| [PaneState](../../aspose.cells/worksheet/panestate) { get; } | Указывает, есть ли у панели горизонтальные или вертикальные разделения и зафиксированы ли эти разделения. |
| [Pictures](../../aspose.cells/worksheet/pictures) { get; } | Получает коллекцию[`Picture`](../../aspose.cells.drawing/picture). |
| [PivotTables](../../aspose.cells/worksheet/pivottables) { get; } | Получает все сводные таблицы на этом листе. |
| [Protection](../../aspose.cells/worksheet/protection) { get; } | Представляет различные типы опций защиты, доступные для рабочего листа. Поддерживает расширенные параметры защиты в ExcelXP и более поздних версиях. |
| [QueryTables](../../aspose.cells/worksheet/querytables) { get; } | Получает[`QueryTableCollection`](../querytablecollection)на листе. |
| [Scenarios](../../aspose.cells/worksheet/scenarios) { get; } | Получает коллекцию[`Scenario`](../scenario). |
| [Shapes](../../aspose.cells/worksheet/shapes) { get; } | Возвращает все фигуры на этом рабочем листе. |
| [ShowFormulas](../../aspose.cells/worksheet/showformulas) { get; set; } | Указывает, показывать ли формулы или их результаты. |
| [Slicers](../../aspose.cells/worksheet/slicers) { get; } | Получить коллекцию Slicer на листе |
| [SmartTagSetting](../../aspose.cells/worksheet/smarttagsetting) { get; } | Получает все объекты[`SmartTagCollection`](../../aspose.cells.markup/smarttagcollection)рабочего листа. |
| [SparklineGroupCollection](../../aspose.cells/worksheet/sparklinegroupcollection) { get; } | Получает коллекцию групп спарклайнов на листе. |
| [TabColor](../../aspose.cells/worksheet/tabcolor) { get; set; } | Представляет цвет вкладки рабочего листа. |
| [TabId](../../aspose.cells/worksheet/tabid) { get; set; } | Задает внутренний идентификатор листа. |
| [TextBoxes](../../aspose.cells/worksheet/textboxes) { get; } | Получает коллекцию[`TextBox`](../../aspose.cells.drawing/textbox). |
| [Timelines](../../aspose.cells/worksheet/timelines) { get; } | Получить коллекцию Timeline на листе |
| [TransitionEntry](../../aspose.cells/worksheet/transitionentry) { get; set; } | Указывает, включена ли опция Ввод формулы перехода (совместимость с Lotus). |
| [TransitionEvaluation](../../aspose.cells/worksheet/transitionevaluation) { get; set; } | Указывает, включена ли опция оценки формулы перехода (совместимость с Lotus). |
| [Type](../../aspose.cells/worksheet/type) { get; set; } | Представляет тип листа. |
| [UniqueId](../../aspose.cells/worksheet/uniqueid) { get; set; } | Получает и устанавливает уникальный идентификатор, он аналогичен {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [Validations](../../aspose.cells/worksheet/validations) { get; } | Получает набор параметров проверки данных на листе. |
| [VerticalPageBreaks](../../aspose.cells/worksheet/verticalpagebreaks) { get; } | Получает коллекцию[`VerticalPageBreakCollection`](../verticalpagebreakcollection). |
| [ViewType](../../aspose.cells/worksheet/viewtype) { get; set; } | Получает и задает тип представления. |
| [VisibilityType](../../aspose.cells/worksheet/visibilitytype) { get; set; } | Указывает видимое состояние для этого листа. |
| [Workbook](../../aspose.cells/worksheet/workbook) { get; } | Получает объект книги, содержащий этот лист. |
| [Zoom](../../aspose.cells/worksheet/zoom) { get; set; } | Представляет коэффициент масштабирования в процентах. Должно быть от 10 до 400. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddPageBreaks](../../aspose.cells/worksheet/addpagebreaks)(string) | Добавляет разрыв страницы. |
| [AdvancedFilter](../../aspose.cells/worksheet/advancedfilter)(bool, string, string, string, bool) | Фильтрует данные по сложным критериям. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn#autofitcolumn)(int) | Автоподбор ширины столбца. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn#autofitcolumn_1)(int, int, int) | Автоподбор ширины столбца. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns)() | Автоподбор всех столбцов на этом листе. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_1)(AutoFitterOptions) | Автоподбор всех столбцов на этом листе. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_2)(int, int) | Автоподбор ширины столбцов. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_3)(int, int, AutoFitterOptions) | Автоподбор ширины столбцов. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_4)(int, int, int, int) | Автоподбор ширины столбцов. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_5)(int, int, int, int, AutoFitterOptions) | Автоподбор ширины столбцов. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow)(int) | Автоподбор высоты строки. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_1)(int, int, int) | Автоподбор высоты строки. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_2)(int, int, int, AutoFitterOptions) | Автоподбор высоты строки. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_3)(int, int, int, int) | Автоподбор высоты строки в прямоугольном диапазоне. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows)() | Автоподбор всех строк на этом листе. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_1)(AutoFitterOptions) | Автоподбор всех строк на этом листе. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_2)(bool) | Автоподбор всех строк на этом листе. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_3)(int, int) | Автоподбор высоты строки в диапазоне. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_4)(int, int, AutoFitterOptions) | Автоподбор высоты строки в диапазоне. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula)(string) | Вычисляет формулу. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula_2)(CalculationOptions, bool) | Вычисляет все формулы на этом листе. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula_1)(string, CalculationOptions) | Вычисляет формулу. |
| [ClearComments](../../aspose.cells/worksheet/clearcomments)() | Удаляет все комментарии в электронной таблице конструктора. |
| [CloseAccessCache](../../aspose.cells/worksheet/closeaccesscache)(AccessCacheOptions) | Закрывает сеанс, использующий кэши для доступа к данным на этом листе. |
| [Copy](../../aspose.cells/worksheet/copy#copy)(Worksheet) | Копирует содержимое и форматы с другого рабочего листа. |
| [Copy](../../aspose.cells/worksheet/copy#copy_1)(Worksheet, CopyOptions) | Копирует содержимое и форматы с другого рабочего листа. |
| [Dispose](../../aspose.cells/worksheet/dispose)() | Выполняет определяемые приложением задачи, связанные с освобождением, освобождением или сбросом неуправляемых ресурсов. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes#freezepanes_1)(string, int, int) | Замораживает панели в указанной ячейке рабочего листа. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes#freezepanes)(int, int, int, int) | Замораживает панели в указанной ячейке рабочего листа. |
| [GetFreezedPanes](../../aspose.cells/worksheet/getfreezedpanes)(out int, out int, out int, out int) | Получает области стоп-кадра. |
| [GetPanes](../../aspose.cells/worksheet/getpanes)() | Получает оконные панели. |
| [GetPrintingPageBreaks](../../aspose.cells/worksheet/getprintingpagebreaks)(ImageOrPrintOptions) | Получает автоматические разрывы страниц. |
| [GetSelectedRanges](../../aspose.cells/worksheet/getselectedranges)() | Получает выбранные диапазоны ячеек в электронной таблице конструктора. |
| [MoveTo](../../aspose.cells/worksheet/moveto)(int) | Перемещает лист в другое место электронной таблицы. |
| [Protect](../../aspose.cells/worksheet/protect#protect)(ProtectionType) | Защищает рабочий лист. |
| [Protect](../../aspose.cells/worksheet/protect#protect_1)(ProtectionType, string, string) | Защищает рабочий лист. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables)() | Обновляет все сводные таблицы на этом рабочем листе. |
| [RemoveAllDrawingObjects](../../aspose.cells/worksheet/removealldrawingobjects)() | Удаляет все объекты чертежа на этом рабочем листе. |
| [RemoveAutoFilter](../../aspose.cells/worksheet/removeautofilter)() | Удаляет автоматический фильтр рабочего листа. |
| [RemoveSplit](../../aspose.cells/worksheet/removesplit)() | Удаляет разделенное окно. |
| [Replace](../../aspose.cells/worksheet/replace)(string, string) | Заменяет текст во всех ячейках новой строкой. |
| [SelectRange](../../aspose.cells/worksheet/selectrange)(int, int, int, int, bool) | Выбирает диапазон. |
| [SetVisible](../../aspose.cells/worksheet/setvisible)(bool, bool) | Устанавливает видимые параметры. |
| [Split](../../aspose.cells/worksheet/split)() | Разделяет окно. |
| [StartAccessCache](../../aspose.cells/worksheet/startaccesscache)(AccessCacheOptions) | Запускает сеанс, который использует кэши для доступа к данным на этом листе. |
| override [ToString](../../aspose.cells/worksheet/tostring)() | Возвращает строку, представляющую текущий объект Worksheet. |
| [UnFreezePanes](../../aspose.cells/worksheet/unfreezepanes)() | Размораживает панели на рабочем листе. |
| [Unprotect](../../aspose.cells/worksheet/unprotect#unprotect)() | Снимает защиту с листа. |
| [Unprotect](../../aspose.cells/worksheet/unprotect#unprotect_1)(string) | Снимает защиту с листа. |
| [XmlMapQuery](../../aspose.cells/worksheet/xmlmapquery)(string, XmlMap) | Запрос областей ячеек, которые сопоставлены/связаны с определенным путем карты xml. |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

  // Заморозить панели на "AS40" с 10 строками и 10 столбцами
sheet.FreezePanes("AS40", 10, 10);

//Добавить гиперссылку в ячейку A1
sheet.Hyperlinks.Add("A1", 1, 1, "http:  //www.aspose.com");

[Visual Basic]

Dim workbook as Workbook = new Workbook()

Dim sheet as Worksheet = workbook.Worksheets(0)

'Заморозить панели на "AS40" с 10 строками и 10 столбцами
sheet.FreezePanes("AS40", 10, 10)

'Добавить гиперссылку в ячейку A1
sheet.Hyperlinks.Add("A1", 1, 1, "http:  //www.aspose.com")
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
