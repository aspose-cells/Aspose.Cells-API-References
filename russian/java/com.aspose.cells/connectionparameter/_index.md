---
title: "ConnectionParameter"
second_title: "Справочник API Aspose.Cells for Java"
description: "Указывает свойства любых параметров, используемых во внешних соединениях данных. Параметры действительны для ODBC и веб‑запросов."
type: docs
url: /ru/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

Указывает свойства любых параметров, используемых во внешних соединениях данных. Параметры действительны для ODBC и веб‑запросов.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | Ссылка на ячейку, указывающая, значение какой ячейки использовать для параметра запроса. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Имя параметра. |
| [getPrompt()](#getPrompt--) | Строка подсказки для параметра. |
| [getRefreshOnChange()](#getRefreshOnChange--) | Флаг, указывающий, следует ли автоматически обновлять запрос, когда содержимое ячейки, предоставляющей значение параметра, изменяется. |
| [getSqlType()](#getSqlType--) | SQL‑тип данных параметра. |
| [getType()](#getType--) | Тип используемого параметра. |
| [getValue()](#getValue--) | Нецелочисленное числовое значение, целочисленное значение, строковое значение или логическое значение для использования в качестве параметра запроса. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | Ссылка на ячейку, указывающая, значение какой ячейки использовать для параметра запроса. |
| [setName(String value)](#setName-java.lang.String-) | Имя параметра. |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | Строка подсказки для параметра. |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | Флаг, указывающий, следует ли автоматически обновлять запрос, когда содержимое ячейки, предоставляющей значение параметра, изменяется. |
| [setSqlType(int value)](#setSqlType-int-) | SQL‑тип данных параметра. |
| [setType(int value)](#setType-int-) | Тип используемого параметра. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Нецелочисленное числовое значение, целочисленное значение, строковое значение или логическое значение для использования в качестве параметра запроса. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


Ссылка на ячейку, указывающая, значение какой ячейки использовать для параметра запроса. Используется только когда parameterType имеет значение cell.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Имя параметра.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


Строка подсказки для параметра. Предоставляется пользователю таблицы вместе с интерфейсом ввода для сбора значения параметра перед обновлением внешних данных. Используется только когда parameterType = prompt.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


Флаг, указывающий, следует ли автоматически обновлять запрос, когда содержимое ячейки, предоставляющей значение параметра, изменяется. Если true, внешние данные обновляются с использованием нового значения параметра каждый раз при изменении. Если false, внешние данные обновляются только по запросу пользователя или при возникновении другого события, вызывающего обновление (например, при открытии книги).

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


SQL‑тип данных параметра. Действителен только для источников ODBC.

См. [SqlDataType](../../com.aspose.cells/sqldatatype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Тип используемого параметра. Если parameterType=value, будет использовано значение из boolean, double, integer или string. В этом случае ожидается, что будет указано только одно из \\{boolean, double, integer, or string\\}.

См. [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Нецелочисленное числовое значение, целочисленное значение, строковое значение или логическое значение для использования в качестве параметра запроса. Используется только когда parameterType имеет значение value.

**Returns:**
java.lang.Object
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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


Ссылка на ячейку, указывающая, значение какой ячейки использовать для параметра запроса. Используется только когда parameterType имеет значение cell.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Имя параметра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


Строка подсказки для параметра. Предоставляется пользователю таблицы вместе с интерфейсом ввода для сбора значения параметра перед обновлением внешних данных. Используется только когда parameterType = prompt.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


Флаг, указывающий, следует ли автоматически обновлять запрос, когда содержимое ячейки, предоставляющей значение параметра, изменяется. Если true, внешние данные обновляются с использованием нового значения параметра каждый раз при изменении. Если false, внешние данные обновляются только по запросу пользователя или при возникновении другого события, вызывающего обновление (например, при открытии книги).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


SQL‑тип данных параметра. Действителен только для источников ODBC.

См. [SqlDataType](../../com.aspose.cells/sqldatatype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Тип используемого параметра. Если parameterType=value, будет использовано значение из boolean, double, integer или string. В этом случае ожидается, что будет указано только одно из \\{boolean, double, integer, or string\\}.

См. [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Нецелочисленное числовое значение, целочисленное значение, строковое значение или логическое значение для использования в качестве параметра запроса. Используется только когда parameterType имеет значение value.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

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

