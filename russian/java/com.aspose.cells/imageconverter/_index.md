---
title: "ImageConverter"
second_title: "Справочник API Aspose.Cells for Java"
description: "Конвертер для преобразования шаблонного файла в изображения."
type: docs
url: /ru/java/com.aspose.cells/imageconverter/
---

**Inheritance:**
java.lang.Object
```
public class ImageConverter
```

Конвертер для преобразования шаблонного файла в изображения.

**Example**

```
         ImageConverter.process("template.xlsx", "res.png");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | Преобразует файл шаблона в изображения |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Преобразует файл шаблона в изображения |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Преобразует файл шаблона в изображения. |
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```


Преобразует файл шаблона в изображения

**Remarks**

При конвертации в изображение формата, поддерживающего несколько страниц (например, tiff), указанные [LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) или [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) будут использованы напрямую для полученного изображения.

Для других типов изображений, если параметры сохранения указали Stream в качестве вывода, все полученные изображения будут сохранены в один и тот же Stream. В противном случае файлы вывода будут созданы на основе указанного выходного файла параметров сохранения путем добавления номера листа и части разбиения. Например, если указанный выходной файл — Image.png, то сгенерированные файлы изображений будут Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Параметры ввода и загрузки |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Параметры вывода и сохранения |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)
```


Преобразует файл шаблона в изображения

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Параметры ввода и загрузки |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Параметры сохранения. Его вывод ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) или [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) не оказывает влияния, поскольку все выводы будут задаваться параметром "provider". |
| provider | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) | Поставщик параметров сохранения для сохранения сгенерированных изображений |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Преобразует файл шаблона в изображения.

**Remarks**

Файлы вывода будут созданы на основе указанного результирующего файла путем добавления номера листа и части разбиения. Например, если указанный выходной файл — Image.png, то сгенерированные файлы изображений будут Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | java.lang.String | Файл шаблона, который будет преобразован в изображения. |
| resultFile | java.lang.String | Полученный файл (шаблон имени) для сгенерированных изображений. |

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

