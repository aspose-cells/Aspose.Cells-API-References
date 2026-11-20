---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Справочник API Aspose.Cells for Java"
description: "Реализация, предоставляющая параметры сохранения, которые сохраняют разбитые части в файлы, а путь результирующего файла называется так, может содержать каталоги SheetIndex или SheetName SplitPartIndex."
type: docs
url: /ru/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

Реализация, предоставляющая параметры сохранения, которые сохраняют разбитые части в файлы, а путь результирующего файла называется так (может содержать каталоги): [getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(или SheetName)+[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Освобождает ресурсы после обработки текущей части разделения. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Всегда ли добавлять индекс листа или его имя в путь файла. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Всегда ли добавлять индекс части разбиения в путь файла. |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | Заголовочная часть (до добавления содержимого листа и части разбиения) пути файла. |
| [getPathTail()](#getPathTail--) | Конечная часть (после последовательных номеров) пути файла. |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Получает параметры сохранения, из которых берутся настройки вывода для текущей части разделения. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Шаблон для создания экземпляра параметров сохранения в [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetPrefix()](#getSheetPrefix--) | Префикс для индекса листа. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Смещение индекса части разделения между тем, что используется в пути к файлу, и его фактическим значением([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Префикс для индекса части разделения. |
| [getUseSheetName()](#getUseSheetName--) | Определяет, строит ли путь к файлу с использованием имени листа вместо индекса листа. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Всегда ли добавлять индекс листа или его имя в путь файла. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Всегда ли добавлять индекс части разбиения в путь файла. |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | Заголовочная часть (до добавления содержимого листа и части разбиения) пути файла. |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | Конечная часть (после последовательных номеров) пути файла. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Шаблон для создания экземпляра параметров сохранения в [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | Префикс для индекса листа. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Смещение индекса части разделения между тем, что используется в пути к файлу, и его фактическим значением([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Префикс для индекса части разделения. |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | Определяет, строит ли путь к файлу с использованием имени листа вместо индекса листа. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Освобождает ресурсы после обработки текущей части разделения.

**Remarks**

По умолчанию этот метод просто закрывает поток, указанный в [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--), напрямую (если параметры сохранения указали поток в качестве назначения). Пользователь может переопределить этот метод, чтобы управлять освобождением ресурсов в соответствии со своими требованиями и реализацией [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | параметры сохранения, используемые для текущей части разделения. |

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


Определяет, всегда ли добавлять индекс листа или его имя к пути к файлу. Значение по умолчанию — false, то есть когда существует только один лист, индекс листа (или имя) и соответствующий префикс не будут добавлены к пути к файлу.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Определяет, всегда ли добавлять индекс части разделения к пути к файлу. Значение по умолчанию — false, то есть когда существует только одна часть разделения, её индекс и соответствующий префикс не будут добавлены к пути к файлу.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


Заголовочная часть (до добавления содержимого листа и части разбиения) пути файла.

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


Заключительная часть (после последовательных номеров) пути к файлу. Должна включать расширение имени файла.

**Returns:**
java.lang.String
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Получает параметры сохранения, из которых берутся настройки вывода для текущей части разделения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


Шаблон для создания экземпляра параметров сохранения в [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Если шаблон был указан, созданный экземпляр скопирует все настройки из него и соответственно обновит выходной файл.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Действует только когда [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) равно false.

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


Префикс для индекса листа.

**Remarks**

Если существует только один лист и [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) равно false, то этот префикс и индекс листа (или имя) не будут добавлены к результирующему пути к файлу.

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


Смещение индекса части разделения между тем, что используется в пути к файлу, и его фактическим значением([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


Префикс для индекса части разделения.

**Remarks**

Если существует только одна часть разделения и [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) равно false, то этот префикс и индекс части разделения (0) не будут добавлены к результирующему пути к файлу.

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


Определяет, строит ли путь к файлу с использованием имени листа вместо индекса листа. Значение по умолчанию — false.

**Remarks**

Имя листа никогда не будет автоматически переименовано. Поэтому, устанавливая его в true, убедитесь, что нет специального имени листа, которое может привести к недопустимому пути к файлу или имени.

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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


Определяет, всегда ли добавлять индекс листа или его имя к пути к файлу. Значение по умолчанию — false, то есть когда существует только один лист, индекс листа (или имя) и соответствующий префикс не будут добавлены к пути к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Определяет, всегда ли добавлять индекс части разделения к пути к файлу. Значение по умолчанию — false, то есть когда существует только одна часть разделения, её индекс и соответствующий префикс не будут добавлены к пути к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


Заголовочная часть (до добавления содержимого листа и части разбиения) пути файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


Заключительная часть (после последовательных номеров) пути к файлу. Должна включать расширение имени файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Шаблон для создания экземпляра параметров сохранения в [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Если шаблон был указан, созданный экземпляр скопирует все настройки из него и соответственно обновит выходной файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Действует только когда [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) равно false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


Префикс для индекса листа.

**Remarks**

Если существует только один лист и [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) равно false, то этот префикс и индекс листа (или имя) не будут добавлены к результирующему пути к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


Смещение индекса части разделения между тем, что используется в пути к файлу, и его фактическим значением([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


Префикс для индекса части разделения.

**Remarks**

Если существует только одна часть разделения и [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) равно false, то этот префикс и индекс части разделения (0) не будут добавлены к результирующему пути к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


Определяет, строит ли путь к файлу с использованием имени листа вместо индекса листа. Значение по умолчанию — false.

**Remarks**

Имя листа никогда не будет автоматически переименовано. Поэтому, устанавливая его в true, убедитесь, что нет специального имени листа, которое может привести к недопустимому пути к файлу или имени.

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

