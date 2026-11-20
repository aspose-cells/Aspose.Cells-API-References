---
title: "SpreadsheetLocker"
second_title: "Справочник API Aspose.Cells for Java"
description: "API с низким уровнем кода для блокировки файла таблицы."
type: docs
url: /ru/java/com.aspose.cells/spreadsheetlocker/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetLocker
```

API с низким уровнем кода для блокировки файла таблицы.

**Example**

```
         SpreadsheetLocker.process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-) | Блокирует файл таблицы с указанными настройками. |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-) | Блокирует файл таблицы с указанными настройками. |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-) | Блокирует файл таблицы с указанными настройками. |
| [process(String templateFile, String resultFile, String openPassword, String writePassword)](#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Блокирует файл таблицы с указанными настройками. |
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)
```


Блокирует файл таблицы с указанными настройками.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Параметры ввода и загрузки |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Параметры вывода и сохранения |
| provider | [AbstractLowCodeProtectionProvider](../../com.aspose.cells/abstractlowcodeprotectionprovider) | Реализация для предоставления настроек защиты |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)
```


Блокирует файл таблицы с указанными настройками.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Параметры ввода и загрузки |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Параметры вывода и сохранения |
| openPassword | java.lang.String | Пароль для шифрования файла |
| writePassword | java.lang.String | Пароль для защиты от изменения электронной таблицы |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)
```


Блокирует файл таблицы с указанными настройками.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Параметры ввода и загрузки |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Параметры вывода и сохранения |
| openPassword | java.lang.String | Пароль для шифрования файла |
| writePassword | java.lang.String | Пароль для защиты от изменения электронной таблицы |
| workbookPassword | java.lang.String | Пароль для защиты рабочей книги |
| workbookType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Тип защиты для защиты рабочей книги |

### process(String templateFile, String resultFile, String openPassword, String writePassword) {#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile, String openPassword, String writePassword)
```


Блокирует файл таблицы с указанными настройками.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | java.lang.String | Файл шаблона, который будет заблокирован |
| resultFile | java.lang.String | Полученный файл |
| openPassword | java.lang.String | Пароль для шифрования файла |
| writePassword | java.lang.String | Пароль для защиты от изменения электронной таблицы |

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

