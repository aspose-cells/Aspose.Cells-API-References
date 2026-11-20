---
title: "GridJsService"
second_title: "Справочник API Aspose.Cells for Java"
description: "Предоставляет базовые API операций, используемые в действиях контроллера."
type: docs
url: /ru/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

Предоставляет базовые API операций, используемые в действиях контроллера.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | Конструктор по умолчанию для GridJsService |
## Методы

| Метод | Описание |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Применяет операцию добавления изображения из локального файла. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Применяет операцию добавления изображения из локального файла. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Проверяет, находится ли экземпляр рабочей книги в кэше памяти. Этот метод применяется только для режима совместной работы. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Очищает все записи кэша JSON (память и диск). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Очищает все записи кэша JSON, принадлежащие указанному уникальному идентификатору. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Применяет операцию копирования изображения. |
| [destroy()](#destroy--) | этот метод предназначен только для Java, он реализует метод destroy в DisposableBean, который будет вызван автоматически Spring после завершения запроса, фактически он вызовет метод Dispose |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Получает строку JSON для файла по указанному уникальному идентификатору. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Записывает строку JSON файла в поток. |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Записывает строку JSON файла в поток по указанному уникальному идентификатору. |
| [dispose()](#dispose--) | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Применяет операцию загрузки файла |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | Получить поток файла |
| [getSettings()](#getSettings--) | Представляет настройки рабочей книги. |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Получить поток изображения. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Получает URL изображения. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Записывает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор, в поток.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Получает данные массива байтов встроенного OLE-объекта. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Представляет настройки рабочей книги. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Перевести все строковые значения на целевой язык в листе. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Применяет операцию обновления. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


Конструктор по умолчанию для GridJsService

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
```


Применяет операцию добавления изображения из локального файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| p | java.lang.String | Параметр строки JSON |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| filestream | java.io.InputStream | Поток файла изображения |

**Returns:**
java.lang.String - Результат строки JSON
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Применяет операцию добавления изображения из локального файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| p | java.lang.String | Параметр строки JSON |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| filestream | java.io.InputStream | Поток файла изображения |
| imageurl | java.lang.String | Укажите URL изображения. |

**Returns:**
java.lang.String - Результат строки JSON
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public boolean checkInCacheForCollaborative(String uid)
```


Проверяет, находится ли экземпляр рабочей книги в кэше памяти. Этот метод применяется только для режима совместной работы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public void clearAllJsonCache()
```


Очищает все записи кэша JSON (память и диск).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


Очищает все записи кэша JSON, принадлежащие указанному уникальному идентификатору. Вызовите это после изменения исходного файла вне канала, чтобы следующий запрос сгенерировал JSON заново.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


Применяет операцию копирования изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| p | java.lang.String | Параметр строки JSON |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
java.lang.String - Результат строки JSON
### destroy() {#destroy--}
```
public void destroy()
```


этот метод предназначен только для Java, он реализует метод destroy в DisposableBean, который будет вызван автоматически Spring после завершения запроса, фактически он вызовет метод Dispose

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Получает строку JSON для файла по указанному уникальному идентификатору.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Полный путь к файлу |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


Записывает строку JSON файла в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток, который будет записан |
| filePath | java.lang.String | Полный путь к файлу |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Записывает строку JSON файла в поток по указанному уникальному идентификатору.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток, который будет записан |
| filePath | java.lang.String | Полный путь к файлу |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

### dispose() {#dispose--}
```
public void dispose()
```


Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов.

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
```


Применяет операцию загрузки файла

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| p | java.lang.String | Параметр JSON |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| filename | java.lang.String | Имя файла |

**Returns:**
java.lang.String - URL файла
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public InputStream getFile(String fileid)
```


Получить поток файла

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileid | java.lang.String | идентификатор файла |

**Returns:**
java.io.InputStream - Поток файла
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Представляет настройки рабочей книги.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public InputStream image(String uid, String picid)
```


Получить поток изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| picid | java.lang.String | Идентификатор изображения. |

**Returns:**
java.io.InputStream - Поток изображения
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public String imageUrl(String baseURL, String picid, String uid)
```


Получает URL изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| baseURL | java.lang.String | Базовый URL действия. |
| picid | java.lang.String | Идентификатор изображения. |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
java.lang.String - URL изображения
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String sheetName, String uid)
```


Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | имя листа. |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


Записывает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор, в поток..

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток, который будет записан |
| sheetName | java.lang.String | Имя листа. |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public String load(String uid, String filename)
```


Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| filename | java.lang.String | Указывает имя файла в JSON. Если установить значение null, имя файла по умолчанию: book1. |

**Returns:**
java.lang.String - JSON-строка
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] ole(String uid, String sheetname, int oleid, String label)
```


Получает данные массива байтов встроенного OLE-объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| sheetname | java.lang.String | Имя листа рабочей книги. |
| oleid | int | Идентификатор встроенного OLE-объекта. |
| label | java.lang.String | Отображаемая метка встроенного OLE-объекта. |

**Returns:**
byte[] - Данные массива байтов встроенного OLE-объекта.
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Представляет настройки рабочей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage) {#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-}
```
public String translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)
```


Перевести все строковые значения на целевой язык в листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| sheetName | java.lang.String | Имя листа |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | Переводчик, реализующий функцию translate |
| целевой язык | java.lang.String | Целевой язык |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Применяет операцию обновления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| p | java.lang.String | Строка в формате JSON операции обновления. |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

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

