---
title: "PivotFormatCondition"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет условие форматирования PivotTable в коллекции PivotFormatCondition."
type: docs
url: /ru/java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

Представляет условие форматирования PivotTable в коллекции PivotFormatCondition.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте класс [PivotConditionalFormat](../../com.aspose.cells/pivotconditionalformat). Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Example**

```
```
## Методы

| Метод | Описание |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | Добавляет ограничение условного форматирования PivotTable в полях столбцов. |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | Добавляет ограничение условного форматирования PivotTable в полях столбцов. |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | Добавляет ограничение условного форматирования PivotTable в полях данных. |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | Добавляет ограничение условного форматирования PivotTable в полях данных. |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | Добавляет ограничение условного форматирования PivotTable в полях строк. |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | Добавляет ограничение условного форматирования PivotTable в полях строк. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Получить условия для условного форматирования сводной таблицы. |
| [getRuleType()](#getRuleType--) | Получает тип правила для условного форматирования сводной таблицы. |
| [getScopeType()](#getScopeType--) | Получает тип области для условного форматирования сводной таблицы. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | Устанавливает условные области объекта PivotFormatCondition. |
| [setRuleType(int value)](#setRuleType-int-) | Устанавливает тип правила для условного форматирования сводной таблицы. |
| [setScopeType(int value)](#setScopeType-int-) | Устанавливает тип области для условного форматирования сводной таблицы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


Добавляет ограничение условного форматирования PivotTable в полях столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | Поле PivotField в полях столбцов. |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


Добавляет ограничение условного форматирования PivotTable в полях столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldName | java.lang.String | Имя PivotField. |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


Добавляет ограничение условного форматирования PivotTable в полях данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | Поле PivotField в полях данных. |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


Добавляет ограничение условного форматирования PivotTable в полях данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldName | java.lang.String | Имя PivotField. |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


Добавляет ограничение условного форматирования PivotTable в полях строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | Поле PivotField в полях строк. |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


Добавляет ограничение условного форматирования PivotTable в полях строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldName | java.lang.String | Имя PivotField. |

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
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Получить условия для условного форматирования сводной таблицы.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Получает тип правила для условного форматирования сводной таблицы.

См. [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Получает тип области для условного форматирования сводной таблицы.

См. [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Returns:**
int
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




### setConditionalAreas() {#setConditionalAreas--}
```
public void setConditionalAreas()
```


Устанавливает условные области объекта PivotFormatCondition.

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Устанавливает тип правила для условного форматирования сводной таблицы.

См. [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Устанавливает тип области для условного форматирования сводной таблицы.

См. [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

