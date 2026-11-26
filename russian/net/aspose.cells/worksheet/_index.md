---
title: "Класс Worksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Worksheet. Инкапсулирует объект, представляющий отдельный рабочий лист"
type: docs
url: /ru/net/aspose.cells/worksheet/
---
## Worksheet class

Инкапсулирует объект, представляющий отдельный лист.

```csharp
public class Worksheet : IDisposable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ActiveCell](../../aspose.cells/worksheet/activecell/) { get; set; } | Получает или задает активную ячейку в рабочем листе. |
| [AllowEditRanges](../../aspose.cells/worksheet/alloweditranges/) { get; } | Получает коллекцию разрешённых диапазонов редактирования в рабочем листе. |
| [AutoFilter](../../aspose.cells/worksheet/autofilter/) { get; } | Представляет автофильтр для указанного рабочего листа. |
| [BackgroundImage](../../aspose.cells/worksheet/backgroundimage/) { get; set; } | Получает и задает фоновое изображение рабочего листа. |
| [Cells](../../aspose.cells/worksheet/cells/) { get; } | Получает коллекцию [`Cells`](../cells/). |
| [CellWatches](../../aspose.cells/worksheet/cellwatches/) { get; } | Получает коллекцию ячеек этого листа, наблюдаемых в окне 'watch window'. |
| [Charts](../../aspose.cells/worksheet/charts/) { get; } | Получает коллекцию [`Chart`](../../aspose.cells.charts/chart/) |
| [CheckBoxes](../../aspose.cells/worksheet/checkboxes/) { get; } | Получает коллекцию [`CheckBox`](../../aspose.cells.drawing/checkbox/). |
| [CodeName](../../aspose.cells/worksheet/codename/) { get; set; } | Получает кодовое имя рабочего листа. |
| [Comments](../../aspose.cells/worksheet/comments/) { get; } | Получает коллекцию [`Comment`](../comment/). |
| [ConditionalFormattings](../../aspose.cells/worksheet/conditionalformattings/) { get; } | Получает ConditionalFormattings в рабочем листе. |
| [CustomProperties](../../aspose.cells/worksheet/customproperties/) { get; } | Получает объект, представляющий информацию об идентификаторе, связанную с рабочим листом. |
| [DisplayRightToLeft](../../aspose.cells/worksheet/displayrighttoleft/) { get; set; } | Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию false. |
| [DisplayZeros](../../aspose.cells/worksheet/displayzeros/) { get; set; } | True, если отображаются нулевые значения. |
| [ErrorCheckOptions](../../aspose.cells/worksheet/errorcheckoptions/) { get; } | Получает настройки проверки ошибок, применяемые к определённым диапазонам. |
| [FirstVisibleColumn](../../aspose.cells/worksheet/firstvisiblecolumn/) { get; set; } | Представляет индекс первой видимой колонки. |
| [FirstVisibleRow](../../aspose.cells/worksheet/firstvisiblerow/) { get; set; } | Представляет индекс первой видимой строки. |
| [GridlineColor](../../aspose.cells/worksheet/gridlinecolor/) { get; set; } | Получает и задаёт цвет линий сетки |
| [HasAutofilter](../../aspose.cells/worksheet/hasautofilter/) { get; } | Указывает, имеет ли этот лист автофильтр. |
| [HorizontalPageBreaks](../../aspose.cells/worksheet/horizontalpagebreaks/) { get; } | Получает коллекцию [`HorizontalPageBreakCollection`](../horizontalpagebreakcollection/). |
| [Hyperlinks](../../aspose.cells/worksheet/hyperlinks/) { get; } | Получает коллекцию [`HyperlinkCollection`](../hyperlinkcollection/). |
| [Index](../../aspose.cells/worksheet/index/) { get; } | Получает индекс листа в коллекции листов. |
| [IsGridlinesVisible](../../aspose.cells/worksheet/isgridlinesvisible/) { get; set; } | Получает или задаёт значение, указывающее, видимы ли линии сетки. По умолчанию true. |
| [IsOutlineShown](../../aspose.cells/worksheet/isoutlineshown/) { get; set; } | Указывает, показывать ли контур. |
| [IsPageBreakPreview](../../aspose.cells/worksheet/ispagebreakpreview/) { get; set; } | Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц. |
| [IsProtected](../../aspose.cells/worksheet/isprotected/) { get; } | Указывает, защищён ли лист. |
| [IsRowColumnHeadersVisible](../../aspose.cells/worksheet/isrowcolumnheadersvisible/) { get; set; } | Получает или задаёт значение, указывающее, будет ли лист отображать заголовки строк и столбцов. По умолчанию true. |
| [IsRulerVisible](../../aspose.cells/worksheet/isrulervisible/) { get; set; } | Указывает, видима ли линейка. Это свойство применяется только в режиме предварительного просмотра разрывов страниц. |
| [IsSelected](../../aspose.cells/worksheet/isselected/) { get; set; } | Указывает, выбран ли этот лист при открытии книги. |
| [IsVisible](../../aspose.cells/worksheet/isvisible/) { get; set; } | Представляет, видим ли лист. |
| [ListObjects](../../aspose.cells/worksheet/listobjects/) { get; } | Получает все ListObjects в этом листе. |
| [Name](../../aspose.cells/worksheet/name/) { get; set; } | Получает или задаёт имя листа. |
| [OleObjects](../../aspose.cells/worksheet/oleobjects/) { get; } | Представляет коллекцию [`OleObject`](../../aspose.cells.drawing/oleobject/) в листе. |
| [Outline](../../aspose.cells/worksheet/outline/) { get; } | Получает контур этого листа. |
| [PageSetup](../../aspose.cells/worksheet/pagesetup/) { get; } | Представляет описание параметров страницы в этом листе. |
| [PaneState](../../aspose.cells/worksheet/panestate/) { get; } | Указывает, имеет ли панель горизонтальное или вертикальное разделение, и заморожены ли эти разделения. |
| [Pictures](../../aspose.cells/worksheet/pictures/) { get; } | Получает коллекцию [`Picture`](../../aspose.cells.drawing/picture/). |
| [PivotTables](../../aspose.cells/worksheet/pivottables/) { get; } | Получает все сводные таблицы в этом листе. |
| [Protection](../../aspose.cells/worksheet/protection/) { get; } | Представляет различные типы параметров защиты, доступных для листа. Поддерживает расширенные параметры защиты в ExcelXP и более новых версиях. |
| [QueryTables](../../aspose.cells/worksheet/querytables/) { get; } | Получает [`QueryTableCollection`](../querytablecollection/) в листе. |
| [Scenarios](../../aspose.cells/worksheet/scenarios/) { get; } | Получает коллекцию [`Scenario`](../scenario/). |
| [Shapes](../../aspose.cells/worksheet/shapes/) { get; } | Возвращает все графические фигуры в этом листе. |
| [ShowDataTypeIcons](../../aspose.cells/worksheet/showdatatypeicons/) { get; set; } | Указывает, показывать ли значки типов данных. |
| [ShowFormulas](../../aspose.cells/worksheet/showformulas/) { get; set; } | Указывает, показывать ли формулы или их результаты. |
| [Slicers](../../aspose.cells/worksheet/slicers/) { get; } | Получить коллекцию Slicer в листе |
| [SmartTagSetting](../../aspose.cells/worksheet/smarttagsetting/) { get; } | Получает все объекты [`SmartTagCollection`](../../aspose.cells.markup/smarttagcollection/) листа. |
| [SparklineGroups](../../aspose.cells/worksheet/sparklinegroups/) { get; } | Получает группы спарклайнов в листе. |
| [TabColor](../../aspose.cells/worksheet/tabcolor/) { get; set; } | Представляет цвет вкладки листа. |
| [TabId](../../aspose.cells/worksheet/tabid/) { get; set; } | Указывает внутренний идентификатор листа. |
| [TextBoxes](../../aspose.cells/worksheet/textboxes/) { get; } | Получает коллекцию [`TextBox`](../../aspose.cells.drawing/textbox/). |
| [Timelines](../../aspose.cells/worksheet/timelines/) { get; } | Получить коллекцию Timeline в листе |
| [TransitionEntry](../../aspose.cells/worksheet/transitionentry/) { get; set; } | Указывает, включена ли опция Transition Formula Entry (совместимость с Lotus). |
| [TransitionEvaluation](../../aspose.cells/worksheet/transitionevaluation/) { get; set; } | Указывает, включена ли опция Transition Formula Evaluation (совместимость с Lotus). |
| [Type](../../aspose.cells/worksheet/type/) { get; set; } | Представляет тип листа. |
| [UniqueId](../../aspose.cells/worksheet/uniqueid/) { get; set; } | Получает и задает уникальный идентификатор, он совпадает с {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [Validations](../../aspose.cells/worksheet/validations/) { get; } | Получает коллекцию настроек проверки данных в листе. |
| [VerticalPageBreaks](../../aspose.cells/worksheet/verticalpagebreaks/) { get; } | Получает коллекцию [`VerticalPageBreakCollection`](../verticalpagebreakcollection/). |
| [ViewType](../../aspose.cells/worksheet/viewtype/) { get; set; } | Получает и задает тип представления. |
| [VisibilityType](../../aspose.cells/worksheet/visibilitytype/) { get; set; } | Указывает видимое состояние этого листа. |
| [Workbook](../../aspose.cells/worksheet/workbook/) { get; } | Получает объект книги, содержащий этот лист. |
| [Zoom](../../aspose.cells/worksheet/zoom/) { get; set; } | Представляет коэффициент масштабирования в процентах. Должен быть в диапазоне от 10 до 400. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddPageBreaks](../../aspose.cells/worksheet/addpagebreaks/)(string) | Добавляет разрыв страницы. |
| [AdvancedFilter](../../aspose.cells/worksheet/advancedfilter/)(bool, string, string, string, bool) | Фильтрует данные, используя сложные критерии. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn/#autofitcolumn)(int) | Автоматически подгоняет ширину столбца. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Автоматически подгоняет ширину столбца. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns)() | Автоматически подгоняет все столбцы в этом листе. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_1)(AutoFitterOptions) | Автоматически подгоняет все столбцы в этом листе. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_2)(int, int) | Автоматически подгоняет ширину столбцов. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_3)(int, int, AutoFitterOptions) | Автоматически подгоняет ширину столбцов. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_4)(int, int, int, int) | Автоматически подгоняет ширину столбцов. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_5)(int, int, int, int, AutoFitterOptions) | Автоматически подгоняет ширину столбцов. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow)(int) | Автоматически подгоняет высоту строки. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_1)(int, int, int) | Автоматически подгоняет высоту строки. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_2)(int, int, int, AutoFitterOptions) | Автоматически подгоняет высоту строки. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_3)(int, int, int, int) | Автоматически подгоняет высоту строки в прямоугольном диапазоне. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows)() | Автоматически подгоняет все строки в этом листе. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_1)(AutoFitterOptions) | Автоматически подгоняет все строки в этом листе. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_2)(bool) | Автоматически подгоняет все строки в этом листе. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_3)(int, int) | Автоматически подгоняет высоту строки в диапазоне. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_4)(int, int, AutoFitterOptions) | Автоматически подгоняет высоту строки в диапазоне. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula)(string, CalculationOptions) | Вычисляет формулу как массивную формулу. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula_1)(string, CalculationOptions, int, int) | Вычисляет формулу как массивную формулу. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula_2)(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) | Вычисляет формулу как массивную формулу. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula)(string) | Вычисляет формулу. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_3)(CalculationOptions, bool) | Вычисляет все формулы в этом листе. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_1)(string, CalculationOptions) | Вычисляет выражение формулы напрямую. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_2)(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) | Вычисляет выражение формулы напрямую. |
| [ClearComments](../../aspose.cells/worksheet/clearcomments/)() | Очищает все комментарии в проектируемой таблице. |
| [CloseAccessCache](../../aspose.cells/worksheet/closeaccesscache/)(AccessCacheOptions) | Закрывает сеанс, использующий кэш для доступа к данным в этом листе. |
| [ConvertFormulaReferenceStyle](../../aspose.cells/worksheet/convertformulareferencestyle/)(string, bool, int, int) | Преобразует стиль ссылок в формуле. |
| [Copy](../../aspose.cells/worksheet/copy/#copy)(Worksheet) | Копирует содержимое и форматы из другого листа. |
| [Copy](../../aspose.cells/worksheet/copy/#copy_1)(Worksheet, CopyOptions) | Копирует содержимое и форматы из другого листа. |
| [Dispose](../../aspose.cells/worksheet/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [Filter](../../aspose.cells/worksheet/filter/)(CellArea) | Фильтрует диапазон. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes/#freezepanes_1)(string, int, int) | Замораживает области в указанной ячейке листа. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes/#freezepanes)(int, int, int, int) | Замораживает области в указанной ячейке листа. |
| [GetAdvancedFilter](../../aspose.cells/worksheet/getadvancedfilter/)() | Получает настройки расширенного фильтра. |
| [GetAllPictures](../../aspose.cells/worksheet/getallpictures/)() | Получает все изображения, включая вложенные в ячейку и находящиеся над ячейками. |
| [GetAreasOfXmlMapQuery](../../aspose.cells/worksheet/getareasofxmlmapquery/)(string, XmlMap) | Запрашивает области ячеек, сопоставленные/связанные с конкретным путём XML‑карты. |
| [GetFreezedPanes](../../aspose.cells/worksheet/getfreezedpanes/)(out int, out int, out int, out int) | Получает замороженные области. |
| [GetPanes](../../aspose.cells/worksheet/getpanes/)() | Получает области окна. |
| [GetPrintingPageBreaks](../../aspose.cells/worksheet/getprintingpagebreaks/)(ImageOrPrintOptions) | Получает автоматические разрывы страниц. |
| [GetSelectedAreas](../../aspose.cells/worksheet/getselectedareas/)() | Получает выбранные диапазоны ячеек в проектируемой таблице. |
| [GetSelectedRanges](../../aspose.cells/worksheet/getselectedranges/)() | (**Obsolete.**) Получает выбранные диапазоны ячеек в проектируемой таблице. |
| [MoveTo](../../aspose.cells/worksheet/moveto/)(int) | Перемещает лист в другое место в таблице. |
| [Protect](../../aspose.cells/worksheet/protect/#protect)(ProtectionType) | Защищает лист. |
| [Protect](../../aspose.cells/worksheet/protect/#protect_1)(ProtectionType, string, string) | Защищает лист. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables/#refreshpivottables_1)() | Обновляет все сводные таблицы в этом листе. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Обновляет все сводные таблицы в этом листе. |
| [RemoveAllDrawingObjects](../../aspose.cells/worksheet/removealldrawingobjects/)() | Удаляет все графические объекты в этом листе. |
| [RemoveAutoFilter](../../aspose.cells/worksheet/removeautofilter/)() | Удаляет автофильтр листа. |
| [RemoveSplit](../../aspose.cells/worksheet/removesplit/)() | Удаляет разделённое окно. |
| [Replace](../../aspose.cells/worksheet/replace/)(string, string) | Заменяет весь текст ячеек новой строкой. |
| [SelectRange](../../aspose.cells/worksheet/selectrange/)(int, int, int, int, bool) | Выбирает диапазон. |
| [SetVisible](../../aspose.cells/worksheet/setvisible/)(bool, bool) | Устанавливает видимые параметры. |
| [Split](../../aspose.cells/worksheet/split/)() | Разделяет окно. |
| [StartAccessCache](../../aspose.cells/worksheet/startaccesscache/)(AccessCacheOptions) | Запускает сеанс, использующий кэш для доступа к данным в этом листе. |
| override [ToString](../../aspose.cells/worksheet/tostring/)() | Возвращает строку, представляющую текущий объект листа. |
| [UnFreezePanes](../../aspose.cells/worksheet/unfreezepanes/)() | Размораживает области в листе. |
| [Unprotect](../../aspose.cells/worksheet/unprotect/#unprotect)() | Снимает защиту с листа. |
| [Unprotect](../../aspose.cells/worksheet/unprotect/#unprotect_1)(string) | Снимает защиту с листа. |
| [XmlMapQuery](../../aspose.cells/worksheet/xmlmapquery/)(string, XmlMap) | (**Obsolete.**) Запрашивает области ячеек, сопоставленные/связанные с конкретным путём XML‑карты. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetDemo
    {
        public static void WorksheetExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить свойства листа
            worksheet.Name = "DemoSheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.IsRowColumnHeadersVisible = true;
            worksheet.DisplayZeros = true;
            worksheet.DisplayRightToLeft = false;
            worksheet.IsOutlineShown = true;
            worksheet.IsSelected = true;
            worksheet.FirstVisibleRow = 0;
            worksheet.FirstVisibleColumn = 0;
            worksheet.Zoom = 100;
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsPageBreakPreview = false;
            worksheet.IsRulerVisible = true;
            worksheet.TabColor = System.Drawing.Color.Blue;
            worksheet.CodeName = "Sheet1";
            worksheet.ActiveCell = "A1";

            // Добавить гиперссылку в ячейку A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Заморозить области в "C3" с 3 строками и 3 столбцами
            worksheet.FreezePanes("C3", 3, 3);

            // Добавить правило условного форматирования
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Настройка свойств правила AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Сохраните книгу
            workbook.Save("WorksheetExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


