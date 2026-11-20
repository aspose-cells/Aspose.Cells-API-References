---
title: "PivotGlobalizationSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройки глобализации для сводных таблиц."
type: docs
url: /ru/java/com.aspose.cells/pivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotGlobalizationSettings
```

Представляет настройки глобализации для сводных таблиц.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotGlobalizationSettings()](#PivotGlobalizationSettings--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | Получает числовой формат группы дней сводки. |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | Получает отображаемое имя поля данных сводки. |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | Получает все коротко отформатированные строки за 12 месяцев. |
| [getTextOf24Hours()](#getTextOf24Hours--) | Получает все локально отформатированные строки за 24 часа. |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | Получает локальный текст для 4 кварталов. |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | Получает локальный текст для 4 кварталов. |
| [getTextOfAll()](#getTextOfAll--) | Получает текст метки "(All)" в сводной таблице. |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | Получает локализованный текст "All Periods". |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | Получает текст метки "Column Labels" в сводной таблице. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | Получает текст заголовка поля области значений в PivotTable. |
| [getTextOfDays()](#getTextOfDays--) | Получает локальный текст "Days". |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | Получает текст метки "(blank)" в PivotTable. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | Получает текст метки "Grand Total" в PivotTable. |
| [getTextOfHours()](#getTextOfHours--) | Получает локальный текст "Hours". |
| [getTextOfMinutes()](#getTextOfMinutes--) | Получает локальный текст "Minutes". |
| [getTextOfMonths()](#getTextOfMonths--) | Получает локальный текст "Months". |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | Получает текст метки "(Multiple Items)" в PivotTable. |
| [getTextOfOr()](#getTextOfOr--) | Получает все локально отформатированные строки "or". |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | Получает текст для указанного защищённого имени. |
| [getTextOfProtection()](#getTextOfProtection--) | Получает имя защиты в сводной таблице. |
| [getTextOfQuarters()](#getTextOfQuarters--) | Получает локальный текст "Quarters". |
| [getTextOfRange()](#getTextOfRange--) | Получает локальный текст "Range" |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | Получает текст метки "Row Labels" в PivotTable. |
| [getTextOfSeconds()](#getTextOfSeconds--) | Получает локальный текст "Seconds" |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | Получает текст типа [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) в PivotTable. |
| [getTextOfTotal()](#getTextOfTotal--) | Получает текст метки "Total" в PivotTable. |
| [getTextOfYears()](#getTextOfYears--) | Получает локальный текст "Years". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotGlobalizationSettings() {#PivotGlobalizationSettings--}
```
public PivotGlobalizationSettings()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatOfDayGroup() {#getFormatOfDayGroup--}
```
public String getFormatOfDayGroup()
```


Получает числовой формат группы дней сводной таблицы. Используется только при группировке поля сводной таблицы по дням. Значение по умолчанию — "d-MMM";

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


Получает отображаемое имя поля данных сводной таблицы. Формат по умолчанию — "Sum Of Field".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Функция используется для суммирования значений поля сводной таблицы. |
| name | java.lang.String | Исходное имя поля сводной таблицы. |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


Получает все коротко отформатированные строки за 12 месяцев.

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


Получает все локально отформатированные строки 24‑часового формата. Значение по умолчанию — 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM.

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


Получает локальный текст для 4 кварталов.

**Remarks**

По умолчанию возвращает Quarter1, Quarter2, Quarter3, Quarter4 до версии 26.9. По умолчанию возвращает Qtr1, Qtr2, Qtr3, Qtr4 начиная с версии 26.9.

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


Получает локальный текст для 4 кварталов.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetTextOf4Quarters() method. Это свойство будет удалено через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


Получает текст метки "(All)" в сводной таблице.

**Returns:**
java.lang.String - Текст метки "(All)"
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


Получает локализованный текст "All Periods".

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


Получает текст метки "Column Labels" в сводной таблице.

**Returns:**
java.lang.String - Текст меток столбцов
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


Получает текст заголовка поля области значений в PivotTable.

**Returns:**
java.lang.String - Текст названия заголовка поля данных
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


Получает локальный текст "Days".

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


Получает текст метки "(blank)" в PivotTable.

**Returns:**
java.lang.String - Текст пустых данных
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


Получает текст метки "Grand Total" в PivotTable.

**Returns:**
java.lang.String - Текст метки "Grand Total"
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


Получает локальный текст "Hours".

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


Получает локальный текст "Minutes".

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


Получает локальный текст "Months".

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


Получает текст метки "(Multiple Items)" в PivotTable.

**Returns:**
java.lang.String - Текст метки "(Multiple Items)"
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


Получает все локально отформатированные строки "or".

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


Получает текст для указанного защищённого имени.

**Remarks**

В Ms Excel некоторые имена нельзя использовать в качестве имен PivotFields в сводной таблице. Они различаются в разных регионах, пользователь может явно указать их в соответствии с используемым регионом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| protectedName | java.lang.String | Защищённое имя в сводной таблице. |

**Returns:**
java.lang.String - Локальные защищённые имена сводной таблицы.
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


Получает имя защиты в сводной таблице.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetTextOfProtectedName(string) method. Это свойство будет удалено через 12 месяцев, начиная с марта 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String - Имя защиты PivotTable
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


Получает локальный текст "Quarters".

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


Получает локальный текст "Range"

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


Получает текст метки "Row Labels" в PivotTable.

**Returns:**
java.lang.String - Текст меток строк
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


Получает локальный текст "Seconds"

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


Получает текст типа [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) в PivotTable.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Эта [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Текст данного типа
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


Получает текст метки "Total" в сводной таблице. Вам необходимо переопределить этот метод, когда в сводной таблице содержится два или более PivotFields в области данных.

**Returns:**
java.lang.String - Текст метки "Total"
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


Получает локальный текст "Years".

**Returns:**
java.lang.String -
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

