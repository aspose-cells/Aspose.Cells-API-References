---
title: "FormulaParseOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры при разборе формулы."
type: docs
url: /ru/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

Представляет параметры при разборе формулы.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | Определяет, следует ли проверять надстройки в существующих внешних ссылках текущей книги для пользовательской функции без внешней ссылки. |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | Определение для разбора пользовательских функций. |
| [getLocaleDependent()](#getLocaleDependent--) | Отформатирована ли формула в соответствии с локалью. |
| [getParse()](#getParse--) | Определяет, разбирать ли заданную формулу. |
| [getR1C1Style()](#getR1C1Style--) | Определяет, использует ли формула стиль ссылок R1C1. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | Определяет, следует ли проверять надстройки в существующих внешних ссылках текущей книги для пользовательской функции без внешней ссылки. |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Определение для разбора пользовательских функций. |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | Отформатирована ли формула в соответствии с локалью. |
| [setParse(boolean value)](#setParse-boolean-) | Определяет, разбирать ли заданную формулу. |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | Определяет, использует ли формула стиль ссылок R1C1. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
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
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


Определяет, проверять ли надстройки в существующих внешних ссылках текущей книги для пользовательской функции без внешней ссылки. По умолчанию true (если пользовательская функция совпадает с одной надстройкой в существующих внешних ссылках, то она считается надстройкой).

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


Определение для разбора пользовательских функций.

**Remarks**

Для некоторых специальных требований, например при вычислении пользовательской функции в пользовательском движке, некоторые её параметры необходимо вычислять в массивном режиме; использование этого свойства позволяет пометить такие параметры как массивные при разборе формулы. В противном случае пользователю потребуется позже обновить эти пользовательские функции с помощью [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-), чтобы получить тот же результат.

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


Определяет, отформатирована ли формула в соответствии с локалью. По умолчанию false.

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


Определяет, разбирать ли заданную формулу. По умолчанию true. Если false, то строка формулы будет оставаться без изменений в ячейке, пока пользователь не вызовет другие методы для её разбора или пока разобранные данные формулы не потребуются другим операциям, например при вычислении формул.

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


Определяет, использует ли формула стиль ссылок R1C1. По умолчанию false.

**Returns:**
boolean
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




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


Определяет, проверять ли надстройки в существующих внешних ссылках текущей книги для пользовательской функции без внешней ссылки. По умолчанию true (если пользовательская функция совпадает с одной надстройкой в существующих внешних ссылках, то она считается надстройкой).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


Определение для разбора пользовательских функций.

**Remarks**

Для некоторых специальных требований, например при вычислении пользовательской функции в пользовательском движке, некоторые её параметры необходимо вычислять в массивном режиме; использование этого свойства позволяет пометить такие параметры как массивные при разборе формулы. В противном случае пользователю потребуется позже обновить эти пользовательские функции с помощью [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-), чтобы получить тот же результат.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


Определяет, отформатирована ли формула в соответствии с локалью. По умолчанию false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


Определяет, разбирать ли заданную формулу. По умолчанию true. Если false, то строка формулы будет оставаться без изменений в ячейке, пока пользователь не вызовет другие методы для её разбора или пока разобранные данные формулы не потребуются другим операциям, например при вычислении формул.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


Определяет, использует ли формула стиль ссылок R1C1. По умолчанию false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

