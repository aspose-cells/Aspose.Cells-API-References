---
title: "LowCodeSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Параметры сохранения сгенерированных результатов в режиме low code."
type: docs
url: /ru/java/com.aspose.cells/lowcodesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class LowCodeSaveOptions
```

Параметры сохранения сгенерированных результатов в режиме low code.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LowCodeSaveOptions()](#LowCodeSaveOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Получает файл (при необходимости с путём) для сохранения сгенерированных данных. |
| [getOutputStream()](#getOutputStream--) | Получает поток для записи сгенерированных данных. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохранения для вывода. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Устанавливает файл (при необходимости с путём) для сохранения сгенерированных данных. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Устанавливает поток для записи сгенерированных данных. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Устанавливает формат сохранения для вывода. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptions() {#LowCodeSaveOptions--}
```
public LowCodeSaveOptions()
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
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


Получает файл (при необходимости с путём) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) будет игнорироваться.

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


Получает поток для записи сгенерированных данных. При установке этого свойства значением, отличным от null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) будет игнорироваться.

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Получает формат сохранения для вывода. Как правило, для конкретного процесса в режиме low‑code допускаются только определённые форматы. Пожалуйста, укажите правильный формат для соответствующего процесса, иначе могут возникнуть неожиданные результаты или даже исключения.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

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




### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


Устанавливает файл (при необходимости с путём) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) будет игнорироваться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


Устанавливает поток для записи сгенерированных данных. При установке этого свойства значением, отличным от null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) будет игнорироваться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Устанавливает формат сохранения для вывода. Как правило, для конкретного процесса в режиме low‑code допускаются только определённые форматы. Пожалуйста, укажите правильный формат для соответствующего процесса, иначе могут возникнуть неожиданные результаты или даже исключения.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

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

