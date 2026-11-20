---
title: "GridJsOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все параметры загрузки для GridJs"
type: docs
url: /ru/java/com.aspose.gridjs/gridjsoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridJsOptions
```

Представляет все параметры загрузки для GridJs
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridJsOptions()](#GridJsOptions--) |  |
## Поля

| Поле | Описание |
| --- | --- |
| [CacheImp](#CacheImp) | Пользовательская реализация для хранения кэша, если вы хотите хранить кэш в потоковом режиме, вам нужно установить и реализовать её. |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Указывает, использовать ли клиентский сгенерированный идентификатор вместо фактического идентификатора фигуры в операциях, связанных с редактированием |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Указывает, автоматически подгонять ли ширину столбцов при загрузке файла, значение по умолчанию — false. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Указывает, автоматически подгонять ли высоту строк при загрузке файла, значение по умолчанию — false. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Получает, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. |
| [getBaseRouteName()](#getBaseRouteName--) | Получает базовое имя маршрута URL для контроллера GridJs. Значение по умолчанию — GridJs2 |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Получает значение максимального столбца по умолчанию для пустого листа. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Получает значение максимальной строки по умолчанию для пустого листа. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Получает, включено ли рендеринг диаграмм на стороне клиента. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Получает каталог кэша для хранения файлов электронных таблиц. |
| [getFontFolders()](#getFontFolders--) | Получает папки шрифтов для шрифтов в отрисованных изображениях/фигурах |
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
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Указывает, автоматически подгонять ли ширину столбцов при загрузке файла, значение по умолчанию — false. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Указывает, автоматически подгонять ли высоту строк при загрузке файла, значение по умолчанию — false. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Устанавливает, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Устанавливает базовое имя маршрута URL для контроллера GridJs. Значение по умолчанию — GridJs2. |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Устанавливает, поддерживается ли совместное редактирование, значение по умолчанию — false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Устанавливает максимальное количество столбцов по умолчанию для пустого листа. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Устанавливает максимальное количество строк по умолчанию для пустого листа. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Устанавливает, включено ли клиентское рендеринг диаграмм. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Устанавливает каталог кэша для хранения файлов электронных таблиц. |
| [setFontFolders(String[] value)](#setFontFolders-java.lang.String---) | Устанавливает папки шрифтов для шрифтов в отрисованных изображениях/фигурах. |
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
### GridJsOptions() {#GridJsOptions--}
```
public GridJsOptions()
```


### CacheImp {#CacheImp}
```
public GridCacheForStream CacheImp
```


Пользовательская реализация хранения кэша. Если вы хотите сохранять кэш потоковым способом, необходимо установить и реализовать её. WebAssembly‑хост (IsWasm = true) должен установить её, поскольку для кэша по умолчанию нет локального диска.

### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public boolean RedactionUseClientGenerateId
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
public boolean getAutoFitColumnsOnLoad()
```


Указывает, автоматически подгонять ли ширину столбцов при загрузке файла, значение по умолчанию — false.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public boolean getAutoFitRowsHeightOnLoad()
```


Указывает, автоматически подгонять ли высоту строк при загрузке файла, значение по умолчанию — false.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public boolean getAutoOptimizeForLargeCells()
```


Определяет, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. При этом будут игнорироваться некоторые стили/границы для сокращения времени загрузки. Значение по умолчанию — true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public String getBaseRouteName()
```


Получает базовое имя маршрута URL для контроллера GridJs. Значение по умолчанию — GridJs2

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
public int getEmptySheetMaxCol()
```


Возвращает значение столбца по умолчанию (max) для пустого листа. Значение по умолчанию — 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public int getEmptySheetMaxRow()
```


Возвращает значение строки по умолчанию (max) для пустого листа. Значение по умолчанию — 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public boolean getEnableChartClientRendering()
```


Определяет, следует ли включить клиентскую отрисовку диаграмм. Если установить false, GridJs будет генерировать только изображения/формы диаграмм и не потребует клиентской отрисовки. Значение по умолчанию — true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public String getFileCacheDirectory()
```


Возвращает каталог кэша для хранения файлов электронных таблиц. Необходимо задать конкретный путь перед использованием GridJs.

**Returns:**
java.lang.String
### getFontFolders() {#getFontFolders--}
```
public String[] getFontFolders()
```


Получает папки шрифтов для шрифтов в отрисованных изображениях/фигурах

**Returns:**
java.lang.String[]
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public boolean getIgnoreEmptyContent()
```


