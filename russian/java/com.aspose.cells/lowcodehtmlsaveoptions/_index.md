---
title: "LowCodeHtmlSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Параметры сохранения HTML в режиме low code."
type: docs
url: /ru/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

Параметры сохранения HTML в режиме low code.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | Общие параметры сохранения HTML. |
| [getOutputFile()](#getOutputFile--) | Получает файл (при необходимости с путём) для сохранения сгенерированных данных. |
| [getOutputStream()](#getOutputStream--) | Получает поток для записи сгенерированных данных. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат электронной таблицы. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | Общие параметры сохранения HTML. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Устанавливает файл (при необходимости с путём) для сохранения сгенерированных данных. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Устанавливает поток для записи сгенерированных данных. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Устанавливает формат электронной таблицы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeHtmlSaveOptions() {#LowCodeHtmlSaveOptions--}
```
public LowCodeHtmlSaveOptions()
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
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


Общие параметры сохранения HTML.

**Remarks**

Когда указана одна [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) экземпляр, метод [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) будет перезаписан (если он был указан ранее).

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
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


Получает формат электронной таблицы.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

При изменении этого свойства формат сохранения, указанный методом [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--), будет игнорироваться (если он был указан ранее).

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




### setHtmlOptions(HtmlSaveOptions value) {#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-}
```
public void setHtmlOptions(HtmlSaveOptions value)
```


Общие параметры сохранения HTML.

**Remarks**

Когда указана одна [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) экземпляр, метод [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) будет перезаписан (если он был указан ранее).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

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


Устанавливает формат электронной таблицы.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

При изменении этого свойства формат сохранения, указанный методом [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--), будет игнорироваться (если он был указан ранее).

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

