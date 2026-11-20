---
title: "FileFormatUtil"
second_title: "Справочник API Aspose.Cells for Java"
description: "Предоставляет вспомогательные методы для преобразования перечислений форматов файлов в строки или расширения файлов и обратно."
type: docs
url: /ru/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

Предоставляет вспомогательные методы для преобразования перечислений форматов файлов в строки или расширения файлов и обратно.
## Методы

| Метод | Описание |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | Определяет и возвращает информацию о формате Excel, хранящегося в потоке. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | Определяет и возвращает информацию о формате Excel, хранящегося в потоке. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | Определяет и возвращает информацию о формате Excel, хранящегося в файле. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | Определяет и возвращает информацию о формате Excel, хранящегося в файле. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | Преобразует расширение имени файла в значение SaveFormat. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | Преобразование формата файла в формат сохранения. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | Возвращает true, если расширение .xlt, .xltX, .xltm, .ots. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | Преобразует перечисленное значение формата загрузки в расширение файла. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | Преобразует значение LoadFormat в значение SaveFormat, если это возможно. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | Преобразует перечисленное значение формата сохранения в расширение файла. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | Преобразует значение SaveFormat в значение LoadFormat, если это возможно. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | Определяет и возвращает информацию о формате Excel, хранящегося в потоке. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


Определяет и возвращает информацию о формате Excel, хранящегося в потоке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


Определяет и возвращает информацию о формате Excel, хранящегося в потоке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| пароль | java.lang.String | Пароль для зашифрованных файлов ooxml. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


Определяет и возвращает информацию о формате Excel, хранящегося в файле.

**Remarks**

Поддерживает только проверку некоторых файлов с магической подписью. Если магической подписи нет, мы не можем точно определить формат файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


Определяет и возвращает информацию о формате Excel, хранящегося в файле.

**Remarks**

Поддерживает только проверку некоторых файлов с магической подписью. Если магической подписи нет, мы не можем точно определить формат файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |
| пароль | java.lang.String | Пароль для зашифрованных файлов ooxml. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
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
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


Преобразует расширение имени файла в значение SaveFormat.

**Remarks**

Если расширение не может быть распознано, возвращает [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| extension | java.lang.String | Расширение файла. Может быть с точкой в начале или без неё. Регистронезависимо. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


Преобразование формата файла в формат сохранения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). Тип формата файла. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
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
### isTemplateFormat(String extension) {#isTemplateFormat-java.lang.String-}
```
public static boolean isTemplateFormat(String extension)
```


Возвращает true, если расширение .xlt, .xltX, .xltm, .ots.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


Преобразует перечисленное значение формата загрузки в расширение файла.

**Remarks**

Если его нельзя преобразовать, возвращает null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Формат загруженного файла. |

**Returns:**
java.lang.String - Возвращаемое расширение представляет собой строку в нижнем регистре с точкой в начале.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


Преобразует значение LoadFormat в значение SaveFormat, если это возможно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Формат загрузки. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). Формат сохранения.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveFormatToExtension(int format) {#saveFormatToExtension-int-}
```
public static String saveFormatToExtension(int format)
```


Преобразует перечисленное значение формата сохранения в расширение файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). Формат сохранения. |

**Returns:**
java.lang.String - Возвращаемое расширение представляет собой строку в нижнем регистре с точкой в начале.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


Преобразует значение SaveFormat в значение LoadFormat, если это возможно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Формат сохранения. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). Формат загрузки
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(InputStream stream, String password) {#verifyPassword-java.io.InputStream-java.lang.String-}
```
public static boolean verifyPassword(InputStream stream, String password)
```


Определяет и возвращает информацию о формате Excel, хранящегося в потоке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| пароль | java.lang.String | Пароль для зашифрованных файлов ooxml. |

**Returns:**
boolean - Возвращает, исправлен ли пароль.
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

