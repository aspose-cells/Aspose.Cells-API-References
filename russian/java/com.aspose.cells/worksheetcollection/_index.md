---
title: "WorksheetCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

Инкапсулирует коллекцию объектов [Worksheet](../../com.aspose.cells/worksheet).

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
 
         //Change the name of a worksheet
         sheets.get(0).setName("First Sheet");
 
         //Set the active sheet to the second worksheet
         sheets.setActiveSheetIndex(1);
```
## Методы

| Метод | Описание |
| --- | --- |
| [add()](#add--) | Добавляет лист в коллекцию. |
| [add(int type)](#add-int-) | Добавляет лист в коллекцию. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | Добавляет лист в коллекцию. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | Копирует группу листов. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [clear()](#clear--) | Очистить все листы. |
| [clearPivottables()](#clearPivottables--) | Удаляет сводные таблицы из электронной таблицы. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | Создаёт объект [Range](../../com.aspose.cells/range) из адреса диапазона. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | Создаёт объект [Range](../../com.aspose.cells/range) из адреса диапазона. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [Worksheet](../../com.aspose.cells/worksheet) по указанному индексу. |
| [get(String sheetName)](#get-java.lang.String-) | Получает элемент [Worksheet](../../com.aspose.cells/worksheet) с указанным именем. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Представляет индекс активного листа при открытии электронной таблицы. |
| [getActiveSheetName()](#getActiveSheetName--) | Представляет имя активного листа при открытии электронной таблицы. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все встроенные свойства документа электронной таблицы. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все пользовательские свойства документа электронной таблицы. |
| [getDxfs()](#getDxfs--) | Получает записи главного дифференциального форматирования. |
| [getExternalLinks()](#getExternalLinks--) | Представляет внешние ссылки в книге. |
| [getNamedRanges()](#getNamedRanges--) | Получает все предопределённые именованные диапазоны в электронной таблице. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | Получает все предопределённые именованные диапазоны в электронной таблице. |
| [getNames()](#getNames--) | Получает коллекцию всех объектов Name в электронной таблице. |
| [getOleSize()](#getOleSize--) | Получает отображаемый размер, когда файл Workbook используется как объект Ole. |
| [getPivotCaches()](#getPivotCaches--) | Получает все [PivotCache](../../com.aspose.cells/pivotcache). |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | Получает объект Range по предопределённому имени. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | Получает [Range](../../com.aspose.cells/range) по предопределённому имени или имени таблицы |
| [getRevisionLogs()](#getRevisionLogs--) | Представляет журналы правок. |
| [getSensitivityLabels()](#getSensitivityLabels--) | Представляет все метки чувствительности. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | Получает лист по коду имени. |
| [getTableStyles()](#getTableStyles--) | Получает объект [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--). |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | Получает список авторов ветвящихся комментариев. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | Получает список панелей задач. |
| [getWebExtensions()](#getWebExtensions--) | Получает список панелей задач. |
| [getXmlMaps()](#getXmlMaps--) | Получает XML‑карты в книге. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [insert(int index, int sheetType)](#insert-int-int-) | Вставить лист. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | Вставить лист. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | Указывает, следует ли обновлять все соединения при открытии файла в MS Excel. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | Обновить все сводные таблицы и диаграммы с источником сводных данных. |
| [refreshPivotTables()](#refreshPivotTables--) | Обновляет все сводные таблицы в файле Excel. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Обновляет все сводные таблицы в файле Excel. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | Добавляет функцию надстройки в книгу |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | Добавляет функцию надстройки в книгу |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент по указанному индексу. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Удаляет элемент по указанному имени. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Представляет индекс активного листа при открытии электронной таблицы. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | Представляет имя активного листа при открытии электронной таблицы. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | Устанавливает отображаемый размер, когда файл книги используется как объект OLE. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | Устанавливает отображаемый размер, когда файл книги используется как объект OLE. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | Указывает, следует ли обновлять все соединения при открытии файла в MS Excel. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | Устанавливает XML‑карты в книге. |
| [sortNames()](#sortNames--) | Сортирует определённые имена. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Обменивает местами два листа. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Добавляет лист в коллекцию.

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) индекс объекта.
### add(int type) {#add-int-}
```
public int add(int type)
```


Добавляет лист в коллекцию.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add(SheetType.CHART);
         	Cells cells = workbook.getWorksheets().get(0).getCells();
         	cells.get("c2").putValue(5000);
         	cells.get("c3").putValue(3000);
         	cells.get("c4").putValue(4000);
         	cells.get("c5").putValue(5000);
         	cells.get("c6").putValue(6000);
         	ChartCollection charts = workbook.getWorksheets().get(1).getCharts();
         	int chartIndex = charts.add(ChartType.COLUMN, 10,10,20,20);
         	Chart chart = charts.get(chartIndex);
         	chart.getNSeries().add("Sheet1!C2:C6", true);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). Тип листа. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) индекс объекта.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Добавляет элемент в экземпляр CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект, который нужно добавить в экземпляр CollectionBase. |

**Returns:**
int — позиция, в которую был вставлен новый элемент.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


Добавляет лист в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя листа |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


Копирует группу листов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | Исходные листы. |
| destSheetNames | java.lang.String[] | Имена скопированных листов. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Добавляет лист в коллекцию и копирует данные из существующего листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Индекс исходного листа. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) индекс объекта.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Добавляет лист в коллекцию и копирует данные из существующего листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя исходного листа. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) индекс объекта.
### clear() {#clear--}
```
public void clear()
```


Очистить все листы.

**Remarks**

Книга должна содержать лист.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


Удаляет сводные таблицы из электронной таблицы.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Возвращает, содержит ли экземпляр этот объект

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | тестовый объект |

**Returns:**
boolean — содержит ли экземпляр этот объект
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


Создаёт объект [Range](../../com.aspose.cells/range) из адреса диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| адрес | java.lang.String | Адрес диапазона. |
| sheetIndex | int | Индекс листа. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


Создаёт объект [Range](../../com.aspose.cells/range) из адреса диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| адрес | java.lang.String | Адрес диапазона. |
| sheetIndex | int | Индекс листа. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
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
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


Получает элемент [Worksheet](../../com.aspose.cells/worksheet) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


Получает элемент [Worksheet](../../com.aspose.cells/worksheet) с указанным именем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя листа |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Представляет индекс активного листа при открытии электронной таблицы.

**Remarks**

Индекс листа начинается с нуля.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


Представляет имя активного листа при открытии электронной таблицы.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все встроенные свойства документа электронной таблицы.

**Remarks**

Новый параметр нельзя добавить в список встроенных свойств документа. Можно только получить встроенное свойство и изменить его значение. Ниже приведён список имён встроенных свойств:

Title

Тема

Автор

Ключевые слова

Комментарии

Шаблон

Последний автор

Номер ревизии

Имя приложения

Дата последней печати

Дата создания

Время последнего сохранения

Общее время редактирования

Количество страниц

Количество слов

Количество символов

Безопасность

Категория

Формат

Менеджер

Компания

Количество байт

Количество строк

Количество абзацев

Количество слайдов

Количество заметок

Количество скрытых слайдов

Количество мультимедийных клипов

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все пользовательские свойства документа электронной таблицы.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getDxfs() {#getDxfs--}
```
public DxfCollection getDxfs()
```


Получает записи главного дифференциального форматирования.

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


Представляет внешние ссылки в книге.

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


Получает все предопределённые именованные диапазоны в электронной таблице.

**Returns:**
com.aspose.cells.Range[] - Массив объектов Range. Если ссылка определённого Name внешняя или содержит несколько диапазонов, объект Range не будет возвращён для этого Name.

Возвращает null, если именованный диапазон не существует.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


Получает все предопределённые именованные диапазоны в электронной таблице.

**Returns:**
com.aspose.cells.Range[] - Массив объектов Range.

Возвращает null, если именованный диапазон не существует.
### getNames() {#getNames--}
```
public NameCollection getNames()
```


Получает коллекцию всех объектов Name в электронной таблице.

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


Получает отображаемый размер, когда файл Workbook используется как объект Ole.

**Remarks**

Null означает отсутствие настройки размера ole.

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


Получает все [PivotCache](../../com.aspose.cells/pivotcache).

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


Получает объект Range по предопределённому имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rangeName | java.lang.String | Имя диапазона. |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

Возвращает null, если именованный диапазон не существует.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


Получает [Range](../../com.aspose.cells/range) по предопределённому имени или имени таблицы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rangeName | java.lang.String | Имя диапазона или имя таблицы. |
| currentSheetIndex | int | Индекс листа. -1 представляет глобальный. |
| includeTable | boolean | Указывает, проверять ли все таблицы. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


Представляет журналы правок.

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


Представляет все метки чувствительности.

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


Получает лист по коду имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| codeName | java.lang.String | Кодовое имя листа. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


Получает объект [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--).

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


Получает список авторов ветвящихся комментариев.

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


Получает список панелей задач.

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


Получает список панелей задач.

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


Получает XML‑карты в книге.

**Returns:**
[XmlMapCollection](../../com.aspose.cells/xmlmapcollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Определяет индекс конкретного элемента в экземпляре CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Определяет индекс конкретного элемента в экземпляре CollectionBase. |

**Returns:**
int — индекс значения, если оно найдено в списке; иначе -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


Вставить лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс листа |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Тип листа. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


Вставить лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс листа |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Тип листа. |
| sheetName | java.lang.String | Имя листа. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


Указывает, следует ли обновлять все соединения при открытии файла в MS Excel.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Возвращает перечислитель, который проходит по экземпляру CollectionBase.

**Returns:**
java.util.Iterator — итератор для экземпляра CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Обновить все сводные таблицы и диаграммы с источником сводных данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте метод Workbook.RefreshAll(). Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Обновляет все сводные таблицы в файле Excel.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Обновляет все сводные таблицы в файле Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Опция обновления источника данных сводных таблиц. |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


Добавляет функцию надстройки в книгу

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| id | int | Идентификатор данных, содержащих функции надстроек, можно получить при первом вызове [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) для того же файла надстройки. |
| functionName | java.lang.String | имя функции надстройки |

**Returns:**
java.lang.String - URL файла надстройки, содержащего функции надстройки
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


Добавляет функцию надстройки в книгу

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| addInFile | java.lang.String | файл, содержащий функции надстройки |
| functionName | java.lang.String | имя функции надстройки |
| lib | boolean | является ли указанный файл дополнения в каталоге или подкаталоге библиотеки Workbook Add-In. Этот флаг вступает в силу и имеет значение, когда указанный addInFile имеет относительный путь: true обозначает, что путь относительно библиотеки Add-In, а false — что путь относительно этой книги. |

**Returns:**
int — идентификатор данных, содержащих указанную функцию дополнения
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет элемент по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Значение индекса элемента, который нужно удалить. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Удаляет элемент по указанному имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя элемента, который нужно удалить. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Представляет индекс активного листа при открытии электронной таблицы.

**Remarks**

Индекс листа начинается с нуля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


Представляет имя активного листа при открытии электронной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


Устанавливает отображаемый размер, когда файл книги используется как объект OLE.

**Remarks**

Этот метод обычно используется для настройки размера отображения в файле ppt или doc.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| endRow | int | Индекс конечной строки. |
| startColumn | int | Индекс начального столбца. |
| endColumn | int | Индекс конечного столбца. |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


Устанавливает отображаемый размер, когда файл книги используется как объект OLE.

**Remarks**

Null означает отсутствие настройки размера ole.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


Указывает, следует ли обновлять все соединения при открытии файла в MS Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


Устанавливает XML‑карты в книге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


Сортирует определённые имена.

**Remarks**

Если вы создаёте большое количество именованных диапазонов в файле Excel, пожалуйста, вызовите этот метод после создания всех именованных диапазонов и перед сохранением.

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Обменивает местами два листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex1 | int | Первый лист. |
| sheetIndex2 | int | Второй лист. |

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

