---
title: "DocumentProperty"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет пользовательское или встроенное свойство документа."
type: docs
url: /ru/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

Представляет пользовательское или встроенное свойство документа.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         DocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
 
         //Accessng a custom document property by using the property index
         DocumentProperty customProperty1 = customProperties.get(3);
 
         //Accessng a custom document property by using the property name
         DocumentProperty customProperty2 = customProperties.get("Owner");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Возвращает имя свойства. |
| [getSource()](#getSource--) | Связанный источник контента. |
| [getType()](#getType--) | Получает тип данных свойства. |
| [getValue()](#getValue--) | Получает значение свойства. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | Возвращает true, если у этого свойства нет имени в хранилище OLE2 и уникальное имя было сгенерировано только для публичного API. |
| [isLinkedToContent()](#isLinkedToContent--) | Указывает, связано ли это свойство с содержимым. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | Устанавливает значение свойства. |
| [toBool()](#toBool--) | Возвращает значение свойства как bool. |
| [toDateTime()](#toDateTime--) | Возвращает значение свойства как DateTime в локальном часовом поясе. |
| [toDouble()](#toDouble--) | Возвращает значение свойства как double. |
| [toInt()](#toInt--) | Возвращает значение свойства как integer. |
| [toString()](#toString--) | Возвращает значение свойства в виде строки. |
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


Возвращает имя свойства.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


Связанный источник контента.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Получает тип данных свойства.

Смотрите [PropertyType](../../com.aspose.cells/propertytype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Получает значение свойства.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGeneratedName() {#isGeneratedName--}
```
public boolean isGeneratedName()
```


Возвращает true, если у этого свойства нет имени в хранилище OLE2 и уникальное имя было сгенерировано только для публичного API.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


Указывает, связано ли это свойство с содержимым.

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




### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Устанавливает значение свойства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


Возвращает значение свойства как bool.

**Remarks**

Выбрасывает исключение, если тип свойства не PropertyType.Boolean.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


Возвращает значение свойства как DateTime в локальном часовом поясе.

**Remarks**

Выбрасывает исключение, если тип свойства не PropertyType.Date.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


Возвращает значение свойства как double.

**Remarks**

Выбрасывает исключение, если тип свойства не PropertyType.Float.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


Возвращает значение свойства как integer.

**Remarks**

Выбрасывает исключение, если тип свойства не PropertyType.Number.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


Возвращает значение свойства в виде строки.

**Remarks**

Преобразует числовое свойство с помощью Object.ToString(). Преобразует логическое свойство в "Y" или "N". Преобразует свойство даты в короткую строку даты.

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

