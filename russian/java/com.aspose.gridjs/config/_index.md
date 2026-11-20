---
title: "Конфигурация"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все статические настройки для GridJs"
type: docs
url: /ru/java/com.aspose.gridjs/config/
---

**Inheritance:**
java.lang.Object
```
public class Config
```

Представляет все статические настройки для GridJs
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Config()](#Config--) |  |
## Поля

| Поле | Описание |
| --- | --- |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Указывает, использовать ли клиентский сгенерированный идентификатор вместо фактического идентификатора фигуры в операциях, связанных с редактированием |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Указывает, следует ли автоматически подгонять ширину столбцов при загрузке файла. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Указывает, следует ли автоматически подгонять высоту строк при загрузке файла. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Получает, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. |
| [getBaseRouteName()](#getBaseRouteName--) | Получает базовое имя маршрута для URL контроллера GridJs. значение по умолчанию — "/GridJs2". |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Получает значение максимального столбца по умолчанию для пустого листа. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Получает значение максимальной строки по умолчанию для пустого листа. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Получает, включено ли рендеринг диаграмм на стороне клиента. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Получает каталог кэша для хранения файлов электронных таблиц. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | Получает, отображать ли максимальный диапазон, включающий данные, стиль, объединённые ячейки и фигуры. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | Получает, ограничивать ли общее количество отображаемых фигур/изображений в одном листе; если установлено в true, GridJs ограничит общее количество отображаемых фигур или изображений в одном листе значением MaxShapeOrImageCount, значение по умолчанию — true. |
| [getJsonCache()](#getJsonCache--) | Получает параметры конфигурации кэша JSON. |
| [getLazyLoading()](#getLazyLoading--) | Получает, загружать ли только активный лист, значение по умолчанию — false. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | Получает максимальное время ожидания в секундах при сохранении в PDF. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | Получает общее количество отображаемых фигур или изображений в активном листе, действует, когда IslimitShapeOrImage=true. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | Получает максимальную ширину или высоту для фигуры или изображения; GridJs будет игнорировать фигуру или изображение с шириной или высотой, превышающей это значение, действует, когда IslimitShapeOrImage=true. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | Получает общее количество отображаемых фигур или изображений в рабочей книге, действует, когда IslimitShapeOrImage=true. |
| [getMessageTopic()](#getMessageTopic--) | Получает назначения веб‑сокетов с префиксом "/topic". Значение по умолчанию — "/topic/opr". Используется только в совместном режиме. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | Получает каталог кэша для изображений. |
| [getSameImageDetecting()](#getSameImageDetecting--) | Получает, проверять ли, имеют ли изображения одинаковый источник; значение по умолчанию — true. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | Получает, сохранять ли HTML‑файл как zip‑архив, значение по умолчанию — false. |
| [getShowChartSheet()](#getShowChartSheet--) | Получает, отображать ли лист с диаграммами. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | Получает, следует ли пропускать фигуры, невидимые в UI, значение по умолчанию — true. |
| [getUsePrintArea()](#getUsePrintArea--) | Получает, использовать ли PageSetup.PrintArea для диапазона отображения UI, когда лист имеет настройку PageSetup для PrintArea. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | Получает, поддерживается ли совместное редактирование, значение по умолчанию — false. |
| [isWasm()](#isWasm--) | Получает, работает ли GridJs внутри WebAssembly‑хоста в браузере вместо серверного процесса. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Указывает, следует ли автоматически подгонять ширину столбцов при загрузке файла. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Указывает, следует ли автоматически подгонять высоту строк при загрузке файла. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Устанавливает, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Устанавливает базовое имя маршрута для URL контроллера GridJs. значение по умолчанию — "/GridJs2". |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Устанавливает, поддерживается ли совместное редактирование, значение по умолчанию — false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Устанавливает максимальное количество столбцов по умолчанию для пустого листа. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Устанавливает максимальное количество строк по умолчанию для пустого листа. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Устанавливает, включено ли клиентское рендеринг диаграмм. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Устанавливает каталог кэша для хранения файлов электронных таблиц. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Устанавливает папку шрифтов |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Устанавливает папки шрифтов |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | Устанавливает, отображать ли максимальный диапазон, включающий данные, стиль, объединённые ячейки и фигуры. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | Устанавливает, ограничивать ли общее количество отображаемых фигур/изображений в одном листе; если установлено в true, GridJs ограничит общее количество отображаемых фигур или изображений в одном листе значением MaxShapeOrImageCount. Значение по умолчанию — true. |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | Устанавливает параметры конфигурации кэша JSON. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | Устанавливает, загружать ли только активный лист, значение по умолчанию — false. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | Устанавливает максимальное время ожидания в секундах при сохранении в PDF. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | Устанавливает общее количество отображаемых фигур или изображений в активном листе, действует, когда IslimitShapeOrImage=true. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | Устанавливает максимальную ширину или высоту для фигуры или изображения; GridJs будет игнорировать фигуру или изображение, у которых ширина или высота превышают это значение, действует, когда IslimitShapeOrImage=true. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | Устанавливает общее количество отображаемых фигур или изображений в рабочей книге, действует, когда IslimitShapeOrImage=true. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | Устанавливает назначения websocket с префиксом "/topic". Значение по умолчанию — "/topic/opr". Используется только в режиме совместного редактирования. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | Устанавливает каталог кэша для изображений. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | Устанавливает, проверять ли, имеют ли изображения одинаковый источник, значение по умолчанию — true. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | Устанавливает, сохранять ли HTML‑файл как zip‑архив, значение по умолчанию — false. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | Устанавливает, отображать ли лист с диаграммами. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | Устанавливает, следует ли пропускать формы, невидимые в UI, значение по умолчанию — true. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | Устанавливает, следует ли использовать PageSetup.PrintArea для диапазона отображения в UI, когда лист имеет настройку PageSetup для PrintArea. |
| [setWasm(boolean value)](#setWasm-boolean-) | Устанавливает, следует ли запускать GridJs внутри браузерного WebAssembly‑хоста вместо серверного процесса. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Config() {#Config--}
```
public Config()
```


### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public static boolean RedactionUseClientGenerateId
```


Указывает, использовать ли клиентский сгенерированный идентификатор вместо фактического идентификатора фигуры в операциях, связанных с редактированием

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public static boolean getAutoFitColumnsOnLoad()
```


Указывает, следует ли автоматически подгонять ширину столбцов при загрузке файла. Значение по умолчанию — `false`. Предупреждение: установка значения `true` выполнит операцию автоматической подгонки всех столбцов после загрузки, что может заметно повлиять на производительность.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public static boolean getAutoFitRowsHeightOnLoad()
```


Указывает, следует ли автоматически подгонять высоту строк при загрузке файла. Значение по умолчанию — `false`. Предупреждение: установка значения `true` выполнит операцию автоматической подгонки всех строк после загрузки, что может заметно повлиять на производительность.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```


Определяет, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. При этом будут игнорироваться некоторые стили/границы для сокращения времени загрузки. Значение по умолчанию — true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```


Получает базовое имя маршрута для URL контроллера GridJs. значение по умолчанию — "/GridJs2".

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmptySheetMaxCol() {#getEmptySheetMaxCol--}
```
public static int getEmptySheetMaxCol()
```


Возвращает значение столбца по умолчанию (max) для пустого листа. Значение по умолчанию — 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```


Возвращает значение строки по умолчанию (max) для пустого листа. Значение по умолчанию — 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public static boolean getEnableChartClientRendering()
```


Получает, включена ли отрисовка диаграмм на клиенте. Если установить false, GridJs будет использовать только серверно‑сгенерированные изображения/формы диаграмм. значение по умолчанию — true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```


Возвращает каталог кэша для хранения файлов электронных таблиц. Необходимо задать конкретный путь перед использованием GridJs.

**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```


Определяет, следует ли показывать максимальный диапазон, включающий данные, стили, объединённые ячейки и формы. Если последняя строка или столбец содержит ячейки без значения и формулы, но с пользовательским стилем, они не будут отображаться, когда значение true\u9286?\*. Значение по умолчанию — true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```


Получает, ограничивать ли общее количество отображаемых фигур/изображений в одном листе; если установлено в true, GridJs ограничит общее количество отображаемых фигур или изображений в одном листе значением MaxShapeOrImageCount, значение по умолчанию — true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public static JsonCacheOptions getJsonCache()
```


Возвращает параметры конфигурации JSON‑кэша. Управляет поведением кэша в памяти (L1) и на диске (L2) для сгенерированного JSON книги.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```


Получает, загружать ли только активный лист, значение по умолчанию — false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```


Возвращает максимальное время ожидания (секунды) при сохранении в PDF. Значение по умолчанию — 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```


Возвращает общее количество отображаемых форм или изображений на активном листе; действует, когда IslimitShapeOrImage=true. Значение по умолчанию — 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```


Возвращает максимальную ширину или высоту для формы или изображения; GridJs будет игнорировать формы или изображения, превышающие эти размеры. Действует, когда IslimitShapeOrImage=true. Значение по умолчанию — 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```


Возвращает общее количество отображаемых форм или изображений в книге; действует, когда IslimitShapeOrImage=true. Значение по умолчанию — 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```


Получает назначения веб‑сокетов с префиксом "/topic". Значение по умолчанию — "/topic/opr". Используется только в совместном режиме.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```


Возвращает каталог кэша для изображений (действует, когда GridJsWorkbook.CacheImp равно null). Путь по умолчанию — "\_piccache" внутри FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```


Получает, проверять ли, имеют ли изображения одинаковый источник; значение по умолчанию — true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```


Получает, сохранять ли HTML‑файл как zip‑архив, значение по умолчанию — false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```


Определяет, следует ли показывать лист с диаграммами. Значение по умолчанию — false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```


Получает, следует ли пропускать фигуры, невидимые в UI, значение по умолчанию — true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
```


Определяет, следует ли использовать PageSetup.PrintArea для диапазона отображения в UI, когда лист имеет настройку PageSetup для PrintArea. Значение по умолчанию — false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollaborative() {#isCollaborative--}
```
public static boolean isCollaborative()
```


Получает, поддерживается ли совместное редактирование, значение по умолчанию — false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public static boolean isWasm()
```


Получает, работает ли GridJs внутри WebAssembly‑хоста в браузере вместо серверного процесса. Когда true, путь FileCacheDirectory / диск / прерывающий поток не используется, и кэш файлов должен поступать из GridJsOptions.CacheImp. GridJsOptions.IsWasm задаёт это при создании сервиса GridJs, поэтому один Aspose.Cells.GridJs.dll обслуживает оба хоста. значение по умолчанию — false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFitColumnsOnLoad(boolean value) {#setAutoFitColumnsOnLoad-boolean-}
```
public static void setAutoFitColumnsOnLoad(boolean value)
```


Указывает, следует ли автоматически подгонять ширину столбцов при загрузке файла. Значение по умолчанию — `false`. Предупреждение: установка значения `true` выполнит операцию автоматической подгонки всех столбцов после загрузки, что может заметно повлиять на производительность.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public static void setAutoFitRowsHeightOnLoad(boolean value)
```


Указывает, следует ли автоматически подгонять высоту строк при загрузке файла. Значение по умолчанию — `false`. Предупреждение: установка значения `true` выполнит операцию автоматической подгонки всех строк после загрузки, что может заметно повлиять на производительность.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```


Устанавливает, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. При этом будут игнорироваться некоторые стили/границы для сокращения времени загрузки. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```


Устанавливает базовое имя маршрута для URL контроллера GridJs. значение по умолчанию — "/GridJs2".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```


Устанавливает, поддерживается ли совместное редактирование, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```


Устанавливает значение столбца по умолчанию (max) для пустого листа. Значение по умолчанию — 15.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```


Устанавливает значение строки по умолчанию (max) для пустого листа. Значение по умолчанию — 12.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public static void setEnableChartClientRendering(boolean value)
```


Устанавливает, включена ли отрисовка диаграмм на клиенте. Если установить false, GridJs будет использовать только серверно‑сгенерированные изображения/формы диаграмм. значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```


Устанавливает каталог кэша для хранения файлов электронных таблиц. Необходимо задать конкретный путь перед использованием GridJs.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Устанавливает папку шрифтов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolder | java.lang.String | Папка, содержащая TrueType шрифты. |
| recursive | boolean | Определяет, сканировать ли подпапки. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Устанавливает папки шрифтов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Папки, содержащие TrueType шрифты. |
| recursive | boolean | Определяет, сканировать ли подпапки. |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```


Устанавливает, следует ли показывать максимальный диапазон, включающий данные, стили, объединённые ячейки и формы. Если последняя строка или столбец содержит ячейки без значения и формулы, но с пользовательским стилем, они не будут отображаться, когда значение true\u9286?\*. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```


Устанавливает, ограничивать ли общее количество отображаемых фигур/изображений в одном листе; если установлено в true, GridJs ограничит общее количество отображаемых фигур или изображений в одном листе значением MaxShapeOrImageCount. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public static void setJsonCache(JsonCacheOptions value)
```


Устанавливает параметры конфигурации кэша JSON. Управляет поведением кэша в памяти (L1) и на диске (L2) для сгенерированного JSON рабочей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```


Устанавливает, загружать ли только активный лист, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```


Устанавливает максимальное время ожидания в секундах при сохранении в PDF. значение по умолчанию — 10.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```


Устанавливает общее количество отображаемых фигур или изображений на активном листе, применяется, когда IslimitShapeOrImage=true. значение по умолчанию — 100.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```


Устанавливает максимальную ширину или высоту для фигуры или изображения, GridJs будет игнорировать фигуру или изображение с шириной или высотой, превышающей это значение, применяется, когда IslimitShapeOrImage=true. значение по умолчанию — 10000.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```


Устанавливает общее количество отображаемых фигур или изображений в рабочей книге, применяется, когда IslimitShapeOrImage=true. значение по умолчанию — 300.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```


Устанавливает назначения websocket с префиксом "/topic". Значение по умолчанию — "/topic/opr". Используется только в режиме совместного редактирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```


Устанавливает каталог кэша для изображений (это применяется, когда GridJsWorkbook.CacheImp равно null). путь по умолчанию будет "\_piccache" внутри FileCacheDirectory.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```


Устанавливает, проверять ли, имеют ли изображения одинаковый источник, значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```


Устанавливает, сохранять ли HTML‑файл как zip‑архив, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```


Устанавливает, показывать ли лист с диаграммами. значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```


Устанавливает, следует ли пропускать формы, невидимые в UI, значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```


Устанавливает, использовать ли PageSetup.PrintArea для диапазона отображения в UI, когда лист имеет настройку PageSetup для PrintArea. значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public static void setWasm(boolean value)
```


Устанавливает, работает ли GridJs внутри WebAssembly‑хоста в браузере вместо серверного процесса. Когда true, путь FileCacheDirectory / диск / прерывающий поток не используется, и кэш файлов должен поступать из GridJsOptions.CacheImp. GridJsOptions.IsWasm задаёт это при создании сервиса GridJs, поэтому один Aspose.Cells.GridJs.dll обслуживает оба хоста. значение по умолчанию — false.

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

