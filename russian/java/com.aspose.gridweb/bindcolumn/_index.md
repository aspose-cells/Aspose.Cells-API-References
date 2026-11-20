---
title: "BindColumn"
second_title: "Справочник API Aspose.Cells for Java"
description: "BindColumn."
type: docs
url: /ru/java/com.aspose.gridweb/bindcolumn/
---

**Inheritance:**
java.lang.Object
```
public class BindColumn
```

BindColumn.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [BindColumn()](#BindColumn--) | Конструктор по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeStyle()](#getAlternativeStyle--) | Получает альтернативный стиль столбца. |
| [getCaption()](#getCaption--) | Подпись столбца. |
| [getClass()](#getClass--) |  |
| [getColumnHeaderStyle()](#getColumnHeaderStyle--) | Получает стиль столбца. |
| [getCommandName()](#getCommandName--) | Имя команды столбца. |
| [getCommandText()](#getCommandText--) | Отображаемый текст команды столбца. |
| [getCustomFormat()](#getCustomFormat--) | Пользовательская строка формата. |
| [getDataField()](#getDataField--) | Получает строку имени поля данных. |
| [getEnableSort()](#getEnableSort--) | Указывает, может ли пользователь щелкнуть заголовок столбца для сортировки по этому полю. |
| [getImageUrl()](#getImageUrl--) | URL изображения гиперссылки команды. |
| [getName()](#getName--) | Используется только во время разработки. |
| [getNumberType()](#getNumberType--) | Получает тип числа столбца. |
| [getStyle()](#getStyle--) | Получает стиль столбца. |
| [getUseAlternativeStyle()](#getUseAlternativeStyle--) | Получает, использовать ли альтернативный стиль для столбца. |
| [getValidation()](#getValidation--) | Получает объект проверки столбца. |
| [getWidth()](#getWidth--) | Получает или задает ширину столбца. Принимаются только пиксели или пункты. |
| [hashCode()](#hashCode--) |  |
| [isAutoCreated()](#isAutoCreated--) | Указывает, создаётся ли столбец автоматически. |
| [isReadOnly()](#isReadOnly--) | Указывает, является ли столбец только для чтения. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlternativeStyle(GridTableItemStyle value)](#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-) | Устанавливает альтернативный стиль столбца. |
| [setAutoCreated(boolean value)](#setAutoCreated-boolean-) | Указывает, создаётся ли столбец автоматически. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Подпись столбца. |
| [setColumnHeaderStyle(GridTableItemStyle value)](#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-) | Устанавливает стиль столбца. |
| [setCommandName(String value)](#setCommandName-java.lang.String-) | Имя команды столбца. |
| [setCommandText(String value)](#setCommandText-java.lang.String-) | Отображаемый текст команды столбца. |
| [setCustomFormat(String value)](#setCustomFormat-java.lang.String-) | Пользовательская строка формата. |
| [setDataField(String value)](#setDataField-java.lang.String-) | Устанавливает строку имени поля данных. |
| [setEnableSort(boolean value)](#setEnableSort-boolean-) | Указывает, может ли пользователь щелкнуть заголовок столбца для сортировки по этому полю. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | URL изображения гиперссылки команды. |
| [setNumberType(int value)](#setNumberType-int-) | Устанавливает тип числа столбца. |
| [setReadOnly(boolean value)](#setReadOnly-boolean-) | Указывает, является ли столбец только для чтения. |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Устанавливает стиль столбца. |
| [setUseAlternativeStyle(boolean value)](#setUseAlternativeStyle-boolean-) | Устанавливает, использовать ли альтернативный стиль для столбца. |
| [setValidation(GridValidation value)](#setValidation-com.aspose.gridweb.GridValidation-) | Устанавливает объект проверки столбца. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Получает или задает ширину столбца. Принимаются только пиксели или пункты. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BindColumn() {#BindColumn--}
```
public BindColumn()
```


Конструктор по умолчанию.

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
### getAlternativeStyle() {#getAlternativeStyle--}
```
public GridTableItemStyle getAlternativeStyle()
```


Получает альтернативный стиль столбца.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCaption() {#getCaption--}
```
public String getCaption()
```


Подпись столбца.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnHeaderStyle() {#getColumnHeaderStyle--}
```
public GridTableItemStyle getColumnHeaderStyle()
```


Получает стиль столбца.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCommandName() {#getCommandName--}
```
public String getCommandName()
```


Имя команды столбца. Гиперссылка CellCommand будет создана в привязанной ячейке, если свойство CommandName установлено.

**Returns:**
java.lang.String
### getCommandText() {#getCommandText--}
```
public String getCommandText()
```


Отображаемый текст команды столбца. Если установить значение null, ячейка будет использовать значение поля в качестве текста команды.

**Returns:**
java.lang.String
### getCustomFormat() {#getCustomFormat--}
```
public String getCustomFormat()
```


Пользовательская строка формата.

**Returns:**
java.lang.String
### getDataField() {#getDataField--}
```
public String getDataField()
```


Получает строку имени поля данных.

**Returns:**
java.lang.String
### getEnableSort() {#getEnableSort--}
```
public boolean getEnableSort()
```


Указывает, может ли пользователь щелкнуть заголовок столбца для сортировки по этому полю.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


URL изображения гиперссылки команды.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Используется только во время разработки.

**Returns:**
java.lang.String
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Получает тип числа столбца.

См. [NumberType](../../com.aspose.gridweb/numbertype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Получает стиль столбца.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getUseAlternativeStyle() {#getUseAlternativeStyle--}
```
public boolean getUseAlternativeStyle()
```


Получает, использовать ли альтернативный стиль для столбца.

**Returns:**
boolean
### getValidation() {#getValidation--}
```
public GridValidation getValidation()
```


Получает объект проверки столбца.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Получает или задает ширину столбца. Принимаются только пиксели или пункты.

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoCreated() {#isAutoCreated--}
```
public boolean isAutoCreated()
```


Указывает, создаётся ли столбец автоматически. Если true, столбец будет удалён, когда пользователь изменит источник данных во время разработки.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Указывает, является ли столбец только для чтения.

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




### setAlternativeStyle(GridTableItemStyle value) {#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setAlternativeStyle(GridTableItemStyle value)
```


Устанавливает альтернативный стиль столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoCreated(boolean value) {#setAutoCreated-boolean-}
```
public void setAutoCreated(boolean value)
```


Указывает, создаётся ли столбец автоматически. Если true, столбец будет удалён, когда пользователь изменит источник данных во время разработки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Подпись столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setColumnHeaderStyle(GridTableItemStyle value) {#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setColumnHeaderStyle(GridTableItemStyle value)
```


Устанавливает стиль столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setCommandName(String value) {#setCommandName-java.lang.String-}
```
public void setCommandName(String value)
```


Имя команды столбца. Гиперссылка CellCommand будет создана в привязанной ячейке, если свойство CommandName установлено.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCommandText(String value) {#setCommandText-java.lang.String-}
```
public void setCommandText(String value)
```


Отображаемый текст команды столбца. Если установить значение null, ячейка будет использовать значение поля в качестве текста команды.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCustomFormat(String value) {#setCustomFormat-java.lang.String-}
```
public void setCustomFormat(String value)
```


Пользовательская строка формата.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDataField(String value) {#setDataField-java.lang.String-}
```
public void setDataField(String value)
```


Устанавливает строку имени поля данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setEnableSort(boolean value) {#setEnableSort-boolean-}
```
public void setEnableSort(boolean value)
```


Указывает, может ли пользователь щелкнуть заголовок столбца для сортировки по этому полю.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


URL изображения гиперссылки команды.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Устанавливает тип числа столбца.

См. [NumberType](../../com.aspose.gridweb/numbertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setReadOnly(boolean value) {#setReadOnly-boolean-}
```
public void setReadOnly(boolean value)
```


Указывает, является ли столбец только для чтения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Устанавливает стиль столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setUseAlternativeStyle(boolean value) {#setUseAlternativeStyle-boolean-}
```
public void setUseAlternativeStyle(boolean value)
```


Устанавливает, использовать ли альтернативный стиль для столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setValidation(GridValidation value) {#setValidation-com.aspose.gridweb.GridValidation-}
```
public void setValidation(GridValidation value)
```


Устанавливает объект проверки столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridValidation](../../com.aspose.gridweb/gridvalidation) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Получает или задает ширину столбца. Принимаются только пиксели или пункты.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

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

