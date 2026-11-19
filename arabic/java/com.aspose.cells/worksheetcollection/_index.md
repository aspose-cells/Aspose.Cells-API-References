---
title: "WorksheetCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

يحتوي على مجموعة من كائنات [Worksheet](../../com.aspose.cells/worksheet).

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add()](#add--) | يضيف ورقة عمل إلى المجموعة. |
| [add(int type)](#add-int-) | يضيف ورقة عمل إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | يضيف ورقة عمل إلى المجموعة. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | نسخ مجموعة من أوراق العمل. |
| [addCopy(int sheetIndex)](#addCopy-int-) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [clear()](#clear--) | مسح جميع أوراق العمل. |
| [clearPivottables()](#clearPivottables--) | يمسح جداول المحور من جدول البيانات. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | ينشئ كائن [Range](../../com.aspose.cells/range) من عنوان النطاق. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | ينشئ كائن [Range](../../com.aspose.cells/range) من عنوان النطاق. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [Worksheet](../../com.aspose.cells/worksheet) عند الفهرس المحدد. |
| [get(String sheetName)](#get-java.lang.String-) | يحصل على عنصر [Worksheet](../../com.aspose.cells/worksheet) بالاسم المحدد. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات. |
| [getActiveSheetName()](#getActiveSheetName--) | يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | يرجع مجموعة [DocumentProperty](../../com.aspose.cells/documentproperty) تمثل جميع خصائص المستند المدمجة في جدول البيانات. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | يرجع مجموعة [DocumentProperty](../../com.aspose.cells/documentproperty) تمثل جميع خصائص المستند المخصصة في جدول البيانات. |
| [getDxfs()](#getDxfs--) | يحصل على سجلات التنسيق التفاضلي الرئيسية. |
| [getExternalLinks()](#getExternalLinks--) | يمثل الروابط الخارجية في دفتر العمل. |
| [getNamedRanges()](#getNamedRanges--) | يحصل على جميع النطاقات المسماة المعرفة مسبقًا في جدول البيانات. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | يحصل على جميع النطاقات المسماة المعرفة مسبقًا في جدول البيانات. |
| [getNames()](#getNames--) | يحصل على مجموعة جميع كائنات Name في جدول البيانات. |
| [getOleSize()](#getOleSize--) | يحصل على الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole. |
| [getPivotCaches()](#getPivotCaches--) | يحصل على جميع [PivotCache](../../com.aspose.cells/pivotcache). |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | يحصل على كائن Range بالاسم المحدد مسبقًا. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | يحصل على [Range](../../com.aspose.cells/range) بالاسم المحدد مسبقًا أو باسم الجدول |
| [getRevisionLogs()](#getRevisionLogs--) | يمثل سجلات المراجعات. |
| [getSensitivityLabels()](#getSensitivityLabels--) | يمثل جميع تسميات الحساسية. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | يحصل على ورقة العمل بالاسم الرمزي. |
| [getTableStyles()](#getTableStyles--) | يحصل على كائن [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--). |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | يحصل على قائمة مؤلفي التعليقات المتسلسلة. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | يحصل على قائمة ألواح المهام. |
| [getWebExtensions()](#getWebExtensions--) | يحصل على قائمة ألواح المهام. |
| [getXmlMaps()](#getXmlMaps--) | يحصل على خرائط XML في دفتر العمل. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [insert(int index, int sheetType)](#insert-int-int-) | إدراج ورقة عمل. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | إدراج ورقة عمل. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | يشير إلى ما إذا كان يتم تحديث جميع الاتصالات عند فتح الملف في MS Excel. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | تحديث جميع جداول المحور والرسوم البيانية مع مصدر المحور. |
| [refreshPivotTables()](#refreshPivotTables--) | يقوم بتحديث جميع جداول PivotTables في ملف Excel. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | يقوم بتحديث جميع جداول PivotTables في ملف Excel. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | يضيف وظيفة الإضافة إلى دفتر العمل |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | يضيف وظيفة الإضافة إلى دفتر العمل |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر عند الفهرس المحدد. |
| [removeAt(String name)](#removeAt-java.lang.String-) | يزيل العنصر بالاسم المحدد. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | يضبط الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | يضبط الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | يشير إلى ما إذا كان يتم تحديث جميع الاتصالات عند فتح الملف في MS Excel. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | يضبط خرائط XML في دفتر العمل. |
| [sortNames()](#sortNames--) | يرتب الأسماء المعرفة. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | يبدل الورقتين. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


يضيف ورقة عمل إلى المجموعة.

**Returns:**
int - فهرس كائن [Worksheet](../../com.aspose.cells/worksheet).
### add(int type) {#add-int-}
```
public int add(int type)
```


يضيف ورقة عمل إلى المجموعة.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). نوع ورقة العمل. |

**Returns:**
int - فهرس كائن [Worksheet](../../com.aspose.cells/worksheet).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


يضيف عنصرًا إلى مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن لإضافته إلى مثيل CollectionBase. |

**Returns:**
int - الموضع الذي تم إدراج العنصر الجديد فيه.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


يضيف ورقة عمل إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم ورقة العمل |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


نسخ مجموعة من أوراق العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | ورقات العمل المصدر. |
| destSheetNames | java.lang.String[] | أسماء الأوراق المنسوخة. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس ورقة العمل المصدر. |

**Returns:**
int - فهرس كائن [Worksheet](../../com.aspose.cells/worksheet).
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم ورقة العمل المصدر. |

**Returns:**
int - فهرس كائن [Worksheet](../../com.aspose.cells/worksheet).
### clear() {#clear--}
```
public void clear()
```


مسح جميع أوراق العمل.

**Remarks**

يجب أن يحتوي دفتر العمل على ورقة عمل.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


يمسح جداول المحور من جدول البيانات.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


إرجاع ما إذا كان المثيل يحتوي على هذا الكائن

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | كائن اختبار |

**Returns:**
boolean - ما إذا كان المثيل يحتوي على هذا الكائن
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


ينشئ كائن [Range](../../com.aspose.cells/range) من عنوان النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العنوان | java.lang.String | عنوان النطاق. |
| sheetIndex | int | فهرس الورقة. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


ينشئ كائن [Range](../../com.aspose.cells/range) من عنوان النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العنوان | java.lang.String | عنوان النطاق. |
| sheetIndex | int | فهرس الورقة. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


يحصل على عنصر [Worksheet](../../com.aspose.cells/worksheet) عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


يحصل على عنصر [Worksheet](../../com.aspose.cells/worksheet) بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم ورقة العمل |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات.

**Remarks**

فهرس الورقة يبدأ من الصفر.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


يرجع مجموعة [DocumentProperty](../../com.aspose.cells/documentproperty) تمثل جميع خصائص المستند المدمجة في جدول البيانات.

**Remarks**

لا يمكن إضافة خاصية جديدة إلى قائمة خصائص المستند المدمجة. يمكنك فقط الحصول على خاصية مدمجة وتغيير قيمتها. القائمة التالية هي أسماء الخصائص المدمجة:

Title

الموضوع

المؤلف

الكلمات المفتاحية

التعليقات

القالب

المؤلف الأخير

رقم المراجعة

اسم التطبيق

تاريخ الطباعة الأخير

تاريخ الإنشاء

وقت الحفظ الأخير

إجمالي وقت التحرير

عدد الصفحات

عدد الكلمات

عدد الأحرف

الأمان

الفئة

التنسيق

المدير

الشركة

عدد البايتات

عدد الأسطر

عدد الفقرات

عدد الشرائح

عدد الملاحظات

عدد الشرائح المخفية

عدد مقاطع الوسائط المتعددة

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


يحصل على عدد العناصر الموجودة في مثيل CollectionBase.

**Returns:**
int - عدد العناصر الموجودة في مثيل CollectionBase.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


يرجع مجموعة [DocumentProperty](../../com.aspose.cells/documentproperty) تمثل جميع خصائص المستند المخصصة في جدول البيانات.

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


يحصل على سجلات التنسيق التفاضلي الرئيسية.

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


يمثل الروابط الخارجية في دفتر العمل.

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


يحصل على جميع النطاقات المسماة المعرفة مسبقًا في جدول البيانات.

**Returns:**
com.aspose.cells.Range[] - مصفوفة من كائنات Range. إذا كان مرجع الاسم المحدد خارجيًا أو يحتوي على نطاقات متعددة، لن يتم إرجاع أي كائن Range لهذا الاسم.

يرجع null إذا لم يكن النطاق المسمى موجودًا.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


يحصل على جميع النطاقات المسماة المعرفة مسبقًا في جدول البيانات.

**Returns:**
com.aspose.cells.Range[] - مصفوفة من كائنات Range.

يرجع null إذا لم يكن النطاق المسمى موجودًا.
### getNames() {#getNames--}
```
public NameCollection getNames()
```


يحصل على مجموعة جميع كائنات Name في جدول البيانات.

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


يحصل على الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole.

**Remarks**

Null يعني عدم وجود إعداد حجم ole.

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


يحصل على جميع [PivotCache](../../com.aspose.cells/pivotcache).

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


يحصل على كائن Range بالاسم المحدد مسبقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rangeName | java.lang.String | اسم النطاق. |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

يرجع null إذا لم يكن النطاق المسمى موجودًا.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


يحصل على [Range](../../com.aspose.cells/range) بالاسم المحدد مسبقًا أو باسم الجدول

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rangeName | java.lang.String | اسم النطاق أو اسم الجدول. |
| currentSheetIndex | int | فهرس الورقة. -1 يمثل العمومي . |
| includeTable | boolean | يشير إلى ما إذا كان يتم فحص جميع الجداول. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


يمثل سجلات المراجعات.

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


يمثل جميع تسميات الحساسية.

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


يحصل على ورقة العمل بالاسم الرمزي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| codeName | java.lang.String | اسم رمز ورقة العمل. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


يحصل على كائن [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--).

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


يحصل على قائمة مؤلفي التعليقات المتسلسلة.

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


يحصل على قائمة ألواح المهام.

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


يحصل على قائمة ألواح المهام.

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


يحصل على خرائط XML في دفتر العمل.

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


يحدد فهرس عنصر محدد في مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | يحدد فهرس عنصر محدد في مثيل CollectionBase. |

**Returns:**
int - فهرس القيمة إذا وجد في القائمة؛ وإلا -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


إدراج ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الورقة |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). نوع الورقة. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


إدراج ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الورقة |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). نوع الورقة. |
| sheetName | java.lang.String | اسم الورقة. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


يشير إلى ما إذا كان يتم تحديث جميع الاتصالات عند فتح الملف في MS Excel.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


يرجع كائن تعداد يتنقل عبر مثيل CollectionBase.

**Returns:**
java.util.Iterator - كائن تكرار لمثيل CollectionBase.
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


تحديث جميع جداول المحور والرسوم البيانية مع مصدر المحور.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة Workbook.RefreshAll(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


يقوم بتحديث جميع جداول PivotTables في ملف Excel.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


يقوم بتحديث جميع جداول PivotTables في ملف Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | الخيار لتحديث مصدر البيانات لجداول المحور. |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


يضيف وظيفة الإضافة إلى دفتر العمل

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| id | int | معرّف البيانات التي تحتوي على وظائف الإضافة، يمكن الحصول عليه من خلال الاستدعاء الأول لـ [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) لنفس ملف الإضافة. |
| functionName | java.lang.String | اسم وظيفة الإضافة |

**Returns:**
java.lang.String - عنوان URL لملف الإضافة الذي يحتوي على وظائف الإضافة
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


يضيف وظيفة الإضافة إلى دفتر العمل

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| addInFile | java.lang.String | الملف يحتوي على وظائف الإضافة |
| functionName | java.lang.String | اسم وظيفة الإضافة |
| lib | boolean | ما إذا كان ملف الإضافة المعطى موجودًا في الدليل أو الدليل الفرعي لمكتبة إضافات المصنف. هذا العلم يُفعَّل ويُحدث فرقًا عندما يكون ملف الإضافة المعطى مسارًا نسبيًا: true يعني أن المسار نسبيًا لمكتبة الإضافة وfalse يعني أن المسار نسبيًا لهذا المصنف. |

**Returns:**
int - معرف البيانات التي تحتوي على الدالة الإضافية المعطاة
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل العنصر عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | قيمة الفهرس للعنصر المراد إزالته. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


يزيل العنصر بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العنصر المراد إزالته. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات.

**Remarks**

فهرس الورقة يبدأ من الصفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


يضبط الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole.

**Remarks**

يُستخدم هذا الأسلوب عادةً لضبط حجم العرض في ملف ppt أو ملف doc.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endColumn | int | فهرس العمود النهائي. |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


يضبط الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole.

**Remarks**

Null يعني عدم وجود إعداد حجم ole.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


يشير إلى ما إذا كان يتم تحديث جميع الاتصالات عند فتح الملف في MS Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


يضبط خرائط XML في دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


يرتب الأسماء المعرفة.

**Remarks**

إذا قمت بإنشاء عدد كبير من النطاقات المسماة في ملف Excel، يرجى استدعاء هذا الأسلوب بعد إنشاء جميع النطاقات المسماة وقبل الحفظ.

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


يبدل الورقتين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex1 | int | ورقة العمل الأولى. |
| sheetIndex2 | int | ورقة العمل الثانية. |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

