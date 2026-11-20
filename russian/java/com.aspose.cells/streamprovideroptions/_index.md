---
title: "StreamProviderOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры потока."
type: docs
url: /ru/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

Представляет параметры потока.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | Инициализирует новый экземпляр класса [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
| [StreamProviderOptions()](#StreamProviderOptions--) | Инициализирует новый экземпляр класса [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | Пользовательский путь (URL), сохранённый в сгенерированном HTML‑файле для указанного источника. |
| [getDefaultPath()](#getDefaultPath--) | Путь по умолчанию (URL), сохранённый в сгенерированном HTML‑файле для указанного источника. |
| [getInputStream()](#getInputStream--) | Получает входной поток для получения данных. |
| [getResourceLoadingType()](#getResourceLoadingType--) | Получает тип загружаемого ресурса. |
| [getStream()](#getStream--) | Получает выходной поток для записи сохранённых данных. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | Пользовательский путь (URL), сохранённый в сгенерированном HTML‑файле для указанного источника. |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | Устанавливает входной поток для получения данных. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | Устанавливает тип загружаемого ресурса. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Устанавливает выходной поток для записи сохранённых данных. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


Инициализирует новый экземпляр класса [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). Тип для загрузки связанного ресурса. |
| defaultPath | java.lang.String | Путь по умолчанию. |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


Инициализирует новый экземпляр класса [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

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
### getCustomPath() {#getCustomPath--}
```
public String getCustomPath()
```


Пользовательский путь (URL), сохранённый в сгенерированном HTML‑файле для указанного источника. Если пользователь не задает его, будет использован DefaultPath. Например, данные листа будут сохранены пользователем в d:/sheet001.htm, URL, используемый в основном HTML‑файле, должен быть "d:/sheet001.htm" или другой допустимый относительный путь, доступный из основного HTML‑файла.

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


Путь по умолчанию (URL), сохранённый в сгенерированном HTML‑файле для указанного источника. Например, данные листа, сохранённые в xxx\_files/sheet001.htm, URL, используемый в основном HTML‑файле, должен выглядеть так: "src=\"xxx\_files/sheet001.htm\""

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


Получает входной поток для получения данных.

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


Получает тип загружаемого ресурса.

Смотрите [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


Получает выходной поток для записи сохранённых данных.

**Returns:**
java.io.OutputStream
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




### setCustomPath(String value) {#setCustomPath-java.lang.String-}
```
public void setCustomPath(String value)
```


Пользовательский путь (URL), сохранённый в сгенерированном HTML‑файле для указанного источника. Если пользователь не задает его, будет использован DefaultPath. Например, данные листа будут сохранены пользователем в d:/sheet001.htm, URL, используемый в основном HTML‑файле, должен быть "d:/sheet001.htm" или другой допустимый относительный путь, доступный из основного HTML‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


Устанавливает входной поток для получения данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


Устанавливает тип загружаемого ресурса.

Смотрите [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


Устанавливает выходной поток для записи сохранённых данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.io.OutputStream |  |

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

