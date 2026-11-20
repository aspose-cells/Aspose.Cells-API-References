---
title: "TxtValueQuoteType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Указывает тип использования кавычек для значений в файлах текстового формата."
type: docs
url: /ru/java/com.aspose.cells/txtvaluequotetype/
---

**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```

Указывает тип использования кавычек для значений в файлах текстового формата.
## Поля

| Поле | Описание |
| --- | --- |
| [ALWAYS](#ALWAYS) | Все значения всегда будут заключены в кавычки. |
| [MINIMUM](#MINIMUM) | Кавычки ставятся только при необходимости. |
| [NEVER](#NEVER) | Все значения не будут заключены в кавычки. |
| [NORMAL](#NORMAL) | Все значения, содержащие специальные символы, такие как кавычка или разделитель, будут заключены в кавычки. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Все значения всегда будут заключены в кавычки.

### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```


Кавычки ставятся только при необходимости. Например, если значение содержит кавычку, но кавычка не находится в начале значения, это значение не будет заключено в кавычки.

### NEVER {#NEVER}
```
public static final int NEVER
```


Все значения не будут заключены в кавычки. Экспортированный текстовый файл этого типа может быть считан некорректно, потому что необходимые кавычки отсутствуют.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Все значения, содержащие специальные символы, такие как кавычка или разделитель, будут заключены в кавычки. То же самое, что и поведение MS Excel при экспорте текстового файла.

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

