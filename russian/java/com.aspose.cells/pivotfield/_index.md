---
title: "PivotField"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет поле в отчете сводной таблицы."
type: docs
url: /ru/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

Представляет поле в отчете сводной таблицы.

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
 
          pivot.calculateData(new PivotTableCalculateOption());
 
         //do your business
 
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Добавить вычисляемый элемент формулы в pivot field. |
| [clearFilter()](#clearFilter--) | Очищает настройки фильтра для этого pivot field. |
| [dispose()](#dispose--) | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Фильтрует по значениям даты в строковом или столбцовом pivot field. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | Фильтрует по подписьям строки или столбца сводного поля. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | Фильтрует по значениям данных сводного поля. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | Фильтрует по значениям данных сводного поля. |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | Указывает, можно ли перетаскивать указанное поле в область столбцов. |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | Указывает, можно ли перетаскивать указанное поле в область значений. |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | Указывает, можно ли перетаскивать указанное поле в область страниц. |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | Указывает, можно ли перетаскивать указанное поле в область строк. |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | Указывает, можно ли удалить это pivot field из представления PivotTable. |
| [getAutoShowCount()](#getAutoShowCount--) | Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы. |
| [getAutoShowField()](#getAutoShowField--) | Представляет индекс автоматически отображаемого поля. -1 означает сам PivotField. |
| [getAutoSortField()](#getAutoSortField--) | Представляет индекс поля, которое автоматически сортируется. |
| [getBaseIndex()](#getBaseIndex--) | Представляет индекс в исходных полях pivot. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Получить строку формулы указанного вычисляемого поля. |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Получает текущий отображаемый элемент страницы для этого pivot field (только поле страницы). |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | Получает отображаемый текст текущего элемента страницы для этого поля сводки (только поле страницы). |
| [getDisplayName()](#getDisplayName--) | Представляет отображаемое имя поля сводки в представлении сводной таблицы. |
| [getDragToColumn()](#getDragToColumn--) | Указывает, можно ли перетаскивать указанное поле в область столбцов. |
| [getDragToData()](#getDragToData--) | Указывает, можно ли перетаскивать указанное поле в область значений. |
| [getDragToHide()](#getDragToHide--) | Указывает, можно ли удалить это pivot field из представления PivotTable. |
| [getDragToPage()](#getDragToPage--) | Указывает, можно ли перетаскивать указанное поле в область страниц. |
| [getDragToRow()](#getDragToRow--) | Указывает, можно ли перетаскивать указанное поле в область строк. |
| [getFilters()](#getFilters--) | Получает все фильтры сводки, применённые к этому полю сводки. |
| [getFormula()](#getFormula--) | Получает формулу вычисляемого поля. |
| [getFunction()](#getFunction--) | Представляет функцию, используемую для суммирования этого поля данных сводной таблицы. |
| [getGroupSettings()](#getGroupSettings--) | Получает настройки группировки поля сводки. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Указывает, следует ли вставлять пустую строку после каждого элемента. |
| [getItemCount()](#getItemCount--) | Получает количество базовых элементов в этом поле сводки. |
| [getItems()](#getItems--) | Получить все метки элементов сводки в этом поле. |
| [getMaxValue()](#getMaxValue--) | Получает максимальное значение этого поля. |
| [getMinValue()](#getMinValue--) | Получает максимальное значение этого поля. |
| [getName()](#getName--) | Представляет имя PivotField. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Указывает, является ли операция сортировки, применяемая к этому полю сводки, автоматической сортировкой или простой сортировкой данных. |
| [getNumber()](#getNumber--) | Представляет встроенный формат отображения чисел и дат. |
| [getNumberFormat()](#getNumberFormat--) | Представляет пользовательский формат отображения чисел и дат. |
| [getOriginalItems()](#getOriginalItems--) | Получить оригинальные базовые элементы; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Получает фильтр сводки поля по типу |
| [getPivotFilters()](#getPivotFilters--) | Получает фильтры сводки поля |
| [getPivotItems()](#getPivotItems--) | Получает элементы сводки поля |
| [getPosition()](#getPosition--) | Представляет индекс [PivotField](../../com.aspose.cells/pivotfield) в области. |
| [getRegionType()](#getRegionType--) | Указывает область сводной таблицы, в которой отображается это поле. |
| [getShowAllItems()](#getShowAllItems--) | Указывает, следует ли отображать все элементы в представлении PivotTable, даже если они не содержат сводных данных. |
| [getShowCompact()](#getShowCompact--) | Указывает, следует ли отображать метки следующего поля в той же колонке в представлении Pivot Table. |
| [getShowInCompactForm()](#getShowInCompactForm--) | Получает значение, указывающее, использует ли это поле строки компактный макет. |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Получает значение, указывающее, использует ли это поле строки макет в виде контура. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | Указывает, следует ли отображать промежуточные итоги вверху или внизу элементов. |
| [getShowValuesSetting()](#getShowValuesSetting--) | Получает параметры отображения значений, когда используется вычисление ShowDataAs. |
| [getSortSetting()](#getSortSetting--) | Получает все параметры автоматической сортировки |
| [getSubtotals()](#getSubtotals--) | Получает промежуточные итоги поля. |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Указывает, следует ли показывать указанный промежуточный итог для этого поля сводной таблицы. |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | Получает параметры автоматического отображения Top 10 для поля сводной таблицы. |
| [group()](#group--) | Автоматически группировать поле. |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | Группирует поле сводной таблицы с параметрами. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | Группировать файл по типам группировки даты. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | Группировать файл по числу. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Пользовательская группировка поля. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Группировать файл по типам группировки даты. |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | Пользовательская группировка поля. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | Автоматически группировать поле с интервалом |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Группировать файл по числу. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | Автоматически группировать поле с internal |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | Скрывает все детали каждого элемента сводной таблицы. |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Устанавливает, скрыты ли детали всех PivotItems в поле сводной таблицы. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Устанавливает, скрыт ли конкретный PivotItem в поле данных. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Устанавливает, скрыт ли конкретный PivotItem в поле данных. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Устанавливает, скрыты ли детали конкретного PivotItem в поле сводной таблицы. |
| [initPivotItems()](#initPivotItems--) | Инициализировать элементы сводного поля. |
| [isAscendShow()](#isAscendShow--) | Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию. |
| [isAscendSort()](#isAscendSort--) | Указывает, сортируются ли элементы этого поля сводной таблицы автоматически по возрастанию. |
| [isAutoShow()](#isAutoShow--) | Указывает, отображается ли указанный поле PivotTable автоматически. |
| [isAutoSort()](#isAutoSort--) | Указывает, сортируются ли элементы этого поля PivotTable автоматически. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Указывает, показывает ли указанный поле автоматические промежуточные итоги. |
| [isCalculatedField()](#isCalculatedField--) | Указывает, является ли это поле сводной таблицы вычисляемым полем. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Указывает, скрыт ли конкретный PivotItem. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Указывает, скрывать ли детали конкретного PivotItem.. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | Указывает, включать ли новые элементы в поле при ручной фильтрации. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | Указывает, следует ли вставлять разрывы страниц после каждого элемента. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | Указывает, можно ли выбирать несколько элементов в поле страниц. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | Указывает, следует ли повторять метки поля в области строк или столбцов. |
| [isValueFields()](#isValueFields--) | Указывает, представляет ли это поле поля значений. |
| [isValuesField()](#isValuesField--) | Указывает, представляет ли это поле поле значений. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | Указывает, можно ли перетаскивать указанное поле в область столбцов. |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | Указывает, можно ли перетаскивать указанное поле в область значений. |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | Указывает, можно ли перетаскивать указанное поле в область страниц. |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | Указывает, можно ли перетаскивать указанное поле в область строк. |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | Указывает, можно ли удалить это pivot field из представления PivotTable. |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Указывает, сортируются ли элементы этого поля сводной таблицы автоматически по возрастанию. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Указывает, отображается ли указанный поле PivotTable автоматически. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Представляет индекс автоматически отображаемого поля. -1 означает сам PivotField. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Указывает, сортируются ли элементы этого поля PivotTable автоматически. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Представляет индекс поля, которое автоматически сортируется. |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Указывает, показывает ли указанный поле автоматические промежуточные итоги. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Представляет индекс в исходных полях pivot. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Устанавливает текущий отображаемый элемент страницы для этого сводного поля (только поле страниц). |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | Получает отображаемый текст текущего элемента страницы для этого поля сводки (только поле страницы). |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Представляет отображаемое имя поля сводки в представлении сводной таблицы. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Указывает, можно ли перетаскивать указанное поле в область столбцов. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Указывает, можно ли перетаскивать указанное поле в область значений. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Указывает, можно ли удалить это pivot field из представления PivotTable. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Указывает, можно ли перетаскивать указанное поле в область страниц. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Указывает, можно ли перетаскивать указанное поле в область строк. |
| [setFunction(int value)](#setFunction-int-) | Представляет функцию, используемую для суммирования этого поля данных сводной таблицы. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Указывает, включать ли новые элементы в поле при ручной фильтрации. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Указывает, следует ли вставлять пустую строку после каждого элемента. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Указывает, следует ли вставлять разрывы страниц после каждого элемента. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Указывает, можно ли выбирать несколько элементов в поле страниц. |
| [setName(String value)](#setName-java.lang.String-) | Представляет имя PivotField. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Указывает, является ли операция сортировки, применяемая к этому полю сводки, автоматической сортировкой или простой сортировкой данных. |
| [setNumber(int value)](#setNumber-int-) | Представляет встроенный формат отображения чисел и дат. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Представляет пользовательский формат отображения чисел и дат. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Указывает, следует ли повторять метки поля в области строк или столбцов. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Указывает, следует ли отображать все элементы в представлении PivotTable, даже если они не содержат сводных данных. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Указывает, следует ли отображать метки следующего поля в той же колонке в представлении Pivot Table. |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | Устанавливает значение, указывающее, использует ли это поле строк компактный макет. |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Устанавливает значение, указывающее, использует ли это поле строк макет в виде контура. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Указывает, следует ли отображать промежуточные итоги вверху или внизу элементов. |
| [setSubtotals(int value)](#setSubtotals-int-) | Устанавливает промежуточные итоги поля. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Устанавливает способ подсчёта промежуточных итогов указанного поля. |
| [showAllDetails()](#showAllDetails--) | Показать все детали каждого сводного элемента. |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | Устанавливает расчёт "Показать значения как" для этого сводного поля. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | Отображает значения поля данных в другом формате, когда используется расчёт ShowDataAs. |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | Настраивает расчёт "Показать значения как" для этого поля данных. |
| [sortBy(int sortType)](#sortBy-int-) | Сортирует это сводное поле. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | Сортирует это сводное поле. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | Сортирует это сводное поле. |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | Сортирует это сводное поле. |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | Настраивает параметры Top10 AutoShow для этого сводного поля. |
| [ungroup()](#ungroup--) | Разгруппировать сводное поле. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Добавить вычисляемый элемент формулы в pivot field.

**Remarks**

Поддерживается только добавление вычисляемого элемента в поле строк/столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя элемента. |
| formula | java.lang.String | Формула сводного элемента. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Очищает настройки фильтра для этого pivot field.

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
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


Фильтрует по значениям даты в строковом или столбцовом pivot field.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Тип фильтрации данных. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | Дата метки условия фильтра |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | Верхняя граница даты метки условия фильтра между |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


Фильтрует по подписьям строки или столбца сводного поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Тип фильтрации данных. |
| label1 | java.lang.String | Метка условия фильтра |
| label2 | java.lang.String | Верхняя граница метки условия фильтра между |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


Фильтрует по значениям данных сводного поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| valueFieldIndex | int | Индекс поля значения в области значений. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Тип фильтрации данных. |
| value1 | double | Значение условия фильтра |
| value2 | double | Верхнее значение условия фильтра между |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Фильтрует по значениям данных сводного поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| valueFieldIndex | int | Индекс поля данных в области данных. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Тип фильтрации данных. Может быть только Count, Sum и Percent. |
| isTop | boolean | Указывает, применяется ли фильтр сверху или снизу |
| itemCount | int | Количество элементов |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


Указывает, можно ли перетаскивать указанное поле в область столбцов. Значение по умолчанию — true.

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


Указывает, можно ли перетаскивать указанное поле в область значений. Значение по умолчанию — true.

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


Указывает, можно ли перетаскивать указанное поле в область страниц. Значение по умолчанию — true.

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


Указывает, можно ли перетаскивать указанное поле в область строк. Значение по умолчанию — true.

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


Указывает, можно ли удалить это сводное поле из представления сводной таблицы. Значение по умолчанию — true.

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.Top10AutoShowSettings.AutoShowCount или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


Представляет индекс поля автоотображения. -1 означает сам PivotField. Это должен быть индекс полей данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.Top10AutoShowSettings.RankBy или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


Представляет индекс поля, которое автоматически сортируется. -1 означает сам PivotField, остальные означают позицию полей данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.SortSetting.SortBy или метод PivotField.SortBy(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Представляет индекс в исходных полях pivot.

**Remarks**

ПРИМЕЧАНИЕ: Этот сеттер свойства теперь устарел. Этот сеттер будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Получить строку формулы указанного вычисляемого поля.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.GetFormula(). Этот метод будет удалён через 12 месяцев, начиная с августа 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


Получает текущий отображаемый элемент страницы для этого pivot field (только поле страницы).

**Remarks**

Используйте [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) в качестве сигнального значения, указывающего "Select All". Это предопределённый маркер и не является действительным индексом элемента.

**Returns:**
short
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


Получает отображаемый текст текущего элемента страницы для этого поля сводки (только поле страницы).

**Remarks**

Возвращает "(All)", когда [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) равно [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX). Для других значений возвращает строковое представление индекса элемента.

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Представляет отображаемое имя поля сводки в представлении сводной таблицы.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


Указывает, можно ли перетаскивать указанное поле в область столбцов. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToColumn. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


Указывает, можно ли перетаскивать указанное поле в область значений. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToData. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Указывает, можно ли удалить это сводное поле из представления сводной таблицы. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowRemovingFromView. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


Указывает, можно ли перетаскивать указанное поле в область страниц. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToPage. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


Указывает, можно ли перетаскивать указанное поле в область строк. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToRow. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


Получает все фильтры сводки, применённые к этому полю сводки.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


Получает формулу вычисляемого поля. Работает только для вычисляемого поля.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


Представляет функцию, используемую для суммирования этого поля данных сводной таблицы.

См. [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Получает настройки группировки поля сводки.

**Remarks**

Если это поле не сгруппировано, будет возвращено Null.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Указывает, следует ли вставлять пустую строку после каждого элемента. Только для полей строк.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Получает количество базовых элементов в этом поле сводки.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.PivotItems.Count. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Получить все метки элементов сводки в этом поле.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


Получает максимальное значение этого поля.

**Remarks**

Работает только для полей строк или столбцов, значение которых должно быть датой/временем, числом или пустым.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


Получает максимальное значение этого поля.

**Remarks**

Работает только для полей строк или столбцов, значение которых должно быть датой/временем, числом или пустым.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


Представляет имя PivotField.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


Указывает, является ли операция сортировки, применяемая к этому полю сводки, автоматической сортировкой или простой сортировкой данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство !PivotField.SortSetting.IsSimpleSort. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


Представляет встроенный формат отображения чисел и дат.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Представляет пользовательский формат отображения чисел и дат.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


Получить оригинальные базовые элементы;

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


Получает фильтр сводки поля по типу

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| тип | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


Получает фильтры сводки поля

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.GetFilters(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


Получает элементы сводки поля

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Представляет индекс [PivotField](../../com.aspose.cells/pivotfield) в области.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


Указывает область сводной таблицы, в которой отображается это поле.

Смотрите [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Указывает, следует ли отображать все элементы в представлении PivotTable, даже если они не содержат сводных данных. Значение по умолчанию — false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Указывает, следует ли отображать метки следующего поля в той же колонке в представлении Pivot Table. Только для полей строк.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.ShowInCompactForm. Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


Возвращает значение, указывающее, использует ли это поле строки компактный макет. Применяется только к полям строк.

**Remarks**

Компактный режим — это подрежим контурного макета. Эта настройка вступает в силу только когда [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) равно true.

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Возвращает значение, указывающее, использует ли это поле строки контурный макет. Применяется только к полям строк.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


Указывает, следует ли отображать промежуточные итоги вверху или внизу элементов.

**Remarks**

Работает только для полей сводной таблицы в строковой области, когда ShowInOutlineForm равно true.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


Получает параметры отображения значений, когда используется вычисление ShowDataAs.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


Получает все параметры автоматической сортировки

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


Возвращает промежуточные итоги поля. Только для полей сводной таблицы строк или столбцов.

См. [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Example**

```
         //No subtotals
         rowField.setSubtotals(PivotFieldSubtotalType.NONE);
         //Automatic subtotals
         //rowField.Subtotals = PivotFieldSubtotalType.Automatic;
         //Single subtotals: Sum
         //rowField.Subtotals = PivotFieldSubtotalType.Sum;
         //Multipl subtotals: Sum and count numbers 
         //rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

**Returns:**
int
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


Указывает, следует ли показывать указанный промежуточный итог для этого поля сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Тип промежуточного итога. |

**Returns:**
boolean — Возвращает, отображается ли указанный промежуточный итог.
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


Получает параметры автоматического отображения Top 10 для поля сводной таблицы.

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


Автоматически группировать поле.

**Remarks**

Если поле содержит только пустые значения и дату/время, оно будет сгруппировано по месяцам. Если поле содержит только пустые значения и числа, оно будет сгруппировано по числам. В остальных случаях возвращается false без какой-либо группы.

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


Группирует поле сводной таблицы с параметрами.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | Параметры настройки группировки полей сводной таблицы. |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Группировать файл по типам группировки даты.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isAutoStart | boolean | Указывает, следует ли автоматически определять значение даты и времени начала. |
| start | [DateTime](../../com.aspose.cells/datetime) | Дата и время начала |
| isAutoEnd | boolean | Указывает, следует ли автоматически определять значение даты и времени окончания. |
| end | [DateTime](../../com.aspose.cells/datetime) | Дата и время окончания |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Типы группировки |
| interval | double | Интервал |
| firstAsNewField | boolean | Указывает, следует ли добавить новое поле в сводную таблицу. Только для первого элемента группы. |

**Returns:**
boolean - False означает, что это поле нельзя сгруппировать по дате и времени.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


Группировать файл по числу.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isAutoStart | boolean | Указывает, следует ли автоматически определять начальное значение. |
| начало | double | Начальное значение |
| isAutoEnd | boolean | Указывает, следует ли автоматически определять конечное значение. |
| конец | double | Конечное значение |
| interval | double | Интервал |
| newField | boolean | Указывает, добавляется ли новое поле в сводную таблицу |

**Returns:**
boolean - False означает, что это поле нельзя сгруппировать по дате и времени.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Пользовательская группировка поля.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions options) с свойством PivotFieldGroupOptions.DiscreteGroupItems. Этот метод будет удалён через 6 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | Пользовательские элементы группы. |
| newField | boolean | Указывает, добавляется ли новое поле в сводную таблицу |

**Returns:**
boolean - False означает, что это поле нельзя сгруппировать по дате и времени.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Группировать файл по типам группировки даты.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | Дата и время начала |
| end | [DateTime](../../com.aspose.cells/datetime) | Дата и время окончания |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Типы группировки |
| interval | double | Интервал |
| firstAsNewField | boolean | Указывает, следует ли добавить новое поле в сводную таблицу. Только для первого элемента группы. |

**Returns:**
boolean - False означает, что это поле нельзя сгруппировать по дате и времени.
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


Пользовательская группировка поля.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions options) с свойством PivotFieldGroupOptions.DiscreteGroupItems. Этот метод будет удалён через 6 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | Пользовательские элементы группы. |
| newField | boolean | Указывает, добавляется ли новое поле в сводную таблицу |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


Автоматически группировать поле с интервалом

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| interval | double | Внутреннее значение группы. Автоматическое значение будет назначено, если оно равно нулю, |
| newField | boolean | Указывает, добавляется ли новое поле в сводную таблицу. Только для группировки по DateTime. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


Группировать файл по числу.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| начало | double | Начальное значение |
| конец | double | Конечное значение |
| interval | double | Интервал |
| newField | boolean | Указывает, добавляется ли новое поле в сводную таблицу |

**Returns:**
boolean - False означает, что это поле нельзя сгруппировать по дате и времени.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


Автоматически группировать поле с internal

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Типы группировки |
| interval | double | Внутреннее значение группы. Автоматическое значение будет назначено, если оно равно нулю, работает только при группировке по числам или дням. |
| newField | boolean | Указывает, добавляется ли новое поле в сводную таблицу. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetails() {#hideAllDetails--}
```
public void hideAllDetails()
```


Скрывает все детали каждого элемента сводной таблицы.

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


Устанавливает, скрыты ли детали всех PivotItems в поле сводной таблицы. То есть сворачивает/разворачивает это поле.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте методы PivotItemsCollection.HideAllDetails() и UnhideAllDetails(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isHiddenDetail | boolean | Скрывать ли детали сводного поля. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


Устанавливает, скрыт ли конкретный PivotItem в поле данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.PivotItems[int].IsHidden. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс pivotItem в pivotField. |
| isHidden | boolean | скрыт ли конкретный PivotItem |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


Устанавливает, скрыт ли конкретный PivotItem в поле данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.PivotItems[string].IsHidden. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| itemValue | java.lang.String | Имя pivotItem в pivotField. |
| isHidden | boolean | Скрыт ли конкретный PivotItem |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


Устанавливает, скрыты ли детали конкретного PivotItem в поле сводной таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.PivotItems[int].IsDetailHidden. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс pivotItem в pivotField. |
| isHiddenDetail | boolean | скрыт ли конкретный PivotItem |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


Инициализировать элементы сводного поля.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Пожалуйста, просто удалите вызов этого метода. Этот метод будет удалён через 6 месяцев, начиная с октября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.Top10AutoShowSettings.IsTop или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


Указывает, сортируются ли элементы этого поля сводной таблицы автоматически по возрастанию.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.SortSetting.SortType или метод PivotField.SortBy(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Указывает, отображается ли указанный поле PivotTable автоматически.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.Top10AutoShowSettings.IsAutoShow или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Указывает, сортируются ли элементы этого поля PivotTable автоматически.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.SortSetting.SortType или метод PivotField.SortBy(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


Указывает, отображает ли указанное поле автоматические промежуточные итоги. По умолчанию true.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


Указывает, является ли это поле сводной таблицы вычисляемым полем.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Указывает, скрыт ли конкретный PivotItem.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.PivotItems[int].IsHidden. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс pivotItem в pivotField. |

**Returns:**
boolean — скрыт ли конкретный PivotItem
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Указывает, скрывать ли детали конкретного PivotItem..

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.PivotItems[int].IsDetailHidden. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс pivotItem в pivotField. |

**Returns:**
boolean — скрыты ли детали конкретного PivotItem
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


Указывает, следует ли включать новые элементы в поле при ручной фильтрации. Значение по умолчанию — false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


Указывает, следует ли вставлять разрывы страниц после каждого элемента. Значение по умолчанию — false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


Указывает, можно ли выбирать несколько элементов в поле страниц. Значение по умолчанию — false.

**Remarks**

Только для полей страниц (фильтра).

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


Указывает, следует ли повторять метки поля в строковой или столбцовой области. Значение по умолчанию — false.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


Указывает, представляет ли это поле поля значений.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте свойство PivotField.IsValuesField. Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


Указывает, представляет ли это поле поле значений.

**Remarks**

Работает только при наличии двух и более полей данных в представлении сводной таблицы.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllowDraggingToColumn(boolean value) {#setAllowDraggingToColumn-boolean-}
```
public void setAllowDraggingToColumn(boolean value)
```


Указывает, можно ли перетаскивать указанное поле в область столбцов. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


Указывает, можно ли перетаскивать указанное поле в область значений. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


Указывает, можно ли перетаскивать указанное поле в область страниц. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


Указывает, можно ли перетаскивать указанное поле в область строк. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


Указывает, можно ли удалить это сводное поле из представления сводной таблицы. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.Top10AutoShowSettings.IsTop или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Указывает, сортируются ли элементы этого поля сводной таблицы автоматически по возрастанию.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.SortSetting.SortType или метод PivotField.SortBy(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Указывает, отображается ли указанный поле PivotTable автоматически.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.Top10AutoShowSettings.IsAutoShow или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.Top10AutoShowSettings.AutoShowCount или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Представляет индекс поля автоотображения. -1 означает сам PivotField. Это должен быть индекс полей данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.Top10AutoShowSettings.RankBy или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Указывает, сортируются ли элементы этого поля PivotTable автоматически.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.SortSetting.SortType или метод PivotField.SortBy(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Представляет индекс поля, которое автоматически сортируется. -1 означает сам PivotField, остальные означают позицию полей данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.SortSetting.SortBy или метод PivotField.SortBy(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Указывает, отображает ли указанное поле автоматические промежуточные итоги. По умолчанию true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Представляет индекс в исходных полях pivot.

**Remarks**

ПРИМЕЧАНИЕ: Этот сеттер свойства теперь устарел. Этот сеттер будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Устанавливает текущий отображаемый элемент страницы для этого сводного поля (только поле страниц).

**Remarks**

Используйте [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) в качестве сигнального значения, указывающего "Select All". Это предопределённый маркер и не является действительным индексом элемента.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | short |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


Получает отображаемый текст текущего элемента страницы для этого поля сводки (только поле страницы).

**Remarks**

Возвращает "(All)", когда [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) равно [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX). Для других значений возвращает строковое представление индекса элемента.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Представляет отображаемое имя поля сводки в представлении сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Указывает, можно ли перетаскивать указанное поле в область столбцов. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToColumn. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Указывает, можно ли перетаскивать указанное поле в область значений. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToData. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Указывает, можно ли удалить это сводное поле из представления сводной таблицы. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowRemovingFromView. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Указывает, можно ли перетаскивать указанное поле в область страниц. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToPage. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Указывает, можно ли перетаскивать указанное поле в область строк. Значение по умолчанию — true.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.AllowDraggingToRow. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Представляет функцию, используемую для суммирования этого поля данных сводной таблицы.

См. [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Указывает, следует ли включать новые элементы в поле при ручной фильтрации. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Указывает, следует ли вставлять пустую строку после каждого элемента. Только для полей строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Указывает, следует ли вставлять разрывы страниц после каждого элемента. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Указывает, можно ли выбирать несколько элементов в поле страниц. Значение по умолчанию — false.

**Remarks**

Только для полей страниц (фильтра).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Представляет имя PivotField.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Указывает, является ли операция сортировки, применяемая к этому полю сводки, автоматической сортировкой или простой сортировкой данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство !PivotField.SortSetting.IsSimpleSort. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Представляет встроенный формат отображения чисел и дат.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Представляет пользовательский формат отображения чисел и дат.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Указывает, следует ли повторять метки поля в строковой или столбцовой области. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Указывает, следует ли отображать все элементы в представлении PivotTable, даже если они не содержат сводных данных. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Указывает, следует ли отображать метки следующего поля в той же колонке в представлении Pivot Table. Только для полей строк.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.ShowInCompactForm. Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


Устанавливает значение, указывающее, использует ли это поле строк компактный макет. Применяется только к полям строк.

**Remarks**

Компактный режим — это подрежим контурного макета. Эта настройка вступает в силу только когда [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) равно true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Устанавливает значение, указывающее, использует ли это поле строк макет с контуром. Применяется только к полям строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Указывает, следует ли отображать промежуточные итоги вверху или внизу элементов.

**Remarks**

Работает только для полей сводной таблицы в строковой области, когда ShowInOutlineForm равно true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


Устанавливает промежуточные итоги поля. Только для полей строк или столбцов сводной таблицы.

См. [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Устанавливает способ подсчёта промежуточных итогов указанного поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| показано | boolean | Отображает ли указанное поле эти промежуточные итоги. |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


Показать все детали каждого сводного элемента.

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


Устанавливает расчёт "Показать значения как" для этого сводного поля.

**Remarks**

Только для поля данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Тип расчёта "Show Values As". |
| baseField | int | Индекс базового поля, используемого для расчёта. |
| baseItem | int | Индекс базового элемента для расчёта. Используйте [PivotShowValuesSetting.PREVIOUS\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#PREVIOUS-PIVOT-ITEM) (-1) для предыдущего элемента, [PivotShowValuesSetting.NEXT\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#NEXT-PIVOT-ITEM) (-2) для следующего элемента; отрицательные значения обозначают порядковый индекс конкретного элемента сводной таблицы. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


Отображает значения поля данных в другом формате, когда используется расчёт ShowDataAs.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). Тип формата отображения данных. |
| baseField | int | Индекс поля, на котором основан расчёт ShowDataAs. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). Тип позиции базового элемента. |
| baseItem | int | Индекс базового элемента, на котором основан расчёт ShowDataAs. Работает только когда baseItemPositionType имеет значение custom. |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


Настраивает расчёт "Показать значения как" для этого поля данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Тип расчёта для Show Values As. |
| baseField | java.lang.String | Имя базового поля, используемого в расчёте. |
| baseItem | java.lang.String | Подпись обычного элемента сводной таблицы. Также принимает зарезервированные литеральные ключевые слова: `(previous)` для предыдущего элемента, `(next)` для следующего элемента. Передайте `null`, если выбранный тип расчёта не требует базового элемента. |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


Сортирует это сводное поле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Тип сортировки этого поля. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


Сортирует это сводное поле.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotField.SortBy(SortOrder, int,string) или свойство PivotField.IsAutoSort. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Тип сортировки этого поля. |
| fieldSortedBy | int | Индекс поля сводной таблицы, по которому производится сортировка. -1 означает сортировку по меткам данных этого поля, остальные значения указывают индекс поля данных, по которому сортировать. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


Сортирует это сводное поле.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotField.SortBy(SortOrder, int,string). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Тип сортировки этого поля. |
| fieldSortedBy | int | Индекс поля сводной таблицы, по которому производится сортировка. -1 означает сортировку по меткам данных этого поля, остальные значения указывают индекс поля данных, по которому сортировать. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). Тип данных, по которым производится сортировка. |
| cellName | java.lang.String | Сортировать по значениям в строке или столбце |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


Сортирует это сводное поле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Тип сортировки этого поля. |
| fieldSortedBy | int | Индекс поля сводной таблицы, по которому производится сортировка. -1 означает сортировку по меткам данных этого поля, остальные значения указывают индекс поля данных, по которому сортировать. |
| cellName | java.lang.String | Сортировать по значениям в строке или столбце. Если Null, группировать по общему итогу поля, иначе группировать по значениям в выбранном столбце или строке. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy) {#top10AutoShow-boolean-boolean-int-int-}
```
public void top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)
```


Настраивает параметры Top10 AutoShow для этого сводного поля.

**Remarks**

Этот метод настраивает формат . XLS (двоичный): AutoShow (Top10) является нативным и единственно поддерживаемым вариантом. XLSX (OpenXML): базовый формат файла поддерживает AutoShow Top10, но пользовательский интерфейс Excel 2007 и новее отображает это только через фильтр Top10. Если совместимость с XLS не требуется, рекомендуется использовать фильтр Top10.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isAutoShow | boolean | true — включить AutoShow; false — отключить. |
| isTop | boolean | Если true, показывать верхние элементы; false — нижние элементы. |
| количество | int | Количество отображаемых верхних/нижних элементов. |
| rankBy | int | Индекс поля данных, используемого для ранжирования. Используйте -1 для ранжирования по собственным значениям элемента сводной таблицы. |

### ungroup() {#ungroup--}
```
public void ungroup()
```


Разгруппировать сводное поле.

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

