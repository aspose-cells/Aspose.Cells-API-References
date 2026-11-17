---
title: "Класс Worksheet"
linktitle: "Worksheet"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Worksheet. Инкапсулирует объект, представляющий лист в Go."
type: docs
weight: 200
url: /ru/go-cpp/worksheet/
---

## Worksheet class

Инкапсулирует объект, представляющий отдельный лист.

```go

type Worksheet struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [Dispose](./dispose/) | Выполняет задачи, определённые приложением, связанные с освобождением, выпуском или сбросом неуправляемых ресурсов. |
| [GetProtection](./getprotection/) | Представляет различные типы параметров защиты, доступные для листа. Поддерживает расширенные параметры защиты в ExcelXP и более новых версиях. |
| [GetUniqueId](./getuniqueid/) | Получает и задает уникальный идентификатор, он совпадает с {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetUniqueId](./setuniqueid/) | Получает и задает уникальный идентификатор, он совпадает с {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [GetPanes](./getpanes/) | Получает области окна. |
| [GetWorkbook](./getworkbook/) | Получает объект книги, содержащий этот лист. |
| [GetCells](./getcells/) | Получает коллекцию Aspose.Cells.Cells. |
| [GetQueryTables](./getquerytables/) | Получает QueryTableCollection в листе. |
| [GetType](./gettype/) | Представляет тип листа. |
| [SetType](./settype/) | Представляет тип листа. |
| [GetName](./getname/) | Получает или задает имя листа. |
| [SetName](./setname/) | Получает или задает имя листа. |
| [GetShowFormulas](./getshowformulas/) | Указывает, показывать ли формулы или их результаты. |
| [SetShowFormulas](./setshowformulas/) | Указывает, показывать ли формулы или их результаты. |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | Указывает, показывать ли значки типов данных. |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | Указывает, показывать ли значки типов данных. |
| [IsGridlinesVisible](./isgridlinesvisible/) | Получает или задает значение, указывающее, видимы ли линии сетки. По умолчанию true. |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | Получает или задает значение, указывающее, видимы ли линии сетки. По умолчанию true. |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | Получает или задает значение, указывающее, будет ли лист отображать заголовки строк и столбцов. По умолчанию true. |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | Получает или задает значение, указывающее, будет ли лист отображать заголовки строк и столбцов. По умолчанию true. |
| [GetPaneState](./getpanestate/) | Указывает, имеет ли область горизонтальные или вертикальные разделения, и заморожены ли эти разделения. |
| [GetDisplayZeros](./getdisplayzeros/) | True, если отображаются нулевые значения. |
| [SetDisplayZeros](./setdisplayzeros/) | True, если отображаются нулевые значения. |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию false. |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию false. |
| [IsOutlineShown](./isoutlineshown/) | Указывает, показывать ли контур. |
| [SetIsOutlineShown](./setisoutlineshown/) | Указывает, показывать ли контур. |
| [IsSelected](./isselected/) | Указывает, будет ли этот лист выбран при открытии книги. |
| [SetIsSelected](./setisselected/) | Указывает, будет ли этот лист выбран при открытии книги. |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | Замораживает области в указанной ячейке листа. |
| [GetFreezedPanes](./getfreezedpanes/) | Получает замороженные области. |
| [Split](./split/) | Разделяет окно. |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | Замораживает области в указанной ячейке листа. |
| [UnFreezePanes](./unfreezepanes/) | Размораживает области в листе. |
| [RemoveSplit](./removesplit/) | Удаляет разделение окна. |
| [GetPivotTables](./getpivottables/) | Получает все сводные таблицы в этом листе. |
| [GetListObjects](./getlistobjects/) | Получает все ListObjects в этом листе. |
| [GetTabId](./gettabid/) | Указывает внутренний идентификатор листа. |
| [SetTabId](./settabid/) | Указывает внутренний идентификатор листа. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Получает коллекцию HorizontalPageBreakCollection. |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | Получает коллекцию VerticalPageBreakCollection. |
| [AddPageBreaks](./addpagebreaks/) | Добавляет разрыв страницы. |
| [GetHyperlinks](./gethyperlinks/) | Получает коллекцию HyperlinkCollection. |
| [Copy_Worksheet](./copy_worksheet/) | Копирует содержимое и форматы из другого листа. |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | Копирует содержимое и форматы из другого листа. |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | Автоматически подгоняет ширину столбца. |
| [AutoFitColumns](./autofitcolumns/) | Автоматически подгоняет все столбцы на этом листе. |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | Автоматически подгоняет все столбцы на этом листе. |
| [AutoFitColumn_Int](./autofitcolumn_int/) | Автоматически подгоняет ширину столбца. |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | Автоматически подгоняет ширину столбцов. |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | Автоматически подгоняет ширину столбцов. |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | Автоматически подгоняет ширину столбцов. |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | Автоматически подгоняет ширину столбцов. |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | Автоматически подгоняет высоту строки. |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | Автоматически подгоняет высоту строки. |
| [AutoFitRows](./autofitrows/) | Автоматически подгоняет все строки на этом листе. |
| [AutoFitRows_Bool](./autofitrows_bool/) | Автоматически подгоняет все строки на этом листе. |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | Автоматически подгоняет все строки на этом листе. |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | Автоматически подгоняет высоту строки в диапазоне. |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | Автоматически подгоняет высоту строки в диапазоне. |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | Автоматически подгоняет высоту строки в прямоугольном диапазоне. |
| [AutoFitRow_Int](./autofitrow_int/) | Автоматически подгоняет высоту строки. |
| [GetPageSetup](./getpagesetup/) | Представляет описание настройки страницы на этом листе. |
| [GetAutoFilter](./getautofilter/) | Представляет автофильтр для указанного листа. |
| [Filter](./filter/) | Фильтрует диапазон. |
| [GetAdvancedFilter](./getadvancedfilter/) | Получает настройки расширенного фильтра. |
| [Advanced_Filter](./advanced_filter/) | Фильтрует данные с использованием сложных критериев. |
| [RemoveAutoFilter](./removeautofilter/) | Удаляет автофильтр листа. |
| [GetHasAutofilter](./gethasautofilter/) | Указывает, имеет ли этот лист автофильтр. |
| [GetTransitionEvaluation](./gettransitionevaluation/) | Указывает, включена ли опция оценки формул перехода (совместимость с Lotus). |
| [SetTransitionEvaluation](./settransitionevaluation/) | Указывает, включена ли опция оценки формул перехода (совместимость с Lotus). |
| [GetTransitionEntry](./gettransitionentry/) | Указывает, включена ли опция ввода формул перехода (совместимость с Lotus). |
| [SetTransitionEntry](./settransitionentry/) | Указывает, включена ли опция ввода формул перехода (совместимость с Lotus). |
| [GetVisibilityType](./getvisibilitytype/) | Указывает видимое состояние этого листа. |
| [SetVisibilityType](./setvisibilitytype/) | Указывает видимое состояние этого листа. |
| [SetVisible](./setvisible/) | Устанавливает параметры видимости. |
| [IsVisible](./isvisible/) | Представляет, видим ли лист. |
| [SetIsVisible](./setisvisible/) | Представляет, видим ли лист. |
| [SelectRange](./selectrange/) | Выбирает диапазон. |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | Удаляет все графические объекты в этом листе. |
| [ClearComments](./clearcomments/) | Очищает все комментарии в таблице дизайнера. |
| [GetSparklineGroups](./getsparklinegroups/) | Получает группы спарклайнов в листе. |
| [GetCharts](./getcharts/) | Получает коллекцию диаграмм |
| [GetComments](./getcomments/) | Получает коллекцию комментариев. |
| [GetPictures](./getpictures/) | Получает коллекцию изображений. |
| [GetAllPictures](./getallpictures/) | Получает все изображения, включая изображения, встроенные в ячейку и находящиеся над ячейками. |
| [GetTextBoxes](./gettextboxes/) | Получает коллекцию текстовых полей. |
| [GetCheckBoxes](./getcheckboxes/) | Получает коллекцию флажков. |
| [GetOleObjects](./getoleobjects/) | Представляет коллекцию объектов OleObject в листе. |
| [GetShapes](./getshapes/) | Возвращает все графические фигуры в этом листе. |
| [GetSlicers](./getslicers/) | Получить коллекцию срезов в листе |
| [GetTimelines](./gettimelines/) | Получить коллекцию временных шкал в листе |
| [Protect_ProtectionType](./protect_protectiontype/) | Защищает лист. |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | Защищает лист. |
| [Unprotect](./unprotect/) | Снимает защиту с листа. |
| [Unprotect_String](./unprotect_string/) | Снимает защиту с листа. |
| [GetIndex](./getindex/) | Получает индекс листа в коллекции листов. |
| [MoveTo](./moveto/) | Перемещает лист в другое место в таблице. |
| [IsProtected](./isprotected/) | Указывает, защищён ли лист. |
| [GetValidations](./getvalidations/) | Получает коллекцию настроек проверки данных в листе. |
| [GetAllowEditRanges](./getalloweditranges/) | Получает коллекцию разрешённых диапазонов редактирования в листе. |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | Получает настройки проверки ошибок, применённые к определённым диапазонам. |
| [GetOutline](./getoutline/) | Получает контур этого листа. |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | Представляет индекс первой видимой строки. |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | Представляет индекс первой видимой строки. |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | Представляет индекс первого видимого столбца. |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | Представляет индекс первого видимого столбца. |
| [Replace](./replace/) | Заменяет текст всех ячеек новой строкой. |
| [GetZoom](./getzoom/) | Представляет коэффициент масштабирования в процентах. Должен быть от 10 до 400. |
| [SetZoom](./setzoom/) | Представляет коэффициент масштабирования в процентах. Должен быть от 10 до 400. |
| [GetViewType](./getviewtype/) | Получает и задает тип представления. |
| [SetViewType](./setviewtype/) | Получает и задает тип представления. |
| [IsPageBreakPreview](./ispagebreakpreview/) | Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц. |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц. |
| [IsRulerVisible](./isrulervisible/) | Указывает, видна ли линейка. Это свойство применяется только в режиме предварительного просмотра разрывов страниц. |
| [SetIsRulerVisible](./setisrulervisible/) | Указывает, видна ли линейка. Это свойство применяется только в режиме предварительного просмотра разрывов страниц. |
| [GetSelectedAreas](./getselectedareas/) | Получает выбранные диапазоны ячеек в конструкторе таблицы. |
| [GetTabColor](./gettabcolor/) | Представляет цвет вкладки листа. |
| [SetTabColor](./settabcolor/) | Представляет цвет вкладки листа. |
| [GetGridlineColor](./getgridlinecolor/) | Получает и задает цвет линий сетки. |
| [SetGridlineColor](./setgridlinecolor/) | Получает и задает цвет линий сетки. |
| [GetCodeName](./getcodename/) | Получает кодовое имя листа. |
| [SetCodeName](./setcodename/) | Получает кодовое имя листа. |
| [GetBackgroundImage](./getbackgroundimage/) | Получает и задает фоновое изображение листа. |
| [SetBackgroundImage](./setbackgroundimage/) | Получает и задает фоновое изображение листа. |
| [GetConditionalFormattings](./getconditionalformattings/) | Получает условные форматирования в листе. |
| [GetActiveCell](./getactivecell/) | Получает или задает активную ячейку в листе. |
| [SetActiveCell](./setactivecell/) | Получает или задает активную ячейку в листе. |
| [GetCustomProperties](./getcustomproperties/) | Получает объект, представляющий информацию идентификатора, связанную с листом. |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | Получает автоматические разрывы страниц. |
| [GetSmartTagSetting](./getsmarttagsetting/) | Получает все объекты SmartTagCollection листа. |
| [ToString](./tostring/) | Возвращает строку, представляющую текущий объект Worksheet. |
| [GetScenarios](./getscenarios/) | Получает коллекцию сценариев. |
| [StartAccessCache](./startaccesscache/) | Запускает сеанс, использующий кэш для доступа к данным в этом листе. |
| [CloseAccessCache](./closeaccesscache/) | Закрывает сеанс, использующий кэш для доступа к данным в этом листе. |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Преобразует стиль ссылок формулы. |
| [CalculateFormula_String](./calculateformula_string/) | Вычисляет формулу. |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | Вычисляет выражение формулы напрямую. |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | Вычисляет выражение формулы напрямую. |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | Вычисляет формулу как массивную формулу. |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | Вычисляет формулу как массивную формулу. |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | Вычисляет формулу как массивную формулу. |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | Вычисляет все формулы в этом листе. |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | Запрашивает области ячеек, сопоставленные/связанные с конкретным путем XML‑карты. |
| [GetCellWatches](./getcellwatches/) | Получает коллекцию ячеек на этом листе, наблюдаемых в «окне наблюдения». |
| [RefreshPivotTables](./refreshpivottables/) | Обновляет все сводные таблицы на этом листе. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Обновляет все сводные таблицы на этом листе. |
