---
title: "GridHtmlSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры сохранения html‑файла."
type: docs
url: /ru/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

Представляет параметры сохранения html‑файла.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | Создаёт параметры для сохранения HTML‑файла. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | Создаёт параметры для сохранения HTM‑файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Каталог, в который будут сохраняться вложенные файлы. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Укажите префикс Url прикреплённых файлов, таких как изображения, в HTML‑файле. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Папка кэшированных файлов используется для хранения некоторых больших данных. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Очищать книгу после сохранения файла. |
| [getCreateDirectory()](#getCreateDirectory--) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [getDefaultFontName()](#getDefaultFontName--) | Укажите имя шрифта по умолчанию для экспорта HTML, шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null. |
| [getEncoding()](#getEncoding--) | Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Указывает, экспортировать ли всю книгу в html‑файл. |
| [getExportArea()](#getExportArea--) | Получает экспортируемую CellArea текущего активного Worksheet. |
| [getExportGridLines()](#getExportGridLines--) | Указывает, экспортировать ли сетку. Значение по умолчанию — false. |
| [getExportHeadings()](#getExportHeadings--) | Указывает, экспортировать ли заголовки при сохранении файла в html. Значение по умолчанию — false. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Указывает, сохранять ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Указывает, экспортировать ли только область печати в HTML‑файл. |
| [getExportSingleTab()](#getExportSingleTab--) | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. |
| [getMergeAreas()](#getMergeAreas--) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [getPageTitle()](#getPageTitle--) | Заголовок html‑страницы. |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Разбирать html‑тег в ячейке, например |

, как значение ячейки, или как html‑тег, значение по умолчанию — true |
| [getPresentationPreference()](#getPresentationPreference--) | Указывает, предпочтителен ли html или mht файл для представления. Значение по умолчанию — false. Если вы хотите получить более красивое представление, установите значение в true. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Указывает, обновляются ли данные кэша диаграммы |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохраняемого файла. |
| [getSortNames()](#getSortNames--) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | Указывает, экспортировать ли комментарии при сохранении файла в html; значение по умолчанию — false. |
| [isFullPathLink()](#isFullPathLink--) | Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Каталог, в который будут сохраняться вложенные файлы. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Укажите префикс Url прикреплённых файлов, таких как изображения, в HTML‑файле. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Папка кэшированных файлов используется для хранения некоторых больших данных. |
| [setClearData(boolean value)](#setClearData-boolean-) | Очищать книгу после сохранения файла. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Укажите имя шрифта по умолчанию для экспорта HTML, шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Указывает, экспортировать ли всю книгу в html‑файл. |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | Устанавливает экспортируемую CellArea текущего активного Worksheet. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Указывает, экспортировать ли комментарии при сохранении файла в html; значение по умолчанию — false. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Указывает, экспортировать ли сетку. Значение по умолчанию — false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Указывает, экспортировать ли заголовки при сохранении файла в html. Значение по умолчанию — false. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Указывает, сохранять ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Указывает, экспортировать ли только область печати в HTML‑файл. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Заголовок html‑страницы. |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Разбирать html‑тег в ячейке, например |

, как значение ячейки, или как html‑тег, значение по умолчанию — true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Указывает, предпочтителен ли html или mht файл для представления. Значение по умолчанию — false. Если вы хотите получить более красивое представление, установите значение в true. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Указывает, обновляются ли данные кэша диаграммы |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


Создаёт параметры для сохранения HTML‑файла.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


Создаёт параметры для сохранения HTM‑файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Формат сохраняемого файла. |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в поток html.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Укажите префикс Url вложенных файлов, например изображений в html‑файле. Только при сохранении в поток html.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Папка кэшированных файлов используется для хранения некоторых больших данных.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Очищать книгу после сохранения файла.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Укажите имя шрифта по умолчанию для экспорта HTML, шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Указывает, экспортировать ли всю книгу в html‑файл.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


Получает экспортируемую CellArea текущего активного листа Worksheet. Если задать этот атрибут, область печати текущего активного листа Worksheet будет опущена. При сохранении файла в html будет экспортирована только указанная область.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Указывает, экспортировать ли сетку. Значение по умолчанию — false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Указывает, экспортировать ли заголовки при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, оставьте значение по умолчанию.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Указывает, сохранять ли изображения в формате Base64 в HTML, MHTML или EPUB.

**Remarks**

Когда это свойство установлено в true, данные изображения экспортируются непосредственно в элементы img, и отдельные файлы не создаются.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Указывает, экспортировать ли только область печати в html‑файл. Значение по умолчанию — false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Заголовок html‑страницы. Используется только при сохранении в поток html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Разбирать html‑тег в ячейке, например

, как значение ячейки, или как html‑тег, значение по умолчанию — true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Указывает, предпочтителен ли html или mht файл для представления. Значение по умолчанию — false. Если вы хотите получить более красивое представление, установите значение в true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Указывает, обновляются ли данные кэша диаграммы

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Получает формат сохраняемого файла.

Смотрите [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Указывает, сортировать ли определённые имена перед сохранением файла.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Указывает, проверять ли объединённые ячейки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Указывает, экспортировать ли комментарии при сохранении файла в html; значение по умолчанию — false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false.

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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в поток html.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Укажите префикс Url вложенных файлов, например изображений в html‑файле. Только при сохранении в поток html.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Папка кэшированных файлов используется для хранения некоторых больших данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Очищать книгу после сохранения файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Укажите имя шрифта по умолчанию для экспорта HTML, шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Указывает, экспортировать ли всю книгу в html‑файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


Устанавливает экспортируемую CellArea текущего активного листа Worksheet. Если задать этот атрибут, область печати текущего активного листа Worksheet будет опущена. При сохранении файла в html будет экспортирована только указанная область.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Указывает, экспортировать ли комментарии при сохранении файла в html; значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Указывает, экспортировать ли сетку. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Указывает, экспортировать ли заголовки при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Указывает, сохранять ли изображения в формате Base64 в HTML, MHTML или EPUB.

**Remarks**

Когда это свойство установлено в true, данные изображения экспортируются непосредственно в элементы img, и отдельные файлы не создаются.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Указывает, экспортировать ли только область печати в html‑файл. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Заголовок html‑страницы. Используется только при сохранении в поток html.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Разбирать html‑тег в ячейке, например

, как значение ячейки, или как html‑тег, значение по умолчанию — true

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Указывает, предпочтителен ли html или mht файл для представления. Значение по умолчанию — false. Если вы хотите получить более красивое представление, установите значение в true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Указывает, обновляются ли данные кэша диаграммы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Указывает, сортировать ли определённые имена перед сохранением файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Указывает, проверять ли объединённые ячейки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

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

