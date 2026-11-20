---
title: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Справочник API Aspose.Cells for Java"
description: "Реализация, предоставляющая параметры сохранения, которые сохраняют разделённые части в файлы, а путь результирующего файла определяется с помощью заполнителей."
type: docs
url: /ru/java/com.aspose.cells/lowcodesaveoptionsproviderofplaceholders/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```

Реализация, предоставляющая параметры сохранения, которые сохраняют разделённые части в файлы, а путь результирующего файла определяется с помощью заполнителей.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | Создаёт экземпляр для предоставления параметров сохранения в соответствии с указанными шаблонами. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Освобождает ресурсы после обработки текущей части разделения. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Всегда ли добавлять индекс листа или его имя в путь файла. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Всегда ли добавлять индекс части разбиения в путь файла. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Получает параметры сохранения, из которых берутся настройки вывода для текущей части разделения. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Шаблон для создания экземпляра параметров сохранения в [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | Префикс для индекса листа. |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | Префикс для индекса листа. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Смещение индекса части разделения между тем, что используется в пути к файлу, и его фактическим значением([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Префикс для индекса части разделения. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Всегда ли добавлять индекс листа или его имя в путь файла. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Всегда ли добавлять индекс части разбиения в путь файла. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Шаблон для создания экземпляра параметров сохранения в [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | Префикс для индекса листа. |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | Префикс для индекса листа. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Смещение индекса части разделения между тем, что используется в пути к файлу, и его фактическим значением([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Префикс для индекса части разделения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```


Создаёт экземпляр для предоставления параметров сохранения в соответствии с указанными шаблонами.

**Remarks**

Поддерживаемые заполнители в шаблоне пути к файлу:

 *  $\{SheetIndex\}: will be replaced by the sheet index of the split part
 *  $\{SheetName\}: will be replaced by the sheet name of the split part
 *  $\{SplitPartIndex\}: will be replaced by the index of the split part
 *  $\{SheetIndexPrefix\}: will be replaced by
 *  $\{SheetNamePrefix\}: will be replaced by
 *  $\{SplitPartPrefix\}: will be replaced by

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pathTemplate | java.lang.String | Шаблон результирующего пути к файлу. |

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


Добавлять ли индекс листа или его имя в путь к файлу всегда. Значение по умолчанию — false, то есть когда лист единственный, индекс листа, имя и соответствующий префикс ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) не будут добавлены в путь к файлу.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Добавлять ли индекс части разделения в путь к файлу всегда. Значение по умолчанию — false, то есть когда часть разделения единственная, её индекс и соответствующий префикс ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) не будут добавлены в путь к файлу.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


Шаблон для создания экземпляра параметров сохранения в [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

Если шаблон был указан, созданный экземпляр скопирует все настройки из него и соответственно обновит выходной файл.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```


Префикс для индекса листа.

**Remarks**

Если листов только один и [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) имеет значение false, то этот префикс и индекс листа (или имя) не будут добавлены в результирующий путь к файлу.

**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```


Префикс для индекса листа.

**Remarks**

Если листов только один и [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) имеет значение false, то этот префикс и индекс листа (или имя) не будут добавлены в результирующий путь к файлу.

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

Если часть разделения единственная и [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) имеет значение false, то этот префикс и индекс части (0) не будут добавлены в результирующий путь к файлу.

**Returns:**
java.lang.String
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


Добавлять ли индекс листа или его имя в путь к файлу всегда. Значение по умолчанию — false, то есть когда лист единственный, индекс листа, имя и соответствующий префикс ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) не будут добавлены в путь к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Добавлять ли индекс части разделения в путь к файлу всегда. Значение по умолчанию — false, то есть когда часть разделения единственная, её индекс и соответствующий префикс ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) не будут добавлены в путь к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Шаблон для создания экземпляра параметров сохранения в [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

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

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```


Префикс для индекса листа.

**Remarks**

Если листов только один и [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) имеет значение false, то этот префикс и индекс листа (или имя) не будут добавлены в результирующий путь к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```


Префикс для индекса листа.

**Remarks**

Если листов только один и [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) имеет значение false, то этот префикс и индекс листа (или имя) не будут добавлены в результирующий путь к файлу.

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

Если часть разделения единственная и [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) имеет значение false, то этот префикс и индекс части (0) не будут добавлены в результирующий путь к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

