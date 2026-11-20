---
title: "GridJsWorkbook"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет основной класс входа для GridJs"
type: docs
url: /ru/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

Представляет основной класс входа для GridJs
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | Создаёт новый экземпляр GridJsWorkbook. |
## Поля

| Поле | Описание |
| --- | --- |
| [CacheImp](#CacheImp) | Пользовательская реализация для хранения кэша, если вы хотите хранить кэш в потоковом режиме, вам нужно установить и реализовать её. |
| [CalculateEngine](#CalculateEngine) | Пользовательская реализация движка вычислений, если вы хотите выполнять пользовательские расчёты, вам необходимо установить и реализовать её. |
| [PICTURE_TYPE](#PICTURE-TYPE) | константное значение типа изображения |
| [UpdateMonitor](#UpdateMonitor) | Получает/устанавливает монитор обновления для отслеживания операции обновления |
## Методы

| Метод | Описание |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | Применяет (выполняет) все операции редактирования в рабочей книге, удаляя формы редактирования и их целевые формы или очищая содержимое целевых диапазонов ячеек. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Проверяет, находится ли экземпляр рабочей книги в кэше памяти. Этот метод применяется только для режима совместной работы. |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | Копирует изображение или форму. |
| [dispose()](#dispose--) | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | Получает строку сообщения об ошибке в формате JSON. |
| [exportToJson()](#exportToJson--) | Получает строку JSON из данных в памяти, имя файла по умолчанию в JSON: book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | Получает строку JSON из данных в памяти, задает имя выходного файла в JSON. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | Получает строку JSON из данных в памяти, задает имя выходного файла в JSON. |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | Получает каталог кэша для хранения файлов электронных таблиц. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | Получает формат загрузки по расширению файла |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | Получить поток изображения. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | Получает URL изображения. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | Получает данные массива байтов встроенного OLE-объекта. |
| [getSettings()](#getSettings--) | Представляет настройки рабочей книги. |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e лист \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | Создаёт новый уникальный идентификатор для кэша файлов, используя заданное имя файла. |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | Импортирует файл Excel из потока файла с форматом загрузки. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | Импортирует файл Excel из потока файла с форматом загрузки и паролем открытия. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Импортирует файл Excel из пути к файлу. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | Импортирует файл Excel из потока файла. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | Импортирует файл Excel из потока файла с форматом загрузки и паролем открытия. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | Импортирует файл Excel из пути к файлу. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | Импортирует файл Excel из пути к файлу и пароля открытия. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | Импортирует файл Excel из строки в формате JSON. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Вставляет изображение в лист рабочей книги из потока файла или URL (необходимо предоставить либо поток файла, либо URL) или вставляет форму, когда p.type является одним из AutoShapeType. |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | Создаёт JSON из рабочей книги в памяти и записывает его в указанный поток. |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задаёт имя выходного файла в JSON и записывает её в поток. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор, и записывает её в поток. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | Применяет пакетное обновление к данным в памяти. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | Выполняет редактирование (замену) в файле Excel на основе массива операций JSON. |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | Сохраняет данные в памяти в файл кэша с указанным именем файла и также задаёт пароль открытия; формат сохранения определяется расширением имени файла. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Сохраняет данные в памяти в поток, исходя из формата исходного файла. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | Сохраняет данные в памяти по пути к файлу; если у файла есть расширение, формат сохранения определяется этим расширением. |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | Сохраняет данные в памяти в поток, формат сохранения — HTML. |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | Сохраняет данные в памяти по пути к файлу, формат сохранения — HTML. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | Сохраняет данные в памяти в поток, формат сохранения — PDF. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | Сохраняет данные памяти в указанный путь файла, формат сохранения — pdf. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | Сохраняет данные памяти в поток, формат сохранения — xlsx. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | Сохраняет данные памяти в указанный путь файла, формат сохранения — xlsx. |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | Устанавливает каталог кэша для хранения файлов электронных таблиц. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | Устанавливает URL действия получения базового изображения из контроллера. |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | Устанавливает InterruptMonitor для операции загрузки. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | Устанавливает InterruptMonitor для операции сохранения. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Представляет настройки рабочей книги. |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | Устанавливает прозрачность фигур редактирования в рабочей книге. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Перевести все строковые значения на целевой язык в листе. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Применяет операцию обновления. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


Создаёт новый экземпляр GridJsWorkbook.

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


Пользовательская реализация для хранения кэша, если вы хотите хранить кэш в потоковом режиме, вам нужно установить и реализовать её.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


Пользовательская реализация движка вычислений, если вы хотите выполнять пользовательские расчёты, вам необходимо установить и реализовать её.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


константное значение типа изображения

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


Получает/устанавливает монитор обновления для отслеживания операции обновления

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


Применяет (выполняет) все операции редактирования в рабочей книге, удаляя формы редактирования и их целевые формы или очищая содержимое целевых диапазонов ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| excelFilePath | java.lang.String | Путь к файлу Excel. |
| uid | java.lang.String | Уникальный идентификатор рабочей книги. Если null или пустой, новый uid будет сгенерирован на основе пути к файлу. |

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


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


Копирует изображение или форму.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| p | java.lang.String | JSON-строка для операции, указывающей расположение ячейки, содержит имя листа, номер верхней левой строки, номер верхнего левого столбца для изображения или фигуры\u951b\u5b94tc \{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\} |

**Returns:**
java.lang.String - JSON-строка нового скопированного изображения
### dispose() {#dispose--}
```
public void dispose()
```


Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов.

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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


Получает строку сообщения об ошибке в формате JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| msg | java.lang.String | Сообщение об ошибке. |

**Returns:**
java.lang.String - JSON-строка.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


Получает строку JSON из данных в памяти, имя файла по умолчанию в JSON: book1.

**Returns:**
java.lang.String - JSON-строка.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


Получает строку JSON из данных в памяти, задает имя выходного файла в JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filename | java.lang.String | Указывает имя файла в JSON. Если установить null, имя файла по умолчанию: book1.. |

**Returns:**
java.lang.String - JSON-строка.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


Получает строку JSON из данных в памяти, задает имя выходного файла в JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filename | java.lang.String | Указывает имя файла в JSON. Если установить null, имя файла по умолчанию: book1.. |

**Returns:**
java.lang.StringBuilder - JSON StringBuilder.
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filename | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


Получает каталог кэша для хранения файлов таблиц. Если не установлен, будет использовано статическое свойство из [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) или [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGridLoadFormat(String extension) {#getGridLoadFormat-java.lang.String-}
```
public static int getGridLoadFormat(String extension)
```


Получает формат загрузки по расширению файла

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| extension | java.lang.String | Расширение файла, обычно начинается с '.' . |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


Получить поток изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| picid | java.lang.String | Идентификатор изображения. |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - Поток изображения
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


Получает URL изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| picid | java.lang.String | Идентификатор изображения. |
| delimiter | java.lang.String | Разделитель строки. |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задает имя выходного файла в JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| filename | java.lang.String | Указывает имя файла в JSON. Если установить значение null, имя файла по умолчанию: book1. |

**Returns:**
java.lang.StringBuilder - JSON‑строка StringBuilder
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
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
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Представляет настройки рабочей книги.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e лист \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| sheetName | java.lang.String | \\u5bb8\\u30e4\\u7d94\\u741b\\u3125\\u6095\\u7ec9?\* @param fileName \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


Создаёт новый уникальный идентификатор для кэша файлов, используя заданное имя файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла. |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| fileName | java.lang.String | \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream filestream, int format) {#importExcelFile-java.io.InputStream-int-}
```
public void importExcelFile(InputStream filestream, int format)
```


Импортирует файл Excel из потока файла с форматом загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filestream | java.io.InputStream | Поток Excel‑файла. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). LoadFormat Excel‑файла. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


Импортирует файл Excel из потока файла с форматом загрузки и паролем открытия.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filestream | java.io.InputStream | Поток Excel‑файла. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). LoadFormat Excel‑файла. |
| пароль | java.lang.String | Открывающий пароль Excel‑файла. Значение может быть null, если пароль не установлен. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Импортирует файл Excel из пути к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Полный путь к файлу. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


Импортирует файл Excel из потока файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор кэша файла; если установить null, он будет сгенерирован автоматически. |
| filestream | java.io.InputStream | Поток Excel‑файла. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). LoadFormat Excel‑файла. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


Импортирует файл Excel из потока файла с форматом загрузки и паролем открытия.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор кэша файла; если установить null, он будет сгенерирован автоматически. |
| filestream | java.io.InputStream | Поток Excel‑файла. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). LoadFormat Excel‑файла. |
| пароль | java.lang.String | Открывающий пароль Excel‑файла. Значение может быть null, если пароль не установлен |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


Импортирует файл Excel из пути к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор кэша файла; если установить null, он будет сгенерирован автоматически. |
| fileName | java.lang.String | Полный путь к файлу. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


Импортирует файл Excel из пути к файлу и пароля открытия.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор кэша файла; если установить null, он будет сгенерирован автоматически. |
| fileName | java.lang.String | Полный путь к файлу. |
| пароль | java.lang.String | Открывающий пароль Excel‑файла. Значение может быть null, если пароль не установлен. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


Импортирует файл Excel из строки в формате JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| json | java.lang.String | Строка в формате JSON. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


Вставляет изображение в лист рабочей книги из потока файла или URL (необходимо предоставить либо поток файла, либо URL) или вставляет форму, когда p.type является одним из AutoShapeType.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор кэша файла |
| p | java.lang.String | Строка в формате JSON для операции, указывающей расположение ячейки, имя листа, верхнюю левую строку, верхний левый столбец для изображения\u951b\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | Поток файла изображения |
| imageUrl | java.lang.String | URL изображения |

**Returns:**
java.lang.String - Строка в формате JSON вставленного изображения
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


Генерировать JSON из Workbook в памяти и записать его в указанный поток. При необходимости кэшировать сгенерированный JSON для более быстрого последующего получения. Ключевые отличия от JsonToStreamByUid: - Этот метод использует текущее состояние Workbook в памяти (поле wb) - JsonToStreamByUid загружает Workbook из файлов кэша .cells на диске - Используйте этот метод, когда нужно экспортировать текущее состояние рабочей книги после изменений - Используйте JsonToStreamByUid, когда необходимо заново сгенерировать JSON из ранее кэшированного состояния файла Поведение кэширования (при наличии uid): - Проверяет кэш JSON перед генерацией (L1 память + L2 диск) - При промахе кэша генерирует JSON из Workbook в памяти - Сохраняет сгенерированный JSON в кэше для будущих запросов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Выходной поток для записи данных JSON |
| filename | java.lang.String | Указывает имя файла в JSON. Если установить значение null, имя файла по умолчанию: book1. |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| filename | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


Получает строку JSON файла из кэша, используя указанный уникальный идентификатор, задаёт имя выходного файла в JSON и записывает её в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток, который будет записан |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| filename | java.lang.String | Указывает имя файла в JSON. Если установить значение null, имя файла по умолчанию: book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| sheetName | java.lang.String | имя листа. |

**Returns:**
java.lang.StringBuilder - JSON‑строка StringBuilder
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


Получает строку JSON указанного листа в файле из кэша, используя указанный уникальный идентификатор, и записывает её в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток, который будет записан |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| sheetName | java.lang.String | имя листа. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


Применяет пакетное обновление к данным в памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| json | java.lang.String | Строка в формате JSON для обновления. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr) {#redactFile-java.lang.String-java.lang.String-java.lang.String---}
```
public void redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)
```


Выполняет редактирование (замену) в файле Excel на основе массива операций JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| excelFilePath | java.lang.String | Путь к Excel‑файлу, подлежащему редактированию. |
| uid | java.lang.String | Уникальный идентификатор рабочей книги. Если null или пустой, новый uid будет сгенерирован на основе пути к файлу. |
| arrayOfRedactionOpr | java.lang.String[] | Массив строк JSON, представляющих операции редактирования, которые необходимо применить. |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


Сохраняет данные в памяти в файл кэша с указанным именем файла и также задаёт пароль открытия; формат сохранения определяется расширением имени файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |
| filename | java.lang.String | Имя файла для сохранения. |
| пароль | java.lang.String | Пароль для открытия Excel‑файла. Значение может быть null, если пароль не установлен. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Сохраняет данные в памяти в поток, исходя из формата исходного файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток для сохранения. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


Сохраняет данные в памяти по пути к файлу; если у файла есть расширение, формат сохранения определяется этим расширением.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | java.lang.String | Путь к файлу для сохранения. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


Сохраняет данные в памяти в поток, формат сохранения — HTML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток для сохранения. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


Сохраняет данные в памяти по пути к файлу, формат сохранения — HTML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | java.lang.String | Путь к файлу для сохранения. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


Сохраняет данные в памяти в поток, формат сохранения — PDF.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток для сохранения. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


Сохраняет данные памяти в указанный путь файла, формат сохранения — pdf.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | java.lang.String | Путь к файлу для сохранения. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


Сохраняет данные памяти в поток, формат сохранения — xlsx.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток для сохранения. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


Сохраняет данные памяти в указанный путь файла, формат сохранения — xlsx.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | java.lang.String | Путь к файлу для сохранения. |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


Устанавливает каталог кэша для хранения файлов таблиц. Если не задан, будет использовано статическое свойство из [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) или [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


Устанавливает URL действия получения базового изображения из контроллера.

**Remarks**

Когда CacheImp равен null, необходимо установить это.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| baseImageURL | java.lang.String | URL действия получения базового изображения. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


Устанавливает InterruptMonitor для операции загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | Экземпляр InterruptMonitor. |
| calculateTimeoutMilliseconds | int | Тайм‑аут в миллисекундах для загрузки файла. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


Устанавливает InterruptMonitor для операции сохранения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | Экземпляр InterruptMonitor. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Представляет настройки рабочей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


Устанавливает прозрачность фигур редактирования в рабочей книге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| excelFilePath | java.lang.String | Путь к файлу Excel. |
| uid | java.lang.String | Уникальный идентификатор рабочей книги. Если null или пустой, новый uid будет сгенерирован на основе пути к файлу. |
| isTransparent | boolean | Если true, устанавливает прозрачность 0.89 (полупрозрачный); если false, устанавливает прозрачность 1 (полностью непрозрачный/невидимый). |

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
java.lang.String — строка в формате JSON результата обновления.
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

