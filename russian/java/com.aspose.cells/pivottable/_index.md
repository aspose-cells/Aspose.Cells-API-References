---
title: "Сводная таблица"
second_title: "Справочник API Aspose.Cells for Java"
description: "Краткое описание для PivotTable."
type: docs
url: /ru/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

Краткое описание для PivotTable.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | Добавляет вычисляемое поле к полю сводной таблицы и перетаскивает его в область данных. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | Добавляет вычисляемое поле к полю сводной таблицы. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | Добавляет поле в определённую область. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Добавляет поле в определённую область. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Добавляет поле в определённую область. |
| [calculateData()](#calculateData--) | Вычисляет данные сводной таблицы в ячейки. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | Вычисляет сводную таблицу с параметрами. |
| [calculateRange()](#calculateRange--) | Вычисляет диапазон сводной таблицы. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | Изменить источник данных сводной таблицы. |
| [clearAll()](#clearAll--) | Удалить все поля из областей. |
| [clearData()](#clearData--) | Очистить данные и форматирование представления сводной таблицы. |
| [clearFilters()](#clearFilters--) | Снимает все фильтры с этой сводной таблицы. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | Копирует именованный стиль из другой сводной таблицы. |
| [dispose()](#dispose--) | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | Экспортирует представление сводной таблицы в формате JSON. |
| [fields(int fieldType)](#fields-int-) | Получает конкретные поля по типу поля. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Форматирует выбранную область сводной таблицы. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Форматирует выбранную область сводной таблицы. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Форматирует ячейку в области сводной таблицы |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | Форматирует все ячейки в области сводной таблицы |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | Форматирует данные строк в области сводной таблицы |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров. |
| [getAltTextDescription()](#getAltTextDescription--) | Получает описание альтернативного текста. |
| [getAltTextTitle()](#getAltTextTitle--) | Получает заголовок изменённого текста. |
| [getAutoFormatType()](#getAutoFormatType--) | Получает тип автоматического форматирования сводной таблицы. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | Указывает, следует ли автоматически подгонять ширину столбца при обновлении |
| [getBaseFields()](#getBaseFields--) | Возвращает все базовые поля сводной таблицы. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | Получает область, содержащую кнопку поля. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | Получает объект [Cell](../../com.aspose.cells/cell) по отображаемому имени PivotField. |
| [getChildren()](#getChildren--) | Получает дочерние сводные таблицы, использующие данные этой сводной таблицы в качестве источника данных. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | Возвращает объект PivotFields, который в данный момент отображается как столбцовые поля. |
| [getColumnGrand()](#getColumnGrand--) | Указывает, отображает ли отчёт сводной таблицы общие итоги по столбцам. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | Получает пользовательскую подпись заголовка столбца сводной таблицы. |
| [getColumnRange()](#getColumnRange--) | Возвращает объект CellArea, представляющий диапазон, содержащий область столбцов в отчёте сводной таблицы. |
| [getConditionalFormats()](#getConditionalFormats--) | Получает условные форматы сводной таблицы. |
| [getCustomListSort()](#getCustomListSort--) | Указывает, следует ли учитывать встроенный пользовательский список при сортировке данных |
| [getDataBodyRange()](#getDataBodyRange--) | Возвращает объект [CellArea](../../com.aspose.cells/cellarea), представляющий диапазон, содержащий область данных в списке между строкой заголовка и строкой вставки. |
| [getDataField()](#getDataField--) | Получает объект [PivotField](../../com.aspose.cells/pivotfield), представляющий все поля данных в сводной таблице. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | Получает имя заголовка поля области значений в сводной таблице. |
| [getDataFields()](#getDataFields--) | Получает [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection), представляющую все поля данных в сводной таблице. |
| [getDataSource()](#getDataSource--) | Получает источник данных сводной таблицы. |
| [getDependentPivotTables()](#getDependentPivotTables--) | Получает все [PivotTable](../../com.aspose.cells/pivottable), использующие эту сводную таблицу в качестве источника данных. |
| [getDisplayErrorString()](#getDisplayErrorString--) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих ошибки. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | Указывает, видимы ли элементы в областях строк и столбцов, когда область данных сводной таблицы пуста. |
| [getDisplayNullString()](#getDisplayNullString--) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку, если значение равно null. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | Указывает логическое значение, определяющее, разрешено ли пользователю редактировать ячейки в области данных сводной таблицы. |
| [getEnableDrilldown()](#getEnableDrilldown--) | Указывает, включено ли углубление. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | Указывает, доступен ли диалоговое окно полей сводной таблицы при двойном щелчке пользователя по полю сводной таблицы. |
| [getEnableFieldList()](#getEnableFieldList--) | Указывает, доступен ли список полей для сводной таблицы в представлении Excel. |
| [getEnableWizard()](#getEnableWizard--) | Указывает, доступен ли мастер сводных таблиц. |
| [getErrorString()](#getErrorString--) | Получает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString равно true. Значение по умолчанию — пустая строка. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | Получает внешний источник данных соединения. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | Указывает, отсортированы ли поля в сводной таблице в порядке, отличном от стандартного, в списке полей. |
| [getFields(int fieldType)](#getFields-int-) | Получает конкретный список полей сводной таблицы по региону. |
| [getFilterArea()](#getFilterArea--) | Получает область региона фильтра. |
| [getGrandTotalName()](#getGrandTotalName--) | Возвращает метку, отображаемую в заголовке столбца или строки общей суммы. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | Получает список индексов строк сводной таблицы горизонтальных разрывов страниц. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Получает горизонтальные разрывы страниц этой сводной таблицы. |
| [getIndent()](#getIndent--) | Указывает шаг отступа для компактной оси и может использоваться для установки макета отчета в компактную форму. |
| [getItemPrintTitles()](#getItemPrintTitles--) | Указывает, должны ли имена PivotItem повторяться в верхней части каждой печатной страницы. |
| [getManualUpdate()](#getManualUpdate--) | Указывает, пересчитывается ли отчет сводной таблицы только по запросу пользователя. |
| [getMergeLabels()](#getMergeLabels--) | Получает, следует ли объединять метки полей строк/столбцов, охватывающие несколько ячеек. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров. |
| [getName()](#getName--) | Получает имя сводной таблицы |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | Получает имена внешних соединений источников данных. |
| [getNullString()](#getNullString--) | Получает строку, отображаемую в ячейках, содержащих значения null, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка. |
| [getPageFieldOrder()](#getPageFieldOrder--) | Получает порядок, в котором поля страниц добавляются в макет отчёта сводной таблицы. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | Получает количество полей страниц в каждом столбце или строке отчёта сводной таблицы. |
| [getPageFields()](#getPageFields--) | Возвращает [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection), которые в настоящее время отображаются как поля страниц. |
| [getPivotCache()](#getPivotCache--) | Получает источник данных. |
| [getPivotFilters()](#getPivotFilters--) | Возвращает все фильтры в сводной таблице. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | Получает условия форматирования сводной таблицы. |
| [getPivotFormats()](#getPivotFormats--) | Получает все форматы ячеек, применённые к этой сводной таблице. |
| [getPivotTableStyle()](#getPivotTableStyle--) | Получает настройки [TableStyle](../../com.aspose.cells/tablestyle) этой сводной таблицы. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | Получает название стиля сводной таблицы. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | Получает встроенный стиль сводной таблицы. |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | Получает все сводные таблицы с тем же кэшем сводных данных. |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | Указывает, следует ли сохранять форматирование ячеек ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) при обновлении или пересчёте сводной таблицы. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Указывает, сохраняется ли форматирование ячеек ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) при обновлении или пересчёте сводной таблицы. |
| [getPrintDrill()](#getPrintDrill--) | Указывает логическое значение, определяющее, следует ли печатать индикаторы детализации. |
| [getPrintTitles()](#getPrintTitles--) | Указывает, устанавливаются ли заголовки печати листа на основе отчёта сводной таблицы. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | Указывает, следует ли обновлять данные при открытии файла. |
| [getRefreshDate()](#getRefreshDate--) | Получает дату и время последнего обновления сводной таблицы. |
| [getRefreshedByWho()](#getRefreshedByWho--) | Получает имя последнего пользователя, обновившего эту сводную таблицу. |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | Указывает, повторяются ли подписи элементов сводной таблицы в области строк на каждой печатной странице для полей сводной таблицы в табличной форме. |
| [getRowFields()](#getRowFields--) | Возвращает [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection), которые в настоящее время отображаются как поля строк. |
| [getRowGrand()](#getRowGrand--) | Указывает, следует ли показывать общие итоги для строк этой сводной таблицы. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | Получает пользовательскую подпись заголовка строки в этой сводной таблице. |
| [getRowRange()](#getRowRange--) | Возвращает объект CellArea, представляющий диапазон, содержащий область строк в отчёте сводной таблицы. |
| [getSaveData()](#getSaveData--) | Указывает, сохраняются ли данные отчёта сводной таблицы вместе с книгой. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | Указывает, показывать ли общие итоги для столбцов этой сводной таблицы. |
| [getShowDataTips()](#getShowDataTips--) | Указывает, следует ли отображать подсказки для ячеек данных сводной таблицы. |
| [getShowDrill()](#getShowDrill--) | Получает, отображаются ли кнопки expand/collapse. |
| [getShowEmptyCol()](#getShowEmptyCol--) | Указывает, включать ли пустые столбцы в таблицу |
| [getShowEmptyRow()](#getShowEmptyRow--) | Указывает, включать ли пустые строки в таблицу. |
| [getShowHeaders()](#getShowHeaders--) | Показывать ли подписи полей данных и подписи полей сводной таблицы по оси строк и оси столбцов в представлении сводной таблицы. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | Указывает логическое значение, определяющее, следует ли опустить информацию о свойствах членов из подсказок сводной таблицы. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | Указывает, следует ли применять стиль к заголовку столбца в сводной таблице. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | Указывает, применяется ли чередующееся форматирование к столбцу. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | Указывает, применяется ли форматирование столбца. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | Указывает, следует ли применять стиль к заголовку строки в сводной таблице. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | Указывает, применяется ли чередующееся форматирование строк. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | Указывает, показывать ли общие итоги для строк сводной таблицы. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | Указывает, отображается ли подпись заголовка строки в отчёте сводной таблицы Указывает, отображать ли подписи полей отображения и выпадающие списки фильтров |
| [getShowValuesRow()](#getShowValuesRow--) | Указывает, отображать ли строку значений. |
| [getSource()](#getSource--) | Получить источник данных этой сводной таблицы. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | Получить источник данных этой сводной таблицы. |
| [getSourceDataConnections()](#getSourceDataConnections--) | Получает внешние источники данных соединения. |
| [getSourceType()](#getSourceType--) | Получает тип источника данных сводной таблицы. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | Указывает, включаются ли скрытые элементы полей страниц в отчёте сводной таблицы в промежуточные итоги по строкам и столбцам, блоковые итоги и общие итоги. |
| [getTableRange1()](#getTableRange1--) | Возвращает объект CellArea, представляющий диапазон, содержащий весь отчёт сводной таблицы, но без полей страниц. |
| [getTableRange2()](#getTableRange2--) | Возвращает объект CellArea, представляющий диапазон, содержащий весь отчёт сводной таблицы, включая поля страниц. |
| [getTag()](#getTag--) | Получает пользовательскую строку, связанную с этим представлением сводной таблицы. |
| [getTopRightArea()](#getTopRightArea--) | Представляет пустую область в правом верхнем углу сводной таблицы (в левом верхнем для листов RTL). |
| [getValuesField()](#getValuesField--) | Получает объект [PivotField](../../com.aspose.cells/pivotfield), представляющий все поля данных в сводной таблице. |
| [hasBlankRows()](#hasBlankRows--) | Указывает, добавлять ли пустые строки. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | Указывает, автоматически ли форматируется отчёт сводной таблицы. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | Указывает, совместима ли сводная таблица с Excel2003 при обновлении. Если значение true, строка должна быть длиной не более 255 символов, поэтому если строка превышает 255 символов, она будет усечена. Если значение false, строка не будет иметь указанного ограничения. |
| [isGridDropZones()](#isGridDropZones--) | Указывает, отображает ли отчёт сводной таблицы классический макет сводной таблицы. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров. |
| [isSelected()](#isSelected--) | Указывает, выбрана ли эта сводная таблица. |
| [move(int row, int column)](#move-int-int-) | Перемещает сводную таблицу в другое место листа. |
| [move(String destCellName)](#move-java.lang.String-) | Перемещает сводную таблицу в другое место листа. |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | Переместить один элемент вверх или вниз. |
| [moveTo(int row, int column)](#moveTo-int-int-) | Перемещает сводную таблицу в другое место листа. |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | Перемещает сводную таблицу в другое место листа. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | Перемещает сводную таблицу в другое место листа. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Обновить [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) из источника данных и вычислить данные и стиль для представления сводной таблицы. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Обновить [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) из источника данных и вычислить данные и стиль для представления сводной таблицы. |
| [refreshData()](#refreshData--) | Обновляет данные из его источника данных в кэш сводной таблицы. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | Обновляет данные и настройки сводной таблицы из её источника данных с параметрами. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | Удалить поле из определённой области полей |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | Удаляет поле из определённого региона сводной таблицы. |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | Удаляет поле из определённой области полей. |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | Выбрать область представления сводной таблицы. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | Получает описание альтернативного текста. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | Устанавливает заголовок альтернативного текста. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | Указывает, автоматически ли форматируется отчёт сводной таблицы. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | Устанавливает тип автоматического форматирования сводной таблицы. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | Указывает, следует ли автоматически подгонять ширину столбца при обновлении |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | Указывает, отображает ли отчёт сводной таблицы общие итоги по столбцам. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | Устанавливает пользовательскую подпись заголовка столбца сводной таблицы. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | Указывает, следует ли учитывать встроенный пользовательский список при сортировке данных |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | Устанавливает имя заголовка поля области значений в сводной таблице. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | Устанавливает источник данных сводной таблицы. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих ошибки. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | Указывает, видимы ли элементы в областях строк и столбцов, когда область данных сводной таблицы пуста. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | Указывает, отображает ли отчет сводной таблицы пользовательскую строку, если значение равно null. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | Указывает логическое значение, определяющее, разрешено ли пользователю редактировать ячейки в области данных сводной таблицы. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | Указывает, включено ли углубление. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | Указывает, доступен ли диалоговое окно полей сводной таблицы при двойном щелчке пользователя по полю сводной таблицы. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | Указывает, доступен ли список полей для сводной таблицы в представлении Excel. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | Указывает, доступен ли мастер сводных таблиц. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | Получает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString равно true. Значение по умолчанию — пустая строка. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | Указывает, совместима ли сводная таблица с Excel2003 при обновлении. Если значение true, строка должна быть длиной не более 255 символов, поэтому если строка превышает 255 символов, она будет усечена. Если значение false, строка не будет иметь указанного ограничения. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | Указывает, отсортированы ли поля в сводной таблице в порядке, отличном от стандартного, в списке полей. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | Возвращает метку, отображаемую в заголовке столбца или строки общей суммы. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | Указывает, отображает ли отчёт сводной таблицы классический макет сводной таблицы. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | Указывает, добавлять ли пустые строки. |
| [setIndent(int value)](#setIndent-int-) | Указывает шаг отступа для компактной оси и может использоваться для установки макета отчета в компактную форму. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | Указывает, должны ли имена PivotItem повторяться в верхней части каждой печатной страницы. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | Указывает, пересчитывается ли отчет сводной таблицы только по запросу пользователя. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | Устанавливает, следует ли объединять метки полей строк/столбцов, охватывающие несколько ячеек. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров. |
| [setName(String value)](#setName-java.lang.String-) | Получает имя сводной таблицы |
| [setNullString(String value)](#setNullString-java.lang.String-) | Получает строку, отображаемую в ячейках, содержащих значения null, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | Устанавливает порядок, в котором поля страниц добавляются в макет отчёта сводной таблицы. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | Получает количество полей страниц в каждом столбце или строке отчёта сводной таблицы. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | Получает настройки [TableStyle](../../com.aspose.cells/tablestyle) этой сводной таблицы. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | Устанавливает имя стиля сводной таблицы. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | Устанавливает встроенный стиль сводной таблицы. |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | Указывает, следует ли сохранять форматирование ячеек ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) при обновлении или пересчёте сводной таблицы. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Указывает, сохраняется ли форматирование ячеек ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) при обновлении или пересчёте сводной таблицы. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | Указывает логическое значение, определяющее, следует ли печатать индикаторы детализации. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | Указывает, устанавливаются ли заголовки печати листа на основе отчёта сводной таблицы. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | Указывает, следует ли обновлять данные при открытии файла. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | Указывает, повторяются ли подписи элементов сводной таблицы в области строк на каждой печатной странице для полей сводной таблицы в табличной форме. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | Указывает, следует ли показывать общие итоги для строк этой сводной таблицы. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | Устанавливает пользовательскую подпись заголовка строки в этой сводной таблице. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Указывает, сохраняются ли данные отчёта сводной таблицы вместе с книгой. |
| [setSelected(boolean value)](#setSelected-boolean-) | Указывает, выбрана ли эта сводная таблица. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | Указывает, показывать ли общие итоги для столбцов этой сводной таблицы. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | Указывает, следует ли отображать подсказки для ячеек данных сводной таблицы. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | Устанавливает, показывать ли кнопки развертывания/сворачивания. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | Указывает, включать ли пустые столбцы в таблицу |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | Указывает, включать ли пустые строки в таблицу. |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | Показывать ли подписи полей данных и подписи полей сводной таблицы по оси строк и оси столбцов в представлении сводной таблицы. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | Указывает логическое значение, определяющее, следует ли опустить информацию о свойствах членов из подсказок сводной таблицы. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | Указывает, следует ли применять стиль к заголовку столбца в сводной таблице. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | Указывает, применяется ли чередующееся форматирование к столбцу. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | Указывает, применяется ли форматирование столбца. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | Указывает, следует ли применять стиль к заголовку строки в сводной таблице. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | Указывает, применяется ли чередующееся форматирование строк. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | Указывает, показывать ли общие итоги для строк сводной таблицы. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | Указывает, отображается ли подпись заголовка строки в отчёте сводной таблицы Указывает, отображать ли подписи полей отображения и выпадающие списки фильтров |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | Указывает, отображать ли строку значений. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | Указывает, включаются ли скрытые элементы полей страниц в отчёте сводной таблицы в промежуточные итоги по строкам и столбцам, блоковые итоги и общие итоги. |
| [setTag(String value)](#setTag-java.lang.String-) | Устанавливает пользовательскую строку, связанную с этим представлением сводной таблицы. |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | Показать детали одного элемента в области данных в новой таблице. |
| [showInCompactForm()](#showInCompactForm--) | Отображает представление сводной таблицы в компактной форме. |
| [showInOutlineForm()](#showInOutlineForm--) | Отображает сводную таблицу в виде схемы. |
| [showInTabularForm()](#showInTabularForm--) | Отображает сводную таблицу в табличной форме. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | Показать все страницы фильтра отчёта в соответствии с PivotField, PivotField должен находиться в PageFields. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | Показать все страницы фильтра отчёта в соответствии с индексом позиции в PageFields. |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | Показать все страницы фильтра отчёта в соответствии с именем PivotField, PivotField должен находиться в PageFields. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


Добавляет вычисляемое поле к полю сводной таблицы и перетаскивает его в область данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя вычисляемого поля |
| formula | java.lang.String | Формула вычисляемого поля. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


Добавляет вычисляемое поле к полю сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя вычисляемого поля |
| formula | java.lang.String | Формула вычисляемого поля. |
| dragToDataArea | boolean | True, перетащите это поле в область данных немедленно |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


Добавляет поле в определённую область.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). тип области полей. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | поле в базовых полях. |

**Returns:**
int — позиция поля в конкретных полях.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Добавляет поле в определённую область.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области полей. |
| baseFieldIndex | int | Индекс в базовых полях. |

**Returns:**
int — позиция поля в конкретных полях.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Добавляет поле в определённую область.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области полей. |
| fieldName | java.lang.String | Имя в базовых полях. |

**Returns:**
int — позиция поля в конкретных полях. Если поле с таким именем отсутствует, вернуть -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Вычисляет данные сводной таблицы в ячейки.

**Remarks**

Этот метод вычисляет данные только с кэшированными данными в [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). Поэтому, если вы хотите вычислить с последним источником данных, пожалуйста, используйте метод [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) для вычисления. Если изменены только настройки сводной таблицы, достаточно вызвать [calculateData()](../../com.aspose.cells/pivottable\#calculateData--).

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


Вычисляет сводную таблицу с параметрами.

**Remarks**

Если [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) равно true, этот метод обновит кэш сводных таблиц из источника данных, затем вычислит все сводные таблицы, основанные на том же кэше. В противном случае будет производиться вычисление только с кэшированными данными в кэше.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | Параметры вычисления сводной таблицы |

**Returns:**
com.aspose.cells.PivotTable[] - Возвращает все сводные таблицы, которые были вычислены. Если [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) равно true, все сводные таблицы, основанные на одном и том же кэше, будут вычислены вместе.
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


Вычисляет диапазон сводной таблицы.

**Remarks**

Если этот метод не был вызван, возможно диапазон сводной таблицы некорректен.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


Изменить источник данных сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


Удалить все поля из областей.

### clearData() {#clearData--}
```
public void clearData()
```


Очистить данные и форматирование представления сводной таблицы.

**Remarks**

Если этот метод не будет вызван до того, как вы добавляете или удаляете PivotField, возможно, данные PivotTable некорректны

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


Снимает все фильтры с этой сводной таблицы.

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


Копирует именованный стиль из другой сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Исходная сводная таблица. |

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
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


Экспортирует представление сводной таблицы в формате JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


Получает конкретные поля по типу поля.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод PivotField.GetFields(PivotFieldType). Этот метод будет удалён через 12 месяцев, начиная с мая 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). тип поля. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Форматирует выбранную область сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Диапазон ячеек. |
| style | [Style](../../com.aspose.cells/style) | Стиль |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Форматирует выбранную область сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | Выбранная область представления сводной таблицы. |
| style | [Style](../../com.aspose.cells/style) | Форматированная настройка. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Форматирует ячейку в области сводной таблицы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки ячейки |
| столбец | int | Индекс столбца ячейки |
| style | [Style](../../com.aspose.cells/style) | Стиль, используемый для форматирования ячейки |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


Форматирует все ячейки в области сводной таблицы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Стиль, используемый для форматирования |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


Форматирует данные строк в области сводной таблицы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки объекта Row |
| style | [Style](../../com.aspose.cells/style) | Стиль, используемый для форматирования |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


Получает описание альтернативного текста.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


Получает заголовок изменённого текста.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


Получает тип автоматического форматирования сводной таблицы.

Смотрите [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


Указывает, следует ли автоматически подгонять ширину столбца при обновлении

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


Возвращает все базовые поля сводной таблицы.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


Получает область, содержащую кнопку поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


Получает объект [Cell](../../com.aspose.cells/cell) по отображаемому имени PivotField.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| displayName | java.lang.String | DisplayName поля PivotField |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


Получает дочерние сводные таблицы, использующие данные этой сводной таблицы в качестве источника данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод PivotTable.GetDependentPivotTables(). Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
com.aspose.cells.PivotTable[] - объект массива PivotTable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


Возвращает объект PivotFields, который в данный момент отображается как столбцовые поля.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


Указывает, отображает ли отчёт сводной таблицы общие итоги по столбцам.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotTable.ShowColumnGrandTotals. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


Получает пользовательскую подпись заголовка столбца сводной таблицы.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


Возвращает объект CellArea, представляющий диапазон, содержащий область столбцов в отчёте PivotTable. Только для чтения.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


Получает условные форматы сводной таблицы.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


Указывает, следует ли учитывать встроенный пользовательский список при сортировке данных

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


Возвращает объект [CellArea](../../com.aspose.cells/cellarea), представляющий диапазон, содержащий область данных в списке между строкой заголовка и строкой вставки. Только для чтения.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


Получает объект [PivotField](../../com.aspose.cells/pivotfield), представляющий все поля данных в сводной таблице. Только для чтения. Он будет создан только тогда, когда в области данных присутствует два или более полей данных. По умолчанию он находится в области строк. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea().

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте свойство PivotTable.ValuesField. Этот метод будет удалён через 12 месяцев, начиная с октября 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


Получает имя заголовка поля области значений в сводной таблице.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


Получает [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection), представляющую все поля данных в сводной таблице.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


Получает источник данных сводной таблицы.

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


Получает все [PivotTable](../../com.aspose.cells/pivottable), использующие эту сводную таблицу в качестве источника данных.

**Remarks**

Поскольку сводные таблицы могут зависеть друг от друга, их необходимо обновлять в правильном порядке, чтобы обеспечить согласованность данных.

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих ошибки.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


Указывает, видимы ли элементы в областях строк и столбцов, когда область данных сводной таблицы пуста. Значение по умолчанию — true.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


Указывает, отображает ли отчет сводной таблицы пользовательскую строку, если значение равно null.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


Указывает логическое значение, которое определяет, разрешено ли пользователю редактировать ячейки в области данных сводной таблицы. Значение по умолчанию — false.

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


Указывает, включено ли углубление.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


Указывает, доступен ли диалоговое окно полей сводной таблицы при двойном щелчке пользователя по полю сводной таблицы.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


Указывает, доступен ли список полей для сводной таблицы в представлении Excel.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


Указывает, доступен ли мастер сводных таблиц.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


Получает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString равно true. Значение по умолчанию — пустая строка.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


Получает внешний источник данных соединения.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotTable.GetSourceDataConnections(). Этот метод будет удалён через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


Указывает, отсортированы ли поля в сводной таблице в порядке, отличном от стандартного, в списке полей.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


Получает конкретный список полей сводной таблицы по региону.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). тип региона. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


Получает область региона фильтра.

**Remarks**

Действительно только если существуют фильтрующие поля сводной таблицы. Пустая область будет возвращена, если эта сводная таблица не содержит фильтрующих полей.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


Возвращает метку, отображаемую в заголовке столбца или строки итогов. Значение по умолчанию — строка "Grand Total".

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


Получает список индексов строк сводной таблицы горизонтальных разрывов страниц.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод PivotTable.GetHorizontalPageBreaks(). Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


Получает горизонтальные разрывы страниц этой сводной таблицы.

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


Указывает шаг отступа для компактной оси и может использоваться для установки макета отчета в компактную форму.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


Указывает, должны ли имена PivotItem повторяться в верхней части каждой печатной страницы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.RepeatItemsOnEachPrintedPage. Этот метод будет удалён через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


Указывает, пересчитывается ли отчет сводной таблицы только по запросу пользователя.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


Получает, следует ли объединять метки полей строк/столбцов, охватывающие несколько ячеек.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров.

См. [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotCache.MissingItemsLimit. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Получает имя сводной таблицы

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


Получает имена внешних соединений источников данных.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


Получает строку, отображаемую в ячейках, содержащих значения null, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


Получает порядок, в котором поля страниц добавляются в макет отчёта сводной таблицы.

См. [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


Получает количество полей страниц в каждом столбце или строке отчёта сводной таблицы.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


Возвращает [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection), которые в настоящее время отображаются как поля страниц.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


Получает источник данных.

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


Возвращает все фильтры в сводной таблице.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


Получает условия форматирования сводной таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.ConditionalFormats. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


Получает все форматы ячеек, применённые к этой сводной таблице.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


Получает настройки [TableStyle](../../com.aspose.cells/tablestyle) этой сводной таблицы.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


Получает название стиля сводной таблицы.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


Получает встроенный стиль сводной таблицы.

См. [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


Получает все сводные таблицы с тем же кэшем сводных данных.

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


Указывает, следует ли сохранять форматирование ячеек ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) при обновлении или пересчёте сводной таблицы.

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Указывает, сохраняется ли форматирование ячеек ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) при обновлении или пересчёте сводной таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.PreserveCellFormattingOnUpdate. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


Указывает логическое значение, определяющее, должны ли индикаторы drill выводиться на печать. Печать кнопок раскрытия/сворачивания при отображении в сводной таблице.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


Указывает, устанавливаются ли заголовки печати листа на основе отчёта сводной таблицы. Значение по умолчанию — false.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


Указывает, следует ли обновлять данные при открытии файла.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


Получает дату и время последнего обновления сводной таблицы.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


Получает имя последнего пользователя, обновившего эту сводную таблицу.

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


Указывает, повторяются ли подписи элементов сводной таблицы в области строк на каждой печатной странице для полей сводной таблицы в табличной форме.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


Возвращает [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection), которые в настоящее время отображаются как поля строк.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


Указывает, следует ли показывать общие итоги для строк этой сводной таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotTable.ShowRowGrandTotals. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


Получает пользовательскую подпись заголовка строки в этой сводной таблице.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


Возвращает объект CellArea, представляющий диапазон, содержащий область строк в отчёте сводной таблицы. Только для чтения.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Указывает, сохраняются ли данные отчёта сводной таблицы вместе с книгой.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


Указывает, показывать ли общие итоги для столбцов этой сводной таблицы.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


Указывает, следует ли отображать подсказки для ячеек данных сводной таблицы.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


Получает, отображаются ли кнопки expand/collapse.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


Указывает, включать ли пустые столбцы в таблицу

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


Указывает, включать ли пустые строки в таблицу.

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


Показывать ли подписи полей данных и подписи полей сводной таблицы по оси строк и оси столбцов в представлении сводной таблицы.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


Указывает логическое значение, определяющее, следует ли опустить информацию о свойствах членов из подсказок сводной таблицы.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


Указывает, следует ли применять стиль к заголовку столбца в сводной таблице.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


Указывает, применяется ли чередующееся форматирование к столбцу.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


Указывает, применяется ли форматирование столбца.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


Указывает, следует ли применять стиль к заголовку строки в сводной таблице.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


Указывает, применяется ли чередующееся форматирование строк.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


Указывает, показывать ли общие итоги для строк сводной таблицы.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


Указывает, отображается ли подпись заголовка строки в отчёте сводной таблицы Указывает, отображать ли подписи полей отображения и выпадающие списки фильтров

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.ShowHeaders. Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


Указывает, отображать ли строку значений.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


Получить источник данных этой сводной таблицы.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


Получить источник данных этой сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isOriginal | boolean | Указывает, возвращать оригинальный или отображаемый источник данных. |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


Получает внешние источники данных соединения.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


Получает тип источника данных сводной таблицы.

См. [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


Указывает, включаются ли скрытые элементы полей страниц в отчёте сводной таблицы в промежуточные итоги строк и столбцов, блоковые итоги и общие итоги. Значение по умолчанию — False.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет PivotTable, но не включающий поля страниц. Только для чтения.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет PivotTable, включая поля страниц. Только для чтения.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


Получает пользовательскую строку, связанную с этим представлением сводной таблицы.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


Представляет пустую область в правом верхнем углу сводной таблицы (в левом верхнем для листов RTL).

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


Получает объект [PivotField](../../com.aspose.cells/pivotfield), представляющий все поля данных в сводной таблице. Только для чтения. Он будет создан только тогда, когда в области данных присутствует два или более полей данных. По умолчанию он находится в области строк. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea().

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


Указывает, следует ли добавлять пустые строки. Это свойство применяется только к типам автоформатирования PivotTable, которым необходимо добавлять пустые строки.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.InsertBlankRow. Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose просит прощения за любые неудобства, которые могли возникнуть.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


Указывает, автоматически ли форматируется отчет PivotTable. Флажок "autoformat table", который находится в параметрах pivottable для Excel 2003.

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


Указывает, совместима ли PivotTable с Excel2003 при обновлении PivotTable; если значение true, строка должна быть длиной не более 255 символов, поэтому строки длиннее 255 символов будут усечены. Если значение false, на строку не будет наложено указанное ограничение. Значение по умолчанию — true.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


Указывает, отображает ли отчет PivotTable классический макет pivottable. (включает перетаскивание полей в сетке)

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.AllowMultipleFiltersPerField. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose просит прощения за любые неудобства, которые могли возникнуть.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Указывает, выбрана ли эта сводная таблица.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


Перемещает сводную таблицу в другое место листа.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotTable.MoveTo(). Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose просит прощения за любые неудобства, которые могли возникнуть.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | индекс строки. |
| столбец | int | индекс столбца. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


Перемещает сводную таблицу в другое место листа.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotTable.MoveTo(). Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose просит прощения за любые неудобства, которые могли возникнуть.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destCellName | java.lang.String | имя целевой ячейки. |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


Переместить один элемент вверх или вниз.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Регион. Только для строки или столбца. |
| узлы | java.lang.String[] | Элемент. |
| абсолютный | boolean | Указывает, является ли смещение абсолютной позицией. |
| смещение | int | Если absolute равно true: 0 перемещает в начало, -1 перемещает в конец, остальные значения означают абсолютную позицию; иначе смещение является относительным. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


Перемещает сводную таблицу в другое место листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | индекс строки. |
| столбец | int | индекс столбца. |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


Перемещает сводную таблицу в другое место листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | индекс целевого листа |
| строка | int | индекс строки. |
| столбец | int | индекс столбца. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


Перемещает сводную таблицу в другое место листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destCellName | java.lang.String | имя целевой ячейки. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int refresh()
```


Обновить [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) из источника данных и вычислить данные и стиль для представления сводной таблицы.

**Remarks**

Все сводные таблицы, зависящие от одного и того же PivotCache, будут пересчитаны.

**Returns:**
int — [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Обновить [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) из источника данных и вычислить данные и стиль для представления сводной таблицы.

**Remarks**

Все сводные таблицы, зависящие от одного и того же PivotCache, будут пересчитаны.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int — [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refreshData() {#refreshData--}
```
public int refreshData()
```


Обновляет данные из его источника данных в кэш сводной таблицы.

**Remarks**

Мы собираем данные из источника данных в кэш сводных таблиц, а затем вычисляем данные из кэша в ячейки. И лучше всего просто вызвать [Workbook.refreshAll()](../../com.aspose.cells/workbook\\#refreshAll--) , чтобы обновить и вычислить все сводные таблицы в файле, а не обновлять их по одной. ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод [PivotCache.refresh()](../../com.aspose.cells/pivotcache\\#refresh--) , а также удалите последующий [calculateData()](../../com.aspose.cells/pivottable\\#calculateData--) , поскольку эта сводная таблица будет вычислена при обновлении [getPivotCache()](../../com.aspose.cells/pivottable\\#getPivotCache--) . Этот метод будет удалён через 12 месяцев, начиная с июня 2026 года. Aspose просит прощения за любые неудобства, которые могли возникнуть.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


Обновляет данные и настройки сводной таблицы из её источника данных с параметрами.

**Remarks**

Мы собираем данные из источника данных в кэш сводных таблиц, а затем вычисляем данные из кэша в ячейки. И лучше всего просто вызвать [Workbook.refreshAll()](../../com.aspose.cells/workbook\\#refreshAll--) , чтобы обновить и вычислить все сводные таблицы в файле, а не обновлять их по одной. ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод [PivotCache.refresh()](../../com.aspose.cells/pivotcache\\#refresh--) , а также удалите последующий [calculateData()](../../com.aspose.cells/pivottable\\#calculateData--) , поскольку эта сводная таблица будет вычислена при обновлении [getPivotCache()](../../com.aspose.cells/pivottable\\#getPivotCache--) . Этот метод будет удалён через 12 месяцев, начиная с июня 2026 года. Aspose просит прощения за любые неудобства, которые могли возникнуть.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Параметры обновления источника данных сводной таблицы. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


Удалить поле из определённой области полей

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). тип области полей. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | поле в базовых полях. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


Удаляет поле из определённого региона сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области полей. |
| baseFieldIndex | int | Индекс поля в базовых полях. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


Удаляет поле из определённой области полей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области полей. |
| fieldName | java.lang.String | Имя в базовых полях. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


Выбрать область представления сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Область ячейки. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


Получает описание альтернативного текста.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


Устанавливает заголовок альтернативного текста.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


Указывает, автоматически ли форматируется отчет PivotTable. Флажок "autoformat table", который находится в параметрах pivottable для Excel 2003.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


Устанавливает тип автоматического форматирования сводной таблицы.

Смотрите [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


Указывает, следует ли автоматически подгонять ширину столбца при обновлении

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


Указывает, отображает ли отчёт сводной таблицы общие итоги по столбцам.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotTable.ShowColumnGrandTotals. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


Устанавливает пользовательскую подпись заголовка столбца сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


Указывает, следует ли учитывать встроенный пользовательский список при сортировке данных

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


Устанавливает имя заголовка поля области значений в сводной таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


Устанавливает источник данных сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


Указывает, отображает ли отчет сводной таблицы пользовательскую строку в ячейках, содержащих ошибки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


Указывает, видимы ли элементы в областях строк и столбцов, когда область данных сводной таблицы пуста. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


Указывает, отображает ли отчет сводной таблицы пользовательскую строку, если значение равно null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


Указывает логическое значение, которое определяет, разрешено ли пользователю редактировать ячейки в области данных сводной таблицы. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


Указывает, включено ли углубление.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


Указывает, доступен ли диалоговое окно полей сводной таблицы при двойном щелчке пользователя по полю сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


Указывает, доступен ли список полей для сводной таблицы в представлении Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


Указывает, доступен ли мастер сводных таблиц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


Получает строку, отображаемую в ячейках, содержащих ошибки, когда свойство DisplayErrorString равно true. Значение по умолчанию — пустая строка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


Указывает, совместима ли PivotTable с Excel2003 при обновлении PivotTable; если значение true, строка должна быть длиной не более 255 символов, поэтому строки длиннее 255 символов будут усечены. Если значение false, на строку не будет наложено указанное ограничение. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


Указывает, отсортированы ли поля в сводной таблице в порядке, отличном от стандартного, в списке полей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


Возвращает метку, отображаемую в заголовке столбца или строки итогов. Значение по умолчанию — строка "Grand Total".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


Указывает, отображает ли отчет PivotTable классический макет pivottable. (включает перетаскивание полей в сетке)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


Указывает, следует ли добавлять пустые строки. Это свойство применяется только к типам автоформатирования PivotTable, которым необходимо добавлять пустые строки.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.InsertBlankRow. Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose просит прощения за любые неудобства, которые могли возникнуть.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


Указывает шаг отступа для компактной оси и может использоваться для установки макета отчета в компактную форму.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


Указывает, должны ли имена PivotItem повторяться в верхней части каждой печатной страницы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.RepeatItemsOnEachPrintedPage. Этот метод будет удалён через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


Указывает, пересчитывается ли отчет сводной таблицы только по запросу пользователя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


Устанавливает, следует ли объединять метки полей строк/столбцов, охватывающие несколько ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров.

См. [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotCache.MissingItemsLimit. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


Указывает логическое значение, которое определяет, могут ли поля сводной таблицы иметь несколько установленных фильтров.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.AllowMultipleFiltersPerField. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose просит прощения за любые неудобства, которые могли возникнуть.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Получает имя сводной таблицы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


Получает строку, отображаемую в ячейках, содержащих значения null, когда свойство DisplayNullString равно true. Значение по умолчанию — пустая строка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


Устанавливает порядок, в котором поля страниц добавляются в макет отчёта сводной таблицы.

См. [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


Получает количество полей страниц в каждом столбце или строке отчёта сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


Получает настройки [TableStyle](../../com.aspose.cells/tablestyle) этой сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


Устанавливает имя стиля сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


Устанавливает встроенный стиль сводной таблицы.

См. [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


Указывает, следует ли сохранять форматирование ячеек ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) при обновлении или пересчёте сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Указывает, сохраняется ли форматирование ячеек ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) при обновлении или пересчёте сводной таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.PreserveCellFormattingOnUpdate. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


Указывает логическое значение, определяющее, должны ли индикаторы drill выводиться на печать. Печать кнопок раскрытия/сворачивания при отображении в сводной таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


Указывает, устанавливаются ли заголовки печати листа на основе отчёта сводной таблицы. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


Указывает, следует ли обновлять данные при открытии файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


Указывает, повторяются ли подписи элементов сводной таблицы в области строк на каждой печатной странице для полей сводной таблицы в табличной форме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


Указывает, следует ли показывать общие итоги для строк этой сводной таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotTable.ShowRowGrandTotals. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


Устанавливает пользовательскую подпись заголовка строки в этой сводной таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Указывает, сохраняются ли данные отчёта сводной таблицы вместе с книгой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Указывает, выбрана ли эта сводная таблица.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


Указывает, показывать ли общие итоги для столбцов этой сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


Указывает, следует ли отображать подсказки для ячеек данных сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


Устанавливает, показывать ли кнопки развертывания/сворачивания.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


Указывает, включать ли пустые столбцы в таблицу

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


Указывает, включать ли пустые строки в таблицу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


Показывать ли подписи полей данных и подписи полей сводной таблицы по оси строк и оси столбцов в представлении сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


Указывает логическое значение, определяющее, следует ли опустить информацию о свойствах членов из подсказок сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


Указывает, следует ли применять стиль к заголовку столбца в сводной таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


Указывает, применяется ли чередующееся форматирование к столбцу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


Указывает, применяется ли форматирование столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


Указывает, следует ли применять стиль к заголовку строки в сводной таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


Указывает, применяется ли чередующееся форматирование строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


Указывает, показывать ли общие итоги для строк сводной таблицы.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


Указывает, отображается ли подпись заголовка строки в отчёте сводной таблицы Указывает, отображать ли подписи полей отображения и выпадающие списки фильтров

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.ShowHeaders. Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


Указывает, отображать ли строку значений.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


Указывает, включаются ли скрытые элементы полей страниц в отчёте сводной таблицы в промежуточные итоги строк и столбцов, блоковые итоги и общие итоги. Значение по умолчанию — False.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


Устанавливает пользовательскую строку, связанную с этим представлением сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


Показать детали одного элемента в области данных в новой таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | Смещение до первой строки данных в области данных. |
| columnOffset | int | Смещение до первого столбца данных в области данных. |
| newSheet | boolean | Показать детали на новом листе. |
| destRow | int | Целевая строка. |
| destColumn | int | Целевой столбец. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


Отображает представление сводной таблицы в компактной форме.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


Отображает сводную таблицу в виде схемы.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


Отображает сводную таблицу в табличной форме.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


Показать все страницы фильтра отчёта в соответствии с PivotField, PivotField должен находиться в PageFields.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | Объект PivotField |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


Показать все страницы фильтра отчёта в соответствии с индексом позиции в PageFields.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| posIndex | int | Индекс позиции в PageFields |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


Показать все страницы фильтра отчёта в соответствии с именем PivotField, PivotField должен находиться в PageFields.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldName | java.lang.String | Имя PivotField |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

