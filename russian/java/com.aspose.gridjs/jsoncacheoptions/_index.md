---
title: "JsonCacheOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Параметры конфигурации кэширования JSON в GridJs."
type: docs
url: /ru/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

Параметры конфигурации кэширования JSON в GridJs. Управляет поведением кэша в памяти (L1) и на диске (L2).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | Возвращает, сжимать ли кэш диска с помощью Gzip (по умолчанию: true). |
| [getDiskPath()](#getDiskPath--) | Возвращает путь к каталогу кэша диска. |
| [getDiskTtl()](#getDiskTtl--) | Возвращает TTL кэша диска в минутах (по умолчанию: 1440). |
| [getEnable()](#getEnable--) | Возвращает, включено ли кэширование JSON для более быстрого отклика. |
| [getEnableDisk()](#getEnableDisk--) | Возвращает, включён ли кэш диска (по умолчанию: true). |
| [getImplementation()](#getImplementation--) | Возвращает пользовательскую реализацию кэша JSON. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | Возвращает максимальный размер кэша диска в МБ (по умолчанию: 500 МБ). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | Возвращает максимальное количество записей в кэше памяти (по умолчанию: 1000). |
| [getMemoryTtl()](#getMemoryTtl--) | Возвращает TTL кэша памяти в минутах (по умолчанию: 60). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | Устанавливает, сжимать ли кэш диска с помощью Gzip (по умолчанию: true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | Устанавливает путь к каталогу кэша диска. |
| [setDiskTtl(long value)](#setDiskTtl-long-) | Устанавливает TTL кэша диска в минутах (по умолчанию: 1440). |
| [setEnable(boolean value)](#setEnable-boolean-) | Устанавливает, включить ли кэширование JSON для более быстрого отклика. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | Устанавливает, включить ли кэш диска (по умолчанию: true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | Устанавливает пользовательскую реализацию кэша JSON. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | Устанавливает максимальный размер дискового кэша в МБ (по умолчанию: 500 МБ). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | Устанавливает максимальное количество записей в кэше памяти (по умолчанию: 1000). |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | Устанавливает TTL для кэша памяти в минутах (по умолчанию: 60). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonCacheOptions() {#JsonCacheOptions--}
```
public JsonCacheOptions()
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
### getCompressDisk() {#getCompressDisk--}
```
public boolean getCompressDisk()
```


Получает, следует ли сжимать дисковый кэш с помощью Gzip (по умолчанию: true). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


Получает путь к каталогу дискового кэша. Вступает в силу, когда Enable = true и используется кэш по умолчанию. По умолчанию: [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


Получает TTL для дискового кэша в минутах (по умолчанию: 1440). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


Получает, включено ли кэширование JSON для более быстрого отклика. Когда включено, GridJs будет кэшировать сгенерированный JSON и повторно использовать его для последующих запросов. Значение по умолчанию — false. Примечание: необходимо установить Implementation для использования пользовательского хранилища кэша.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


Получает, включён ли дисковый кэш (по умолчанию: true). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


Получает пользовательскую реализацию кэша JSON. Если не задано, GridJs будет использовать кэш памяти + диска по умолчанию.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


Получает максимальный размер дискового кэша в МБ (по умолчанию: 500 МБ). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


Получает максимальное количество записей в кэше памяти (по умолчанию: 1000). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


Получает TTL для кэша памяти в минутах (по умолчанию: 60). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Returns:**
long
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




### setCompressDisk(boolean value) {#setCompressDisk-boolean-}
```
public void setCompressDisk(boolean value)
```


Устанавливает, следует ли сжимать дисковый кэш с помощью Gzip (по умолчанию: true). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


Устанавливает путь к каталогу дискового кэша. Вступает в силу, когда Enable = true и используется кэш по умолчанию. По умолчанию: [FileCacheDirectory]/json\_cache

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


Устанавливает TTL для дискового кэша в минутах (по умолчанию: 1440). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


Устанавливает, включить ли кэширование JSON для более быстрого отклика. Когда включено, GridJs будет кэшировать сгенерированный JSON и повторно использовать его для последующих запросов. Значение по умолчанию — false. Примечание: необходимо установить Implementation для использования пользовательского хранилища кэша.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


Устанавливает, включён ли дисковый кэш (по умолчанию: true). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


Устанавливает пользовательскую реализацию кэша JSON. Если не задано, GridJs будет использовать кэш памяти + диска по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


Устанавливает максимальный размер дискового кэша в МБ (по умолчанию: 500 МБ). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


Устанавливает максимальное количество записей в кэше памяти (по умолчанию: 1000). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


Устанавливает TTL для кэша памяти в минутах (по умолчанию: 60). Вступает в силу, когда Enable = true и используется кэш по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | long |  |

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