Определяет, следует ли показывать максимальный диапазон, включающий данные, стили, объединённые ячейки и формы. Если последняя строка или столбец содержит ячейки без значения и формулы, но с пользовательским стилем, они не будут отображаться, когда значение true\u9286?\*. Значение по умолчанию — true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public boolean getIslimitShapeOrImage()
```


Получает, ограничивать ли общее количество отображаемых фигур/изображений в одном листе; если установлено в true, GridJs ограничит общее количество отображаемых фигур или изображений в одном листе значением MaxShapeOrImageCount, значение по умолчанию — true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public JsonCacheOptions getJsonCache()
```


Возвращает параметры конфигурации JSON‑кэша. Управляет поведением кэша в памяти (L1) и на диске (L2) для сгенерированного JSON книги.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public boolean getLazyLoading()
```


Получает, загружать ли только активный лист, значение по умолчанию — false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public int getMaxPdfSaveSeconds()
```


Возвращает максимальное время ожидания (секунды) при сохранении в PDF. Значение по умолчанию — 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public int getMaxShapeOrImageCount()
```


Возвращает общее количество отображаемых форм или изображений на активном листе; действует, когда IslimitShapeOrImage=true. Значение по умолчанию — 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public int getMaxShapeOrImageWidthOrHeight()
```


Возвращает максимальную ширину или высоту для формы или изображения; GridJs будет игнорировать формы или изображения, превышающие эти размеры. Действует, когда IslimitShapeOrImage=true. Значение по умолчанию — 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public int getMaxTotalShapeOrImageCount()
```


Возвращает общее количество отображаемых форм или изображений в книге; действует, когда IslimitShapeOrImage=true. Значение по умолчанию — 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public String getMessageTopic()
```


Получает назначения веб‑сокетов с префиксом "/topic". Значение по умолчанию — "/topic/opr". Используется только в совместном режиме.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public String getPictureCacheDirectory()
```


Возвращает каталог кэша для изображений (действует, когда GridJsWorkbook.CacheImp равно null). Путь по умолчанию — "\_piccache" внутри FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public boolean getSameImageDetecting()
```


Получает, проверять ли, имеют ли изображения одинаковый источник; значение по умолчанию — true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public boolean getSaveHtmlAsZip()
```


Получает, сохранять ли HTML‑файл как zip‑архив, значение по умолчанию — false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public boolean getShowChartSheet()
```


Определяет, следует ли показывать лист с диаграммами. Значение по умолчанию — false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public boolean getSkipInvisibleShapes()
```


Получает, следует ли пропускать фигуры, невидимые в UI, значение по умолчанию — true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public boolean getUsePrintArea()
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
public boolean isCollaborative()
```


Получает, поддерживается ли совместное редактирование, значение по умолчанию — false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public boolean isWasm()
```


Определяет, запускается ли GridJs внутри браузерного WebAssembly‑хоста вместо серверного процесса. При true не используется FileCacheDirectory / диск / путь interrupt‑thread, и кэш файлов должен поставляться из CacheImp, поскольку у браузерного хоста нет локального диска. Путь кода выбирается во время выполнения, поэтому один Aspose.Cells.GridJs.dll обслуживает оба хоста. Значение по умолчанию — false.

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
public void setAutoFitColumnsOnLoad(boolean value)
```


Указывает, автоматически подгонять ли ширину столбцов при загрузке файла, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public void setAutoFitRowsHeightOnLoad(boolean value)
```


Указывает, автоматически подгонять ли высоту строк при загрузке файла, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public void setAutoOptimizeForLargeCells(boolean value)
```


Устанавливает, следует ли автоматически оптимизировать производительность загрузки листа с большими ячейками. При этом будут игнорироваться некоторые стили/границы для сокращения времени загрузки. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public void setBaseRouteName(String value)
```


Устанавливает базовое имя маршрута URL для контроллера GridJs. Значение по умолчанию — GridJs2.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public void setCollaborative(boolean value)
```


