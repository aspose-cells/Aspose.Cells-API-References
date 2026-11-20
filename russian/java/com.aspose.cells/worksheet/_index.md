---
title: "Worksheet"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий отдельный лист."
type: docs
url: /ru/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

Инкапсулирует объект, представляющий отдельный лист.

**Example**

В следующем примере показано, как закрепить области и вставить гиперссылку в лист с помощью .Net или VB.

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | Добавляет разрыв страницы. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | Фильтрует данные, используя сложные критерии. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Автоматически подгоняет ширину столбца. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Автоматически подгоняет ширину столбца. |
| [autoFitColumns()](#autoFitColumns--) | Автоматически подгоняет ширину всех столбцов в этом листе. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | Автоматически подгоняет ширину всех столбцов в этом листе. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | Автоматически подгоняет ширину столбцов. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | Автоматически подгоняет ширину столбцов. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | Автоматически подгоняет ширину столбцов. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | Автоматически подгоняет ширину столбцов. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Автоматически подгоняет высоту строки. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Автоматически подгоняет высоту строки. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | Автоматически подгоняет высоту строки. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Автоматически подгоняет высоту строки в прямоугольном диапазоне. |
| [autoFitRows()](#autoFitRows--) | Автоматически подгоняет высоту всех строк в этом листе. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Автоматически подгоняет высоту всех строк в этом листе. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | Автоматически подгоняет высоту всех строк в этом листе. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Автоматически подгоняет высоту строки в диапазоне. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | Автоматически подгоняет высоту строки в диапазоне. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Вычисляет формулу как массивную формулу. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | Вычисляет формулу как массивную формулу. |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | Вычисляет формулу как массивную формулу. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | Вычисляет все формулы в этом листе. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Вычисляет формулу. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Вычисляет выражение формулы напрямую. |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | Вычисляет выражение формулы напрямую. |
| [clearComments()](#clearComments--) | Очищает все комментарии в дизайнерской таблице. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Закрывает сеанс, использующий кэш для доступа к данным в этом листе. |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | Преобразует стиль ссылок в формуле. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | Копирует содержимое и форматы из другого листа. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | Копирует содержимое и форматы из другого листа. |
| [dispose()](#dispose--) | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | Фильтрует диапазон. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Замораживает области в указанной ячейке листа. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Замораживает области в указанной ячейке листа. |
| [getActiveCell()](#getActiveCell--) | Получает активную ячейку в листе. |
| [getAdvancedFilter()](#getAdvancedFilter--) | Получает настройки расширенного фильтра. |
| [getAllPictures()](#getAllPictures--) | Получает все изображения, включая вложенные в ячейку и находящиеся над ячейками. |
| [getAllowEditRanges()](#getAllowEditRanges--) | Получает коллекцию разрешённых диапазонов редактирования в листе. |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Запрашивает области ячеек, сопоставленные/связанные с конкретным путём XML‑карты. |
| [getAutoFilter()](#getAutoFilter--) | Представляет автофильтр для указанного листа. |
| [getBackgroundImage()](#getBackgroundImage--) | Получает фоновое изображение листа. |
| [getCellWatches()](#getCellWatches--) | Получает коллекцию ячеек на этом листе, наблюдаемых в ‘окне наблюдения’. |
| [getCells()](#getCells--) | Получает коллекцию [Cells](../../com.aspose.cells/cells). |
| [getCharts()](#getCharts--) | Получает коллекцию [Chart](../../com.aspose.cells/chart) |
| [getCheckBoxes()](#getCheckBoxes--) | Получает коллекцию [CheckBox](../../com.aspose.cells/checkbox). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Получает кодовое имя листа. |
| [getComments()](#getComments--) | Получает коллекцию [Comment](../../com.aspose.cells/comment). |
| [getConditionalFormattings()](#getConditionalFormattings--) | Получает ConditionalFormattings на листе. |
| [getCustomProperties()](#getCustomProperties--) | Получает объект, представляющий информацию об идентификаторе, связанную с листом. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Указывает, отображается ли указанный лист справа налево вместо слева направо. |
| [getDisplayZeros()](#getDisplayZeros--) | True, если отображаются нулевые значения. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | Получает настройки проверки ошибок, применяемые к определённым диапазонам. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Представляет индекс первой видимой колонки. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Представляет индекс первой видимой строки. |
| [getFreezedPanes()](#getFreezedPanes--) | Получает замороженные области. |
| [getGridlineColor()](#getGridlineColor--) | Получает цвет линий сетки |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Получает коллекцию [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection). |
| [getHyperlinks()](#getHyperlinks--) | Получает коллекцию [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection). |
| [getIndex()](#getIndex--) | Получает индекс листа в коллекции листов. |
| [getListObjects()](#getListObjects--) | Получает все ListObjects на этом листе. |
| [getName()](#getName--) | Получает имя листа. |
| [getOleObjects()](#getOleObjects--) | Представляет коллекцию [OleObject](../../com.aspose.cells/oleobject) на листе. |
| [getOutline()](#getOutline--) | Получает структуру на этом листе. |
| [getPageSetup()](#getPageSetup--) | Представляет описание настройки страницы в этом листе. |
| [getPaneState()](#getPaneState--) | Указывает, имеет ли панель горизонтальные или вертикальные разбиения и заморожены ли они. |
| [getPanes()](#getPanes--) | Получает оконные панели. |
| [getPictures()](#getPictures--) | Получает коллекцию [Picture](../../com.aspose.cells/picture). |
| [getPivotTables()](#getPivotTables--) | Получает все сводные таблицы в этом листе. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | Получает автоматические разрывы страниц. |
| [getProtection()](#getProtection--) | Представляет различные типы параметров защиты, доступных для листа. |
| [getQueryTables()](#getQueryTables--) | Получает [QueryTableCollection](../../com.aspose.cells/querytablecollection) в листе. |
| [getScenarios()](#getScenarios--) | Получает коллекцию [Scenario](../../com.aspose.cells/scenario). |
| [getSelectedAreas()](#getSelectedAreas--) | Получает выбранные диапазоны ячеек в дизайнерской таблице. |
| [getSelectedRanges()](#getSelectedRanges--) | Получает выбранные диапазоны ячеек в дизайнерской таблице. |
| [getShapes()](#getShapes--) | Возвращает все графические объекты в этом листе. |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | Указывает, показывать ли значки типов данных. |
| [getShowFormulas()](#getShowFormulas--) | Указывает, показывать ли формулы или их результаты. |
| [getSlicers()](#getSlicers--) | Получить коллекцию Slicer в листе |
| [getSmartTagSetting()](#getSmartTagSetting--) | Получает все объекты [SmartTagCollection](../../com.aspose.cells/smarttagcollection) листа. |
| [getSparklineGroups()](#getSparklineGroups--) | Получает группы спарклайнов в листе. |
| [getTabColor()](#getTabColor--) | Представляет цвет вкладки листа. |
| [getTabId()](#getTabId--) | Указывает внутренний идентификатор листа. |
| [getTextBoxes()](#getTextBoxes--) | Получает коллекцию [TextBox](../../com.aspose.cells/textbox). |
| [getTimelines()](#getTimelines--) | Получить коллекцию Timeline в листе |
| [getTransitionEntry()](#getTransitionEntry--) | Указывает, включена ли опция Transition Formula Entry (совместимость с Lotus). |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | Указывает, включена ли опция Transition Formula Evaluation (совместимость с Lotus). |
| [getType()](#getType--) | Представляет тип листа. |
| [getUniqueId()](#getUniqueId--) | Получает уникальный идентификатор, он такой же как \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [getValidations()](#getValidations--) | Получает коллекцию настроек проверки данных в листе. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | Получает коллекцию [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection). |
| [getViewType()](#getViewType--) | Получает тип представления. |
| [getVisibilityType()](#getVisibilityType--) | Указывает видимое состояние этого листа. |
| [getWorkbook()](#getWorkbook--) | Получает объект рабочей книги, содержащий этот лист. |
| [getZoom()](#getZoom--) | Представляет коэффициент масштабирования в процентах. |
| [hasAutofilter()](#hasAutofilter--) | Указывает, имеет ли этот лист автофильтр. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Получает значение, указывающее, видимы ли линии сетки. По умолчанию true. |
| [isOutlineShown()](#isOutlineShown--) | Указывает, показывать ли контур. |
| [isPageBreakPreview()](#isPageBreakPreview--) | Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц. |
| [isProtected()](#isProtected--) | Указывает, защищён ли лист. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | Получает значение, указывающее, будет ли лист отображать заголовки строк и столбцов. |
| [isRulerVisible()](#isRulerVisible--) | Указывает, видима ли линейка. |
| [isSelected()](#isSelected--) | Указывает, будет ли этот лист выбран при открытии книги. |
| [isVisible()](#isVisible--) | Представляет, видим ли лист. |
| [moveTo(int index)](#moveTo-int-) | Перемещает лист в другое место в таблице. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | Защищает лист. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | Защищает лист. |
| [refreshPivotTables()](#refreshPivotTables--) | Обновляет все сводные таблицы в этом листе. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Обновляет все сводные таблицы в этом листе. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | Удаляет все графические объекты в этом листе. |
| [removeAutoFilter()](#removeAutoFilter--) | Удаляет автофильтр листа. |
| [removeSplit()](#removeSplit--) | Удаляет разделение окна. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | Заменяет текст всех ячеек новой строкой. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | Выбирает диапазон. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Устанавливает активную ячейку в листе. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Устанавливает фоновое изображение листа. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | Получает кодовое имя листа. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Указывает, отображается ли указанный лист справа налево вместо слева направо. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | True, если отображаются нулевые значения. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Представляет индекс первой видимой колонки. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Представляет индекс первой видимой строки. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Устанавливает цвет линий сетки |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Устанавливает значение, указывающее, видимы ли линии сетки. По умолчанию true. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя листа. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Указывает, показывать ли контур. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | Устанавливает значение, указывающее, будет ли лист отображать заголовки строк и столбцов. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | Указывает, видима ли линейка. |
| [setSelected(boolean value)](#setSelected-boolean-) | Указывает, будет ли этот лист выбран при открытии книги. |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | Указывает, показывать ли значки типов данных. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | Указывает, показывать ли формулы или их результаты. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | Представляет цвет вкладки листа. |
| [setTabId(int value)](#setTabId-int-) | Указывает внутренний идентификатор листа. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | Указывает, включена ли опция Transition Formula Entry (совместимость с Lotus). |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | Указывает, включена ли опция Transition Formula Evaluation (совместимость с Lotus). |
| [setType(int value)](#setType-int-) | Представляет тип листа. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | Устанавливает уникальный идентификатор, он такой же, как \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [setViewType(int value)](#setViewType-int-) | Устанавливает тип представления. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | Указывает видимое состояние этого листа. |
| [setVisible(boolean value)](#setVisible-boolean-) | Представляет, видим ли лист. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | Устанавливает видимые параметры. |
| [setZoom(int value)](#setZoom-int-) | Представляет коэффициент масштабирования в процентах. |
| [split()](#split--) | Разделяет окно. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Запускает сеанс, который использует кэш для доступа к данным в этом листе. |
| [toString()](#toString--) | Возвращает строку, представляющую текущий объект Worksheet. |
| [unFreezePanes()](#unFreezePanes--) | Размораживает области в листе. |
| [unprotect()](#unprotect--) | Снимает защиту с листа. |
| [unprotect(String password)](#unprotect-java.lang.String-) | Снимает защиту с листа. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Запрашивает области ячеек, сопоставленные/связанные с конкретным путём XML‑карты. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


Добавляет разрыв страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


Фильтрует данные, используя сложные критерии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isFilter | boolean | Указывает, применяется ли фильтрация списка на месте. |
| listRange | java.lang.String | Диапазон списка. |
| criteriaRange | java.lang.String | Диапазон критериев. |
| copyTo | java.lang.String | Диапазон, в который копируются данные. |
| uniqueRecordOnly | boolean | Только отображение или копирование уникальных строк. |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Автоматически подгоняет ширину столбца.

**Remarks**

AutoFitColumn является неточной функцией.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Автоматически подгоняет ширину столбца.

**Remarks**

Этот метод автоматически подгоняет высоту строки на основе содержимого в диапазоне ячеек внутри строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |
| firstRow | int | Индекс первой строки. |
| lastRow | int | Индекс последней строки. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```


Автоматически подгоняет ширину всех столбцов в этом листе.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


Автоматически подгоняет ширину всех столбцов в этом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Параметры автоматической подгонки |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


Автоматически подгоняет ширину столбцов.

**Remarks**

AutoFitColumn является неточной функцией.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstColumn | int | Индекс первого столбца. |
| lastColumn | int | Последний индекс столбца. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


Автоматически подгоняет ширину столбцов.

**Remarks**

AutoFitColumn является неточной функцией.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstColumn | int | Индекс первого столбца. |
| lastColumn | int | Последний индекс столбца. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Параметры автоматической подгонки |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


Автоматически подгоняет ширину столбцов.

**Remarks**

AutoFitColumn является неточной функцией.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Индекс первой строки. |
| firstColumn | int | Индекс первого столбца. |
| lastRow | int | Индекс последней строки. |
| lastColumn | int | Последний индекс столбца. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


Автоматически подгоняет ширину столбцов.

**Remarks**

AutoFitColumn является неточной функцией.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Индекс первой строки. |
| firstColumn | int | Индекс первого столбца. |
| lastRow | int | Индекс последней строки. |
| lastColumn | int | Последний индекс столбца. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Параметры автоматической подгонки |

### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Автоматически подгоняет высоту строки.

**Remarks**

AutoFitRow — неточная функция.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Автоматически подгоняет высоту строки.

**Remarks**

Этот метод автоматически подгоняет высоту строки на основе содержимого в диапазоне ячеек внутри строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |
| firstColumn | int | Индекс первого столбца. |
| lastColumn | int | Последний индекс столбца. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```


Автоматически подгоняет высоту строки.

**Remarks**

Этот метод автоматически подгоняет высоту строки на основе содержимого в диапазоне ячеек внутри строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |
| firstColumn | int | Индекс первого столбца. |
| lastColumn | int | Последний индекс столбца. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Параметры автофиттера |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Автоматически подгоняет высоту строки в прямоугольном диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| endRow | int | Индекс конечной строки. |
| startColumn | int | Индекс начального столбца. |
| endColumn | int | Индекс конечного столбца. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Автоматически подгоняет высоту всех строк в этом листе.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Автоматически подгоняет высоту всех строк в этом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| onlyAuto | boolean | True, только автоматически подгоняет высоту строки, когда высота строки не настроена вручную. |

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


Автоматически подгоняет высоту всех строк в этом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Параметры автофиттера |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Автоматически подгоняет высоту строки в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| endRow | int | Индекс конечной строки. |

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


Автоматически подгоняет высоту строки в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| endRow | int | Индекс конечной строки. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Параметры автофиттера. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


Вычисляет формулу как массивную формулу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула для вычисления. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры вычисления формулы |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


Вычисляет формулу как массивную формулу.

**Remarks**

Формула будет рассматриваться как формула динамического массива для вычисления размеров и результата. Указанный пользователем максимальный размер используется в случаях, когда вычисленный результат представляет большой набор данных (например, результат может соответствовать целой строке или столбцу), но пользователь не нуждается в таком большом массиве в соответствии с бизнес‑требованиями или соображениями производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула для вычисления. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры вычисления формулы |
| maxRowCount | int | максимальное количество строк результирующих данных. Если оно неположительно или превышает фактическое количество строк, будет использовано фактическое количество строк. |
| maxColumnCount | int | максимальное количество столбцов результирующих данных. Если оно неположительно или превышает фактическое количество строк, будет использовано фактическое количество столбцов. |

**Returns:**
java.lang.Object[][] - Вычисленный результат формулы.
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


Вычисляет формулу как массивную формулу.

**Remarks**

Формула будет рассматриваться как формула динамического массива для вычисления размеров и результата. Указанный пользователем максимальный размер используется в случаях, когда вычисленный результат представляет большой набор данных (например, результат может соответствовать целой строке или столбцу), но пользователь не нуждается в таком большом массиве в соответствии с бизнес‑требованиями или соображениями производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула для вычисления. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Параметры разбора формулы |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры вычисления формулы |
| baseCellRow | int | Индекс строки базовой ячейки. |
| baseCellColumn | int | Индекс столбца базовой ячейки. |
| maxRowCount | int | Максимальное количество строк результирующих данных. Если оно неположительно или превышает фактическое количество строк, будет использовано фактическое количество строк. |
| maxColumnCount | int | Максимальное количество столбцов результирующих данных. Если оно неположительно или превышает фактическое количество строк, будет использовано фактическое количество столбцов. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Данные расчёта. Они используются в случае, когда пользователю необходимо вычислить некоторые статические формулы при реализации собственного движка расчётов. Для такого случая пользователь должен указать их с помощью данных расчёта, предоставляемых для [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object[][] - Вычисленный результат формулы.
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


Вычисляет все формулы в этом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры расчёта |
| recursive | boolean | True означает, что если ячейки листа зависят от ячеек других листов, зависимые ячейки в других листах также будут рассчитаны. False означает, что все формулы на листе уже рассчитаны и значения верны. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Вычисляет формулу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула для вычисления. |

**Returns:**
java.lang.Object - Результат вычисленной формулы.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


Вычисляет выражение формулы напрямую.

**Remarks**

Формула будет вычислена так же, как если бы она была установлена в ячейку A1. И формула будет рассматриваться как обычная формула. Если необходимо вычислить формулу как массивную и получить массив в качестве результата, используйте [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-) вместо этого.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула для вычисления. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры вычисления формулы |

**Returns:**
java.lang.Object - Вычисленный результат заданной формулы. Возвращаемый объект может быть одного из возможных типов, указанных в [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), или ReferredArea.
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


Вычисляет выражение формулы напрямую.

**Remarks**

Формула будет вычислена так же, как если бы она была установлена в указанную базовую ячейку. И формула будет рассматриваться как обычная формула. Если необходимо вычислить формулу как массивную и получить массив в качестве результата, используйте [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-) вместо этого.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула для вычисления. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Параметры разбора формулы. |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры вычисления формулы. |
| baseCellRow | int | Индекс строки базовой ячейки. |
| baseCellColumn | int | Индекс столбца базовой ячейки. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Данные расчёта. Они используются в случае, когда пользователю необходимо вычислить некоторые статические формулы при реализации собственного движка расчётов. Для такого случая пользователь должен указать их с помощью данных расчёта, предоставляемых для [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object - Вычисленный результат заданной формулы. Возвращаемый объект может быть одного из возможных типов, указанных в [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), или ReferredArea.
### clearComments() {#clearComments--}
```
public void clearComments()
```


Очищает все комментарии в дизайнерской таблице.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Закрывает сеанс, использующий кэш для доступа к данным в этом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). параметры доступа к данным |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


Преобразует стиль ссылок в формуле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Формула для преобразования. |
| toR1C1 | boolean | Стиль ссылки, в который следует преобразовать формулу. Если исходная формула использует стиль ссылки A1, то это значение должно быть true, чтобы формула была преобразована из A1 в R1C1; если исходная формула использует стиль ссылки R1C1, то это значение должно быть false, чтобы формула была преобразована из R1C1 в A1; |
| baseCellRow | int | Индекс строки базовой ячейки. |
| baseCellColumn | int | Индекс столбца базовой ячейки. |

**Returns:**
java.lang.String - Преобразованная формула.
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


Копирует содержимое и форматы из другого листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Исходный лист. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


Копирует содержимое и форматы из другого листа.

**Remarks**

Вы можете копировать данные с другого листа в том же файле или из другого файла. Однако этот метод не поддерживает копирование графических объектов, таких как комментарии, изображения и диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Исходный лист. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

### dispose() {#dispose--}
```
public void dispose()
```


Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


Фильтрует диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Диапазон |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Замораживает области в указанной ячейке листа.

**Remarks**

Индекс строки и индекс столбца не могут одновременно быть нулевыми. Количество строк и количество столбцов также не могут одновременно быть нулевыми.

Первые два параметра задают позицию заморозки, а последние два параметра задают область, замороженную в левом верхнем окне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |
| freezedRows | int | Количество видимых строк в верхней панели, не более индекса строки. |
| freezedColumns | int | Количество видимых столбцов в левой панели, не более индекса столбца. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Замораживает области в указанной ячейке листа.

**Remarks**

Индекс строки и индекс столбца не могут одновременно быть нулевыми. Количество строк и количество столбцов также не могут одновременно быть нулевыми.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |
| freezedRows | int | Количество видимых строк в верхней панели, не более индекса строки. |
| freezedColumns | int | Количество видимых столбцов в левой панели, не более индекса столбца. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Получает активную ячейку в листе.

**Returns:**
java.lang.String
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


Получает настройки расширенного фильтра.

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


Получает все изображения, включая вложенные в ячейку и находящиеся над ячейками.

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


Получает коллекцию разрешённых диапазонов редактирования в листе.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


Запрашивает области ячеек, сопоставленные/связанные с конкретным путём XML‑карты.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | java.lang.String | путь к элементу xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Укажите xml‑карту, если вы хотите выполнить запрос конкретного пути внутри определённой карты |

**Returns:**
com.aspose.cells.CellArea[] - список [CellArea](../../com.aspose.cells/cellarea), сопоставленных/связанных с конкретным путём xml‑карты; если ничего не сопоставлено/связано, возвращается пустой список.
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Представляет автофильтр для указанного листа.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Получает фоновое изображение листа.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


Получает коллекцию ячеек на этом листе, наблюдаемых в ‘окне наблюдения’.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


Получает коллекцию [Cells](../../com.aspose.cells/cells).

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


Получает коллекцию [Chart](../../com.aspose.cells/chart)

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


Получает коллекцию [CheckBox](../../com.aspose.cells/checkbox).

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Получает кодовое имя листа.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


Получает коллекцию [Comment](../../com.aspose.cells/comment).

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


Получает ConditionalFormattings на листе.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


Получает объект, представляющий информацию об идентификаторе, связанную с листом.

**Remarks**

Worksheet.CustomProperties предоставляет предпочтительный механизм для хранения произвольных данных. Он поддерживает устаревшие сторонние компоненты документов, а также ситуации, требующие строгой необходимости в бинарных частях.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию — false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


True, если отображаются нулевые значения.

**Returns:**
boolean
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


Получает настройки проверки ошибок, применяемые к определённым диапазонам.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Представляет индекс первой видимой колонки.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Представляет индекс первой видимой строки.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Получает замороженные области.

**Returns:**
int[] - Возврат null означает, что лист не заморожен 0: индекс строки;1: столбец;2: замороженные строки;3: замороженные строки
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Получает цвет линий сетки

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


Получает коллекцию [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection).

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


Получает коллекцию [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection).

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Получает индекс листа в коллекции листов.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


Получает все ListObjects на этом листе.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


Получает имя листа.

**Remarks**

Максимальная длина имени листа — 31 символ. И вы не можете присвоить одинаковое имя (без учёта регистра) двум листам. Например, вы не можете установить "SheetName1" для первого листа и "SHEETNAME1" для второго листа.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


Представляет коллекцию [OleObject](../../com.aspose.cells/oleobject) на листе.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


Получает структуру на этом листе.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Представляет описание настройки страницы в этом листе.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


Указывает, имеет ли панель горизонтальные или вертикальные разбиения и заморожены ли они.

Смотрите [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


Получает оконные панели.

**Remarks**

Если окно не разделено и не заморожено.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


Получает коллекцию [Picture](../../com.aspose.cells/picture).

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


Получает все сводные таблицы в этом листе.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


Получает автоматические разрывы страниц.

**Remarks**

Каждая область ячейки представляет лист бумаги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Параметры печати |

**Returns:**
com.aspose.cells.CellArea[] - Области автоматических разрывов страниц.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


Представляет различные типы параметров защиты, доступные для листа. Поддерживает расширенные параметры защиты в ExcelXP и более новых версиях.

**Remarks**

Это свойство может защищать лист во всех версиях файлов Excel и поддерживает расширенные параметры защиты в ExcelXP и более новых версиях.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


Получает [QueryTableCollection](../../com.aspose.cells/querytablecollection) в листе.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


Получает коллекцию [Scenario](../../com.aspose.cells/scenario).

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


Получает выбранные диапазоны ячеек в дизайнерской таблице.

**Returns:**
com.aspose.cells.Range[] - Возвращает все выбранные диапазоны.
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


Получает выбранные диапазоны ячеек в дизайнерской таблице.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Worksheet.GetSelectedAreas(). Это свойство будет удалено через 12 месяцев, начиная с марта 2025 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
java.util.ArrayList - ArrayList, содержащий выбранные диапазоны.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Возвращает все графические объекты в этом листе.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


Указывает, показывать ли значки типов данных.

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


Указывает, показывать ли формулы или их результаты.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


Получить коллекцию Slicer в листе

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


Получает все объекты [SmartTagCollection](../../com.aspose.cells/smarttagcollection) листа.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


Получает группы спарклайнов в листе.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Представляет цвет вкладки листа.

**Remarks**

Эта функция поддерживается только в ExcelXP (Excel2002) и более поздних версиях. Если сохранить файл в формате Excel97 или Excel2000, она будет опущена.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


Указывает внутренний идентификатор листа.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


Получает коллекцию [TextBox](../../com.aspose.cells/textbox).

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


Получить коллекцию Timeline в листе

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


Указывает, включена ли опция Transition Formula Entry (совместимость с Lotus).

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


Указывает, включена ли опция Transition Formula Evaluation (совместимость с Lotus).

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Представляет тип листа.

Смотрите [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


Получает уникальный идентификатор, он такой же как \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


Получает коллекцию настроек проверки данных в листе.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


Получает коллекцию [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection).

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


Получает тип представления.

Смотрите [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


Указывает видимое состояние этого листа.

Смотрите [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Получает объект рабочей книги, содержащий этот лист.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Представляет коэффициент масштабирования в процентах. Должен находиться в диапазоне от 10 до 400.

**Remarks**

Пожалуйста, сначала установите тип представления.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


Указывает, имеет ли этот лист автофильтр.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Получает значение, указывающее, видимы ли линии сетки. По умолчанию true.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


Указывает, показывать ли контур.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Указывает, защищён ли лист.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


Возвращает значение, указывающее, будет ли лист отображать заголовки строк и столбцов. По умолчанию — true.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


Указывает, видима ли линейка. Это свойство применяется только в режиме предварительного просмотра разрывов страниц.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Указывает, будет ли этот лист выбран при открытии книги.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Представляет, видим ли лист.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Перемещает лист в другое место в таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс листа назначения. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


Защищает лист.

**Remarks**

Этот метод защищает лист без пароля. Он может защищать лист во всех версиях файлов Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Тип защиты. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


Защищает лист.

**Remarks**

Этот метод может защищать лист во всех версиях файлов Excel.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Тип защиты. |
| пароль | java.lang.String | Пароль. |
| oldPassword | java.lang.String | Если лист уже защищён паролем, пожалуйста, укажите старый пароль. В противном случае вы можете задать этому параметру значение null или пустую строку. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Обновляет все сводные таблицы в этом листе.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Обновляет все сводные таблицы в этом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Опция обновления источника данных сводной таблицы. |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


Удаляет все графические объекты в этом листе.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Удаляет автофильтр листа.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


Удаляет разделение окна.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


Заменяет текст всех ячеек новой строкой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| oldString | java.lang.String | Значение старой строки. |
| newString | java.lang.String | Значение новой строки. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


Выбирает диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка. |
| startColumn | int | Начальный столбец |
| totalRows | int | Количество строк. |
| totalColumns | int | Количество столбцов |
| removeOthers | boolean | True означает удаление других выбранных диапазонов и выбор только этого диапазона. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Устанавливает активную ячейку в листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Устанавливает фоновое изображение листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


Получает кодовое имя листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


True, если отображаются нулевые значения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Представляет индекс первой видимой колонки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Представляет индекс первой видимой строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Устанавливает цвет линий сетки

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Устанавливает значение, указывающее, видимы ли линии сетки. По умолчанию true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя листа.

**Remarks**

Максимальная длина имени листа — 31 символ. И вы не можете присвоить одинаковое имя (без учёта регистра) двум листам. Например, вы не можете установить "SheetName1" для первого листа и "SHEETNAME1" для второго листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Указывает, показывать ли контур.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


Устанавливает значение, указывающее, будет ли лист отображать заголовки строк и столбцов. По умолчанию true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


Указывает, видима ли линейка. Это свойство применяется только в режиме предварительного просмотра разрывов страниц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Указывает, будет ли этот лист выбран при открытии книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


Указывает, показывать ли значки типов данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


Указывает, показывать ли формулы или их результаты.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


Представляет цвет вкладки листа.

**Remarks**

Эта функция поддерживается только в ExcelXP (Excel2002) и более поздних версиях. Если сохранить файл в формате Excel97 или Excel2000, она будет опущена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


Указывает внутренний идентификатор листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


Указывает, включена ли опция Transition Formula Entry (совместимость с Lotus).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


Указывает, включена ли опция Transition Formula Evaluation (совместимость с Lotus).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Представляет тип листа.

Смотрите [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


Устанавливает уникальный идентификатор, он такой же, как \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


Устанавливает тип представления.

Смотрите [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


Указывает видимое состояние этого листа.

Смотрите [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Представляет, видим ли лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


Устанавливает видимые параметры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isVisible | boolean | Является ли лист видимым |
| ignoreError | boolean | Игнорировать ли ошибку, если эта опция недействительна. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Представляет коэффициент масштабирования в процентах. Должен находиться в диапазоне от 10 до 400.

**Remarks**

Пожалуйста, сначала установите тип представления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### split() {#split--}
```
public void split()
```


Разделяет окно.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Запускает сеанс, который использует кэш для доступа к данным в этом листе.

**Remarks**

После завершения доступа к данным следует вызвать [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-) с теми же параметрами, чтобы очистить все кэши и восстановить обычный режим доступа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). параметры доступа к данным |

### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий объект Worksheet.

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Размораживает области в листе.

### unprotect() {#unprotect--}
```
public void unprotect()
```


Снимает защиту с листа.

**Remarks**

Этот метод снимает защиту листа, который защищён без пароля.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Снимает защиту с листа.

**Remarks**

Если лист защищён без пароля, вы можете установить значение null или пустую строку в параметр password.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | java.lang.String | Пароль |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


Запрашивает области ячеек, сопоставленные/связанные с конкретным путём XML‑карты.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Worksheet.GetAreasOfXmlMapQuery(). Это свойство будет удалено через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | java.lang.String | путь к элементу xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Укажите xml‑карту, если вы хотите выполнить запрос конкретного пути внутри определённой карты |

**Returns:**
java.util.ArrayList - список [CellArea](../../com.aspose.cells/cellarea), сопоставленный/связанный с конкретным путём xml‑карты; если ничего не сопоставлено/связано, возвращается пустой список.
