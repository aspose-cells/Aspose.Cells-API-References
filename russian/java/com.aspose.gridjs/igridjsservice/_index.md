---
title: "IGridJsService"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс базовых API операций, используемых в действиях контроллера."
type: docs
url: /ru/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

Представляет интерфейс базовых API операций, используемых в действиях контроллера.
## Методы

| Метод | Описание |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Применяет операцию добавления изображения из локального файла. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Применяет операцию добавления изображения из удалённого URL. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Проверяет, находится ли экземпляр рабочей книги в кэше памяти. Этот метод применяется только для режима совместной работы. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Очищает все записи кэша JSON (память и диск). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Очищает все записи кэша JSON, принадлежащие указанному уникальному идентификатору. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Применяет операцию копирования изображения. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Получает строку JSON для файла по указанному уникальному идентификатору. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Записать JSON-строку книги в поток |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Записывает строку JSON файла в поток по указанному уникальному идентификатору. |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Применяет операцию загрузки файла |
| [getFile(String fileid)](#getFile-java.lang.String-) | Получить поток файла |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Получить поток изображения. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Получает URL изображения. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Записывает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор, в поток.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Получает данные массива байтов встроенного OLE-объекта. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Применяет операцию обновления. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
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
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Применяет операцию добавления изображения из удалённого URL.

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
public abstract boolean checkInCacheForCollaborative(String uid)
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
public abstract void clearAllJsonCache()
```


Очищает все записи кэша JSON (память и диск).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


Очищает все записи кэша JSON, принадлежащие указанному уникальному идентификатору. Вызовите это после изменения исходного файла вне канала, чтобы следующий запрос сгенерировал JSON заново.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


Применяет операцию копирования изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| p | java.lang.String | Параметр строки JSON |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
java.lang.String - Результат строки JSON
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Получает строку JSON для файла по указанному уникальному идентификатору.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


Записать JSON-строку книги в поток

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток, который будет записан |
| filePath | java.lang.String | Путь к файлу |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Записывает строку JSON файла в поток по указанному уникальному идентификатору.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток, который будет записан |
| filePath | java.lang.String | Путь к файлу |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


Получить поток файла

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileid | java.lang.String | идентификатор файла |

**Returns:**
java.io.InputStream - Поток файла
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
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
public abstract String imageUrl(String baseURL, String picid, String uid)
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
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public abstract String load(String uid, String filename)
```


Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| filename | java.lang.String | Указывает имя файла в JSON. Если установить значение null, имя файла по умолчанию: book1. |

**Returns:**
java.lang.String - JSON-строка
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
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
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


Применяет операцию обновления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| p | java.lang.String | Строка в формате JSON операции обновления. |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
java.lang.String
