---
title: "GridCells"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

يحتوي على مجموعة من كائنات [GridCell](../../com.aspose.gridweb/gridcell).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | يحصل على اسم الخلية وفقًا لصفها وعمودها. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | يحصل على فهارس الصف والعمود للخلية وفقًا لاسمه |
| [checkCell(int row, int column)](#checkCell-int-int-) | يحصل على عنصر [GridCell](../../com.aspose.gridweb/gridcell) أو null عند فهرس صف الخلية والعمود المحددين. |
| [checkColumn(int col)](#checkColumn-int-) | يحصل على عنصر [GridColumn](../../com.aspose.gridweb/gridcolumn) أو null عند فهرس العمود المحدد. |
| [checkRow(int i)](#checkRow-int-) | يحصل على عنصر [GridRow](../../com.aspose.gridweb/gridrow) أو null عند فهرس صف الخلية المحدد. |
| [clear()](#clear--) | امسح جميع الخلايا في المجموعة. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | يمسح محتويات نطاق. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | يمسح محتويات نطاق. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | يمسح تنسيق نطاق. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | يمسح تنسيق نطاق. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | يمسح محتويات وتنسيق نطاق. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | يمسح محتويات وتنسيق نطاق. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | يحصل على اسم العمود وفقًا لمؤشر العمود. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | يحصل على مؤشر العمود وفقًا لاسم العمود. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | ينسخ البيانات والتنسيقات لصف كامل. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | ينسخ البيانات والتنسيقات لعدة صفوف كاملة. |
| [deleteBlankColumns()](#deleteBlankColumns--) | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [deleteBlankRows()](#deleteBlankRows--) | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | يحذف عمودًا. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | يحذف عمودًا. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | يحذف عدة أعمدة. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | يحذف نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | يحذف صفًا. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | يحذف عدة صفوف. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | يحذف عدة صفوف في ورقة العمل. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | يصدّر البيانات في مجموعة [GridCells](../../com.aspose.gridweb/gridcells) إلى كائن مصفوفة ثنائية الأبعاد. |
| [get(int row, int column)](#get-int-int-) | يحصل على عنصر [GridCell](../../com.aspose.gridweb/gridcell) عند فهرس صف الخلية والعمود المحددين. |
| [get(String cellName)](#get-java.lang.String-) | يحصل على عنصر [GridCell](../../com.aspose.gridweb/gridcell) عند اسم الخلية المحدد. |
| [getCell(int row, int column)](#getCell-int-int-) | يحصل على عنصر [GridCell](../../com.aspose.gridweb/gridcell) عند فهرس صف الخلية والعمود المحددين. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | يحصل على عرض العمود المحدد |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | يحصل على عرض العمود المحدد، بوحدات البوصة. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | يحصل على عرض العمود المحدد، بوحدات البكسل. |
| [getColumns()](#getColumns--) | يحصل على مجموعة كائنات [GridColumn](../../com.aspose.gridweb/gridcolumn) التي تمثل الأعمدة الفردية في ورقة العمل هذه. |
| [getCount()](#getCount--) | يحصل على عدد الخلايا. |
| [getFirstCell()](#getFirstCell--) | يحصل على الخلية الأولى في ورقة العمل هذه. |
| [getLastCell()](#getLastCell--) | يحصل على الخلية الأخيرة في ورقة العمل هذه. |
| [getMaxColumn()](#getMaxColumn--) | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات أو نمط. |
| [getMaxDataColumn()](#getMaxDataColumn--) | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات. |
| [getMaxDataRow()](#getMaxDataRow--) | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات. |
| [getMaxRow()](#getMaxRow--) | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط. |
| [getMergedCells()](#getMergedCells--) | يحصل على مجموعة الخلايا المدمجة. |
| [getMinColumn()](#getMinColumn--) | الحد الأدنى لمؤشر العمود لتلك الخلايا التي تم إنشاء كائناتها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه). |
| [getMinDataColumn()](#getMinDataColumn--) | الحد الأدنى لمؤشر العمود للخلية التي تحتوي على بيانات. |
| [getMinDataRow()](#getMinDataRow--) | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات. |
| [getMinRow()](#getMinRow--) | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط. |
| [getRow(int i)](#getRow-int-) | يحصل على عنصر [GridRow](../../com.aspose.gridweb/gridrow) عند فهرس صف الخلية المحدد. |
| [getRowEnumerator()](#getRowEnumerator--) | يحصل على مُعدد الصفوف |
| [getRowHeight(int row)](#getRowHeight-int-) | يحصل على ارتفاع الصف المحدد. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | يحصل على ارتفاع صف محدد بوحدة البكسل. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | يحصل على مستوى المخطط للصف. |
| [getRows()](#getRows--) | يحصل على مجموعة كائنات [GridRow](../../com.aspose.gridweb/gridrow) التي تمثل الصفوف الفردية في هذه ورقة العمل. |
| [getStandardHeight()](#getStandardHeight--) | يحصل على ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | يحصل على ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل. |
| [getStandardWidth()](#getStandardWidth--) | يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [getStandardWidthInch()](#getStandardWidthInch--) | يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | احصل على العرض في نوع العرض المختلف. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | يقوم بتجميع الأعمدة. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | يقوم بتجميع الأعمدة. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | يقوم بتجميع الصفوف. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | يخفي عمودًا. |
| [hideRow(int row)](#hideRow-int-) | يخفي صفًا. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | يدرج عمودًا جديدًا في ورقة العمل. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | يدرج عمودًا جديدًا في ورقة العمل. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | يدرج بعض الأعمدة في ورقة العمل. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | يدرج بعض الأعمدة في ورقة العمل. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [insertRow(int rowIndex)](#insertRow-int-) | يدرج صفًا جديدًا في ورقة العمل. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | يدرج عدة صفوف في ورقة العمل. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | يدرج عدة صفوف في ورقة العمل. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | يتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | يتحقق مما إذا كان العمود في الفهرس المحدد مخفيًا. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | يتحقق مما إذا كان الصف في الفهرس المحدد مخفيًا. |
| [iterator()](#iterator--) | يحصل على مُعدد الصفوف |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | ينقل النطاق. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | إزالة القيم المكررة في النطاق. |
| [removeFormulas()](#removeFormulas--) | يزيل جميع الصيغ ويستبدلها بقيمة الصيغة. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | يضبط الحدود لنطاق الخلايا. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | يضبط عرض العمود المحدد. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | يضبط عرض العمود بوحدة البوصة. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | يضبط عرض العمود بوحدة البكسل. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | يضبط ارتفاع الصف المحدد. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | يضبط ارتفاع الصف بوحدة البوصة. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | يضبط ارتفاع الصف بوحدة البكسل. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | يضبط مستوى المخطط للصف. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | يضبط النمط لنطاق خلايا محدد. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | يضبط النمط لنطاق خلايا محدد. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | يرتب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | يرتب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | يفك دمج نطاق محدد من الخلايا المدمجة. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | يفك تجميع الأعمدة. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | يفك تجميع الصفوف. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | يكشف عن عمود |
| [unhideRow(int row)](#unhideRow-int-) | يكشف عن صف. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


يحصل على اسم الخلية وفقًا لصفها وعمودها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |

**Returns:**
java.lang.String - اسم الخلية.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


يحصل على فهارس الصف والعمود للخلية وفقًا لاسمه

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |
| صف | int | فهرس الصف الناتج |
| عمود | int | فهرس العمود الناتج |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


يحصل على عنصر [GridCell](../../com.aspose.gridweb/gridcell) أو null عند فهرس صف الخلية والعمود المحددين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |
| عمود | int | فهرس العمود |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


يحصل على عنصر [GridColumn](../../com.aspose.gridweb/gridcolumn) أو null عند فهرس العمود المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| col | int | The column index. |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


يحصل على عنصر [GridRow](../../com.aspose.gridweb/gridrow) أو null عند فهرس صف الخلية المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| i | int | فهرس الصف |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


امسح جميع الخلايا في المجموعة.

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


يمسح محتويات نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | النطاق المراد مسحه. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


يمسح محتويات نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| endColumn | int | فهرس العمود النهائي. |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


يمسح تنسيق نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | النطاق المراد مسحه. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


يمسح تنسيق نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| endColumn | int | فهرس العمود النهائي. |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


يمسح محتويات وتنسيق نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | النطاق المراد مسحه. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


يمسح محتويات وتنسيق نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| endColumn | int | فهرس العمود النهائي. |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


يحصل على اسم العمود وفقًا لمؤشر العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |

**Returns:**
java.lang.String - اسم العمود.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


يحصل على مؤشر العمود وفقًا لاسم العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnName | java.lang.String | اسم العمود. |

**Returns:**
int - فهرس العمود.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


ينسخ البيانات والتنسيقات لعمود كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | كائن الخلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | int | فهرس عمود المصدر. |
| destinationColumnIndex | int | فهرس عمود الوجهة. |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


ينسخ البيانات والتنسيقات لعمود كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | كائن الخلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | int | فهرس عمود المصدر. |
| destinationColumnIndex | int | فهرس عمود الوجهة. |
| columnNumber | int | رقم العمود المنسوخ. |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


ينسخ البيانات والتنسيقات لصف كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | كائن الخلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | int | فهرس صف المصدر. |
| destinationRowIndex | int | فهرس صف الوجهة. |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


ينسخ البيانات والتنسيقات لعدة صفوف كاملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | كائن الخلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | int | فهرس صف المصدر. |
| destinationRowIndex | int | فهرس صف الوجهة. |
| rowNumber | int | رقم الصف المنسوخ. |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات.

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات.

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


يحذف عمودًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


يحذف عمودًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


يحذف عدة أعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| totalColumns | int | عدد الأعمدة التي سيتم حذفها. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


يحذف نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| endColumn | int | فهرس العمود النهائي. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). خيار إزاحة الخلايا. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


يحذف صفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


يحذف عدة صفوف.

**Remarks**

إذا كان النطاق المحذوف يحتوي على الجزء العلوي (ليس كاملًا) من الجدول (ListObject)، لا يمكن حذف النطاق ولن يتم تنفيذ أي شيء. يعمل كما في MS Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف الأول الذي سيتم حذفه. |
| totalRows | int | عدد الصفوف التي سيتم حذفها. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


يحذف عدة صفوف في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| totalRows | int | عدد الصفوف التي سيتم حذفها. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

**Returns:**
boolean -
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
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


يصدّر البيانات في مجموعة [GridCells](../../com.aspose.gridweb/gridcells) إلى كائن مصفوفة ثنائية الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | int | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | int | عدد الصفوف التي سيتم تصديرها |
| totalColumns | int | عدد الأعمدة التي سيتم تصديرها |

**Returns:**
java.lang.Object[][] - كائن مصفوفة قيم الخلايا المُصدَّرة.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


يحصل على عنصر [GridCell](../../com.aspose.gridweb/gridcell) عند فهرس صف الخلية والعمود المحددين.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


يحصل على عنصر [GridCell](../../com.aspose.gridweb/gridcell) عند اسم الخلية المحدد.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية، بما في ذلك حرف العمود ورقم الصف، على سبيل المثال A5. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


يحصل على عنصر [GridCell](../../com.aspose.gridweb/gridcell) عند فهرس صف الخلية والعمود المحددين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |
| عمود | int | فهرس العمود |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


يحصل على عرض العمود المحدد

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود |

**Returns:**
double - عرض العمود
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


يحصل على عرض العمود المحدد، بوحدات البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود |

**Returns:**
double - عرض العمود
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


يحصل على عرض العمود المحدد، بوحدات البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود |

**Returns:**
int - عرض العمود في العرض العادي.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


يحصل على مجموعة كائنات [GridColumn](../../com.aspose.gridweb/gridcolumn) التي تمثل الأعمدة الفردية في ورقة العمل هذه.

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد الخلايا.

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


يحصل على الخلية الأولى في ورقة العمل هذه.

**Remarks**

يرجع null إذا لم يكن هناك بيانات في ورقة العمل.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


يحصل على الخلية الأخيرة في ورقة العمل هذه.

**Remarks**

يرجع null إذا لم يكن هناك بيانات في ورقة العمل.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات أو نمط.

**Remarks**

إرجاع -1 إذا لم توجد خلية.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات.

**Remarks**

\-1 سيتم إرجاعه إذا لم توجد خلية تحتوي على بيانات. هذه الخاصية تحتاج إلى التكرار وفحص جميع الخلايا في ورقة العمل، لذا فهي عملية مستهلكة للوقت ولا ينبغي استدعاؤها بشكل متكرر.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات.

**Remarks**

إرجاع -1 إذا لم توجد خلية تحتوي على بيانات.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط.

**Remarks**

إرجاع -1 إذا لم توجد خلية تحتوي على بيانات أو نمط في ورقة العمل.

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


يحصل على مجموعة الخلايا المدمجة.

**Remarks**

في هذا التجميع، كل عنصر هو بنية [GridCellArea](../../com.aspose.gridweb/gridcellarea) التي تمثل مساحة من الخلايا المدمجة.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


الحد الأدنى لمؤشر العمود لتلك الخلايا التي تم إنشاء كائناتها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه).

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


الحد الأدنى لمؤشر العمود للخلية التي تحتوي على بيانات.

**Remarks**

\-1 سيتم إرجاعه إذا لم توجد خلية تحتوي على بيانات. هذه الخاصية تحتاج إلى التكرار وفحص جميع الخلايا في ورقة العمل، لذا فهي عملية مستهلكة للوقت ولا ينبغي استدعاؤها بشكل متكرر.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط.

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


يحصل على عنصر [GridRow](../../com.aspose.gridweb/gridrow) عند فهرس صف الخلية المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| i | int | فهرس الصف |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


يحصل على مُعدد الصفوف

**Returns:**
java.util.Iterator - مُعدِّد الصفوف.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


يحصل على ارتفاع الصف المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |

**Returns:**
double - ارتفاع الصف
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


يحصل على ارتفاع صف محدد بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |

**Returns:**
double - ارتفاع الصف
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


يحصل على ارتفاع صف محدد بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |

**Returns:**
int - ارتفاع الصف
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


يحصل على مستوى المخطط للصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |

**Returns:**
int - مستوى المخطط.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


يحصل على مجموعة كائنات [GridRow](../../com.aspose.gridweb/gridrow) التي تمثل الصفوف الفردية في هذه ورقة العمل.

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


يحصل على ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


يحصل على ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل.

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


احصل على العرض في نوع العرض المختلف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | The column index. |

**Returns:**
int - عرض العمود بوحدة البكسل
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


يقوم بتجميع الأعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس العمود الأول لتجميعه. |
| lastIndex | int | فهرس العمود الأخير لتجميعه. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


يقوم بتجميع الأعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس العمود الأول لتجميعه. |
| lastIndex | int | فهرس العمود الأخير لتجميعه. |
| isHidden | boolean | يحدد ما إذا كانت الأعمدة المجمعة مخفية. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


يقوم بتجميع الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول لتجميعه. |
| lastIndex | int | فهرس الصف الأخير لتجميعه. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


يخفي عمودًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


يخفي صفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


يدرج عمودًا جديدًا في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


يدرج عمودًا جديدًا في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق عمل أخرى. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


يدرج بعض الأعمدة في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| totalColumns | int | عدد الأعمدة. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


يدرج بعض الأعمدة في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| totalColumns | int | عدد الأعمدة. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق عمل أخرى. |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | إزاحة المنطقة. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). خيار إزاحة الخلايا. |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | إزاحة المنطقة. |
| shiftNumber | int | عدد الصفوف أو الأعمدة التي سيتم إدراجها. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). خيار إزاحة الخلايا. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


يدرج صفًا جديدًا في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


يدرج عدة صفوف في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| totalRows | int | عدد الصفوف التي سيتم إدراجها. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


يدرج عدة صفوف في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| totalRows | int | عدد الصفوف التي سيتم إدراجها. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق عمل أخرى. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


يتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود |

**Returns:**
منطقي - true إذا كان العمود المعطى لا يحتوي على أي بيانات
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


يتحقق مما إذا كان العمود في الفهرس المحدد مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود |

**Returns:**
منطقي - true إذا كان العمود مخفيًا.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


يتحقق مما إذا كان الصف في الفهرس المحدد مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف |

**Returns:**
منطقي - true إذا كان الصف مخفيًا
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على مُعدد الصفوف

**Returns:**
java.util.Iterator - مُعدد الصفوف
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


يدمج نطاقًا محددًا من الخلايا في خلية واحدة.

**Remarks**

الإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول في هذا النطاق (مؤشر صفر) |
| firstColumn | int | العمود الأول في هذا النطاق (مؤشر صفر) |
| totalRows | int | عدد الصفوف (مؤشر واحد) |
| totalColumns | int | عدد الأعمدة (مستند إلى الواحد) |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


ينقل النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | النطاق الذي يجب تحريكه. |
| destRow | int | صف الوجهة. |
| destColumn | int | عمود الوجهة. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


إزالة القيم المكررة في النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية. |
| startColumn | int | عمود البداية |
| endRow | int | فهرس صف النهاية. |
| endColumn | int | فهرس عمود النهاية. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


يزيل جميع الصيغ ويستبدلها بقيمة الصيغة.

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


يضبط الحدود لنطاق الخلايا.

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | رقم الصف الأول للنطاق (مبني على الصفر). |
| firstColumn | int | رقم العمود الأول للنطاق (مبني على الصفر). |
| rowNumber | int | عدد الصفوف. |
| columnNumber | int | عدد الأعمدة. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). موضع الحد. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | نمط الحد. |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


يضبط عرض العمود المحدد.

**Remarks**

لإخفاء عمود، يتم ضبط عرض العمود إلى صفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| العرض | double | عرض العمود. يجب أن يكون عرض العمود بين 0 و 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


يضبط عرض العمود بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| inches | double | عدد البوصات. |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


يضبط عرض العمود بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| بكسل | int | عدد البكسلات. |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


يضبط ارتفاع الصف المحدد.

**Remarks**

لإخفاء صف، يتم ضبط ارتفاع الصف إلى صفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| الارتفاع | double | ارتفاع الصف. بوحدة النقطة يجب أن يكون بين 0 و 409.5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


يضبط ارتفاع الصف بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| inches | double | عدد البوصات. يجب أن يكون بين 0 و 409.5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


يضبط ارتفاع الصف بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| pixels | int | عدد البكسلات. |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


يضبط مستوى المخطط للصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| outlineLevel | int | مستوى المخطط. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


يضبط النمط لنطاق خلايا محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول في هذا النطاق (مؤشر صفر) |
| firstColumn | int | العمود الأول في هذا النطاق (مؤشر صفر) |
| rowNumber | int | عدد الصفوف (مؤشر واحد) |
| columnNumber | int | عدد الأعمدة (مستند إلى الواحد) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | كائن النمط الذي سيتم تعيينه |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


يضبط النمط لنطاق خلايا محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellRange | java.lang.String | نطاق أسماء الخلايا، مثل "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | كائن النمط الذي سيتم تعيينه |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


يقوم بترتيب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. يقوم بترتيب البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | رقم الصف للخلية الأولى التي سيتم ترتيبها. |
| startColumn | int | رقم العمود للخلية الأولى التي سيتم ترتيبها. |
| الصفوف | int | عدد الصفوف التي سيتم استيرادها. |
| الأعمدة | int | عدد الأعمدة التي سيتم استيرادها. |
| الفهرس | int | فهرس العمود الذي يحدد عمود الفرز. إذا كان الاتجاه من أعلى إلى أسفل، فهو يمثل فهرس العمود الذي يحدد عمود الفرز. إذا كان الاتجاه من اليسار إلى اليمين، فهو يمثل فهرس الصف الذي يحدد صف الفرز. |
| isAsending | boolean | ما إذا كان ترتيب الفرز تصاعديًا . |
| isCaseSensitive | boolean | ما إذا كان الفرز حساسًا لحالة الأحرف . |
| islefttoright | boolean | ما إذا كان اتجاه الفرز من اليسار إلى اليمين |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


يقوم بترتيب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. يقوم بترتيب البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | رقم الصف للخلية الأولى التي سيتم ترتيبها. |
| startColumn | int | رقم العمود للخلية الأولى التي سيتم ترتيبها. |
| الصفوف | int | عدد الصفوف التي سيتم استيرادها. |
| الأعمدة | int | عدد الأعمدة التي سيتم استيرادها. |
| المؤشرات | int[] | مصفوفة فهرس العمود التي تحدد عمود الفرز. إذا كان الاتجاه من أعلى إلى أسفل ،فهي تمثل فهرس العمود الذي يحدد عمود الفرز. إذا كان الاتجاه من اليسار إلى اليمين،فهي تمثل فهرس الصف الذي يحدد صف الفرز. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). مصفوفة ترتيب الفرز . |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). اتجاه الفرز |
| isCaseSensitive | boolean | ما إذا كان الفرز حساسًا لحالة الأحرف . |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


يفك دمج نطاق محدد من الخلايا المدمجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول في هذا النطاق (مؤشر صفر) |
| firstColumn | int | العمود الأول في هذا النطاق (مؤشر صفر) |
| totalRows | int | عدد الصفوف (مؤشر واحد) |
| totalColumns | int | عدد الأعمدة (مستند إلى الواحد) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


يفك تجميع الأعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس العمود الأول الذي سيتم فك تجميعه. |
| lastIndex | int | فهرس العمود الأخير الذي سيتم فك تجميعه. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


يفك تجميع الصفوف.

**Remarks**

يزيل فقط معلومات المجموعة الخارجية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول الذي سيتم فك تجميعه. |
| lastIndex | int | فهرس الصف الأخير الذي سيتم فك تجميعه. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


يكشف عن عمود

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| العرض | double | عرض العمود..يجب أن يكون عرض العمود بين 0 و 255 |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


يكشف عن صف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |

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

