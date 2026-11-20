---
title: "GlobalizationSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройки глобализации."
type: docs
url: /ru/java/com.aspose.cells/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

Представляет настройки глобализации.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Сравнивает две строковые величины согласно определённым правилам сортировки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | Получает имя метки "(All)" в PivotTable. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Получает строковое представление логического значения ячейки |
| [getChartSettings()](#getChartSettings--) | Получает настройки глобализации для Chart. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Преобразует строку в сравнимый объект согласно определённым правилам сортировки. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | Получает имя метки "Column Labels" в PivotTable. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Получает разделитель для элементов строковых данных массива в формуле. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | Получает имя заголовка поля области значений в PivotTable. |
| [getDefaultSheetName()](#getDefaultSheetName--) | Получает имя листа по умолчанию для автоматического добавления листа. |
| [getEmptyDataName()](#getEmptyDataName--) | Получает имя метки "(blank)" в сводной таблице. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Получает строковое значение отображения для ошибочного значения ячейки |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Получает имя общего итога функции. |
| [getListSeparator()](#getListSeparator--) | Получает разделитель для списка, параметров функции и т.д. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Получает зависящий от локали текст для встроенного имени в соответствии с заданным стандартным текстом. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Получает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [getMultipleItemsName()](#getMultipleItemsName--) | Получает имя метки "(Multiple Items)" в сводной таблице. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | Получает имя метки "Grand Total" в сводной таблице. |
| [getPivotSettings()](#getPivotSettings--) | Получает настройки глобализации для сводной таблицы. |
| [getPivotTotalName()](#getPivotTotalName--) | Получает имя метки "Total" в сводной таблице. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | Получает имя защиты в сводной таблице. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | Получает имя метки "Row Labels" в сводной таблице. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | Получает разделитель для строк в данных массива в формуле. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | Получает стандартный текст встроенного имени в соответствии с заданным зависящим от локали текстом. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | Получает стандартное имя функции в соответствии с заданным зависящим от локали именем функции. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для верхнего/нижнего колонтитула в соответствии с заданным локализованным названием стиля шрифта. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | Получает имя типа [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) в сводной таблице. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | Получает название типа строк таблицы, которые состоят из всех строк в ссылочной таблице. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | Получает название типа строк таблицы, которые состоят из текущей строки в ссылочной таблице. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | Получает название типа строк таблицы, которые состоят из области данных ссылочной таблицы. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | Получает название типа строк таблицы, которые состоят из заголовка таблицы. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | Получает название типа строк таблицы, которые состоят из итоговой строки ссылочной таблицы. |
| [getTotalName(int functionType)](#getTotalName-int-) | Возвращает полное имя функции. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Устанавливает настройки глобализации для диаграммы. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Устанавливает параметры глобализации для сводной таблицы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Сравнивает две строковые величины согласно определённым правилам сортировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| v1 | java.lang.String | первая строка |
| v2 | java.lang.String | вторая строка |
| ignoreCase | boolean | нужно ли игнорировать регистр при сравнении значений |

**Returns:**
int — целое число, указывающее лексическое отношение между двумя сравниваемыми значениями
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


Получает имя метки "(All)" в PivotTable.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод GlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String — имя метки "(All)"
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


Получает строковое представление логического значения ячейки

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| bv | boolean | логическое значение |

**Returns:**
java.lang.String - По умолчанию возвращает "TRUE" для истинного значения и "FALSE" для ложного значения.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


Получает настройки глобализации для Chart.

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Преобразует строку в сравнимый объект согласно определённым правилам сортировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| v | java.lang.String | Значение String должно сравниваться с другими. |
| ignoreCase | boolean | нужно ли игнорировать регистр при сравнении значений |

**Returns:**
java.lang.Comparable - Объект может использоваться для сравнения или сортировки строковых значений.
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


Получает имя метки "Column Labels" в PivotTable.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя меток столбцов
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


Получает разделитель для элементов строковых данных массива в формуле.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). |

**Returns:**
java.lang.String -
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


Получает имя заголовка поля области значений в PivotTable.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя заголовка поля данных
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


Получает имя листа по умолчанию для автоматического добавления листа. По умолчанию это "Sheet".

**Remarks**

Имя автоматически добавляемого (например, с помощью [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\#add--)) листа будет состоять из указанного имени плюс порядковый номер. Например, пользователь из Германии может захотеть, чтобы имя листа было "Tabellenblatt2" вместо "Sheet2". Тогда пользователь может реализовать этот метод, чтобы он возвращал "Tabellenblatt".

**Returns:**
java.lang.String - имя листа по умолчанию для автоматического добавления листа
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


Получает имя метки "(blank)" в сводной таблице.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя пустых данных
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


Получает строковое значение отображения для ошибочного значения ячейки

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| err | java.lang.String | значения ошибок, такие как \\#VALUE!,\\#NAME? |

**Returns:**
java.lang.String - По умолчанию возвращает само значение ошибки
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Получает имя общего итога функции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Тип функции. |

**Returns:**
java.lang.String - Имя общего итога функции.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


Получает разделитель для списка, параметров функции и т.д.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


Получает зависящий от локали текст для встроенного имени в соответствии с заданным стандартным текстом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| standardName | java.lang.String | Текст встроенного имени Standard (локаль en-US). |

**Returns:**
java.lang.String - Текст, зависящий от локали. Локаль была указана Workbook, для которого используются эти настройки.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


Получает зависящее от локали имя функции в соответствии с заданным стандартным именем функции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| standardName | java.lang.String | Имя функции Standard (локаль en-US). |

**Returns:**
java.lang.String - Имя функции, зависящее от локали. Локаль была указана Workbook, для которого используются эти настройки.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


Получает имя метки "(Multiple Items)" в сводной таблице.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя метки "(Multiple Items)"
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


Получает имя метки "Grand Total" в сводной таблице.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя метки "Grand Total"
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


Получает настройки глобализации для сводной таблицы.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


Получает имя метки "Total" в сводной таблице. Вам необходимо переопределить этот метод, когда сводная таблица содержит два или более PivotFields в области данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя метки "Total"
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


Получает имя защиты в сводной таблице.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте метод PivotGlobalizationSettings.GetTextOfProtectedName(string). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя защиты PivotTable
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


Получает имя метки "Row Labels" в сводной таблице.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя меток строк
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


Получает разделитель для строк в данных массива в формуле.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


Получает стандартный текст встроенного имени в соответствии с заданным зависящим от локали текстом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| localName | java.lang.String | Текст встроенного имени, зависящий от локали. Локаль была указана в Workbook, для которого используются эти настройки. |

**Returns:**
java.lang.String - Стандартный текст (локаль en-US).
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


Получает стандартное имя функции в соответствии с заданным зависящим от локали именем функции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| localName | java.lang.String | Имя функции, зависящее от локали. Локаль была указана в Workbook, для которого используются эти настройки. |

**Returns:**
java.lang.String - Стандартное имя функции (локаль en-US).
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для верхнего/нижнего колонтитула в соответствии с заданным локализованным названием стиля шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Имя стиля шрифта, зависящее от локали, для Header/Footer. |

**Returns:**
java.lang.String - Стандартное английское имя стиля шрифта (Regular, Bold, Italic)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


Получает имя типа [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) в сводной таблице.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Тип [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Имя типа [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Возвращает типовое имя строк таблицы, которое состоит из всех строк в ссылочной таблице. Значение по умолчанию — "All", поэтому в формуле "\#All" представляет все строки в ссылочной таблице.

**Returns:**
java.lang.String - имя типа строк таблицы
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Возвращает типовое имя строк таблицы, которое состоит из текущей строки в ссылочной таблице. Значение по умолчанию — "This Row", поэтому в формуле "\#This Row" представляет текущую строку в ссылочной таблице.

**Returns:**
java.lang.String - имя типа строк таблицы
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


Получает имя типа строк таблицы, которые составляют область данных ссылочной таблицы. По умолчанию это "Data", поэтому в формуле "\#Data" представляет область данных таблицы.

**Returns:**
java.lang.String - имя типа строк таблицы
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


Получает имя типа строк таблицы, которые составляют заголовок таблицы. По умолчанию это "Headers", поэтому в формуле "\#Headers" представляет заголовок таблицы.

**Returns:**
java.lang.String - имя типа строк таблицы
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


Возвращает типовое имя строк таблицы, которое состоит из итоговой строки в ссылочной таблице. Значение по умолчанию — "Totals", поэтому в формуле "\#Totals" представляет итоговую строку в ссылочной таблице.

**Returns:**
java.lang.String - имя типа строк таблицы
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Возвращает полное имя функции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Тип функции. |

**Returns:**
java.lang.String - Общее имя функции.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Устанавливает настройки глобализации для диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Устанавливает параметры глобализации для сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

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