Устанавливает, поддерживается ли совместное редактирование, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public void setEmptySheetMaxCol(int value)
```


Устанавливает значение столбца по умолчанию (max) для пустого листа. Значение по умолчанию — 15.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public void setEmptySheetMaxRow(int value)
```


Устанавливает значение строки по умолчанию (max) для пустого листа. Значение по умолчанию — 12.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public void setEnableChartClientRendering(boolean value)
```


Устанавливает, следует ли включить клиентскую отрисовку диаграмм. Если установить false, GridJs будет генерировать только изображения/формы диаграмм и не потребует клиентской отрисовки. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public void setFileCacheDirectory(String value)
```


Устанавливает каталог кэша для хранения файлов электронных таблиц. Необходимо задать конкретный путь перед использованием GridJs.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFontFolders(String[] value) {#setFontFolders-java.lang.String---}
```
public void setFontFolders(String[] value)
```


Устанавливает папки шрифтов для шрифтов в отрисованных изображениях/фигурах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String[] |  |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public void setIgnoreEmptyContent(boolean value)
```


Устанавливает, следует ли показывать максимальный диапазон, включающий данные, стили, объединённые ячейки и формы. Если последняя строка или столбец содержит ячейки без значения и формулы, но с пользовательским стилем, они не будут отображаться, когда значение true\u9286?\*. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public void setIslimitShapeOrImage(boolean value)
```


Устанавливает, ограничивать ли общее количество отображаемых фигур/изображений в одном листе; если установлено в true, GridJs ограничит общее количество отображаемых фигур или изображений в одном листе значением MaxShapeOrImageCount. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public void setJsonCache(JsonCacheOptions value)
```


Устанавливает параметры конфигурации кэша JSON. Управляет поведением кэша в памяти (L1) и на диске (L2) для сгенерированного JSON рабочей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public void setLazyLoading(boolean value)
```


Устанавливает, загружать ли только активный лист, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public void setMaxPdfSaveSeconds(int value)
```


Устанавливает максимальное время ожидания в секундах при сохранении в PDF. значение по умолчанию — 10.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public void setMaxShapeOrImageCount(int value)
```


Устанавливает общее количество отображаемых фигур или изображений на активном листе, применяется, когда IslimitShapeOrImage=true. значение по умолчанию — 100.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public void setMaxShapeOrImageWidthOrHeight(int value)
```


Устанавливает максимальную ширину или высоту для фигуры или изображения, GridJs будет игнорировать фигуру или изображение с шириной или высотой, превышающей это значение, применяется, когда IslimitShapeOrImage=true. значение по умолчанию — 10000.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public void setMaxTotalShapeOrImageCount(int value)
```


Устанавливает общее количество отображаемых фигур или изображений в рабочей книге, применяется, когда IslimitShapeOrImage=true. значение по умолчанию — 300.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public void setMessageTopic(String value)
```


Устанавливает назначения websocket с префиксом "/topic". Значение по умолчанию — "/topic/opr". Используется только в режиме совместного редактирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public void setPictureCacheDirectory(String value)
```


Устанавливает каталог кэша для изображений (это применяется, когда GridJsWorkbook.CacheImp равно null). путь по умолчанию будет "\_piccache" внутри FileCacheDirectory.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public void setSameImageDetecting(boolean value)
```


Устанавливает, проверять ли, имеют ли изображения одинаковый источник, значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public void setSaveHtmlAsZip(boolean value)
```


Устанавливает, сохранять ли HTML‑файл как zip‑архив, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public void setShowChartSheet(boolean value)
```


Устанавливает, показывать ли лист с диаграммами. значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public void setSkipInvisibleShapes(boolean value)
```


Устанавливает, следует ли пропускать формы, невидимые в UI, значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public void setUsePrintArea(boolean value)
```


Устанавливает, использовать ли PageSetup.PrintArea для диапазона отображения в UI, когда лист имеет настройку PageSetup для PrintArea. значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public void setWasm(boolean value)
```


Устанавливает, работает ли GridJs внутри хоста браузера WebAssembly вместо серверного процесса. Когда true, пути FileCacheDirectory / диск / прерывающий поток не используются, и кэш файлов должен поступать из CacheImp, поскольку у хоста браузера нет локального диска. Выбираются пути кода во время выполнения, поэтому один Aspose.Cells.GridJs.dll обслуживает оба хоста. значение по умолчанию — false.

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

