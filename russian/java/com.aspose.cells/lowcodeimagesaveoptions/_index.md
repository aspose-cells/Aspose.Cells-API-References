---
title: "LowCodeImageSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Параметры сохранения изображения в режиме low code."
type: docs
url: /ru/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

Параметры сохранения изображения в режиме low code.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | Параметры рендеринга изображений. |
| [getOutputFile()](#getOutputFile--) | Получает файл (при необходимости с путём) для сохранения сгенерированных данных. |
| [getOutputStream()](#getOutputStream--) | Получает поток для записи сгенерированных данных. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохранения. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | Провайдер параметров сохранения для сохранения сгенерированных изображений. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | Параметры рендеринга изображений. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Устанавливает файл (при необходимости с путём) для сохранения сгенерированных данных. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Устанавливает поток для записи сгенерированных данных. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Устанавливает формат сохранения. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Провайдер параметров сохранения для сохранения сгенерированных изображений. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeImageSaveOptions() {#LowCodeImageSaveOptions--}
```
public LowCodeImageSaveOptions()
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Параметры рендеринга изображений.

**Remarks**

Когда указана одна [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) экземпляр, [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) будет перезаписан(если он был указан ранее).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
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


Получает формат сохранения.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Если [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) был указан, установка этого свойства также изменит значение [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) у него.

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


Провайдер параметров сохранения для сохранения сгенерированных изображений.

**Remarks**

Вывод([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) или [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)), указанный этим экземпляром, не будет иметь эффекта, когда это свойство задано. Вместо этого вывод каждого сгенерированного изображения будет определён провайдером.

**Returns:**
[AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
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




### setImageOptions(ImageOrPrintOptions value) {#setImageOptions-com.aspose.cells.ImageOrPrintOptions-}
```
public void setImageOptions(ImageOrPrintOptions value)
```


Параметры рендеринга изображений.

**Remarks**

Когда указана одна [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) экземпляр, [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) будет перезаписан(если он был указан ранее).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

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


Устанавливает формат сохранения.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Если [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) был указан, установка этого свойства также изменит значение [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) у него.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


Провайдер параметров сохранения для сохранения сгенерированных изображений.

**Remarks**

Вывод([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) или [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)), указанный этим экземпляром, не будет иметь эффекта, когда это свойство задано. Вместо этого вывод каждого сгенерированного изображения будет определён провайдером.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) |  |

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

