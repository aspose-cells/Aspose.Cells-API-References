---
title: "Cells"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات المتعلقة بالخلية مثل ... إلخ."
type: docs
url: /ar/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

يحتوي على مجموعة من الكائنات المتعلقة بالخلية، مثل [Cell](../../com.aspose.cells/cell)، [Row](../../com.aspose.cells/row)، ... إلخ.

**Remarks**

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
 
         	//Set default row height
         	cells.setStandardHeight(20);
         	//Set row height
         	cells.setRowHeight(2, 20.5);
 
         	//Set default colum width
         	cells.setStandardWidth(15);
         	//Set column width
         	cells.setColumnWidth(3, 12.57);
 
         	//Merge cells
         	cells.merge(5, 4, 2, 2);
 
         	//Put values to cells
         	cells.get(0, 0).putValue(true);
         	cells.get(0, 1).putValue(1);
         	cells.get(0, 2).putValue("abc");
 
         //Export data
         Object[][] arr = cells.exportArray(0, 0, 10, 10);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | يضيف مرجع كائن نطاق إلى الخلايا |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | يطبق التنسيقات على عمود كامل. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | يطبق التنسيقات على صف كامل. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | يطبق التنسيقات على ورقة عمل كاملة. |
| [checkCell(int row, int column)](#checkCell-int-int-) | يحصل على عنصر [Cell](../../com.aspose.cells/cell) أو null عند فهرس صف الخلية والعمود المحددين. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | يحصل على عنصر [Column](../../com.aspose.cells/column) أو null عند فهرس العمود المحدد. |
| [checkRow(int row)](#checkRow-int-) | يحصل على عنصر [Row](../../com.aspose.cells/row) أو null عند فهرس صف الخلية المحدد. |
| [clear()](#clear--) | يمسح جميع بيانات ورقة العمل. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | يمسح محتويات نطاق. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | يمسح محتويات نطاق. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | يمسح تنسيق نطاق. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | يمسح تنسيق نطاق. |
| [clearMergedCells()](#clearMergedCells--) | يمسح جميع النطاقات المدمجة. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | يمسح محتويات وتنسيق نطاق. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | يمسح محتويات وتنسيق نطاق. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | يحوّل جميع البيانات النصية في ورقة العمل إلى قيمة رقمية إذا كان ذلك ممكنًا. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | ينسخ البيانات وتنسيقات الأعمدة الكاملة. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | ينسخ البيانات وتنسيقات الأعمدة الكاملة. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | ينسخ البيانات وتنسيقات صف كامل. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | ينسخ البيانات وتنسيقات بعض الصفوف الكاملة. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | ينسخ البيانات وتنسيقات بعض الصفوف الكاملة. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | ينسخ البيانات وتنسيقات بعض الصفوف الكاملة. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | ينشئ كائن [Range](../../com.aspose.cells/range) من صفوف الخلايا أو أعمدة الخلايا. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | ينشئ كائن [Range](../../com.aspose.cells/range) من نطاق من الخلايا. |
| [createRange(String address)](#createRange-java.lang.String-) | ينشئ كائن [Range](../../com.aspose.cells/range) من عنوان النطاق. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | ينشئ كائن [Range](../../com.aspose.cells/range) من نطاق من الخلايا. |
| [deleteBlankColumns()](#deleteBlankColumns--) | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [deleteBlankRows()](#deleteBlankRows--) | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو كائن آخر. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو بعض الكائنات الخاصة مثل التعليق المرئي، جدول محوري. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | يحذف عمودًا. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | يحذف عمودًا. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | يحذف عدة أعمدة. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | يحذف عدة أعمدة. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | يحذف نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | يحذف صفًا. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | يحذف صفًا. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | يحذف عدة صفوف. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | يحذف عدة صفوف في ورقة العمل. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | يحذف عدة صفوف في ورقة العمل. |
| [dispose()](#dispose--) | ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | يحصل على الخلية الأخيرة في هذا العمود. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | يحصل على الخلية الأخيرة ذات أعلى فهرس عمود في هذا النطاق. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | يحصل على الخلية الأخيرة في هذا الصف. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | يحصل على الخلية الأخيرة ذات أعلى فهرس صف في هذا النطاق. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | يصدّر البيانات في مجموعة [Cells](../../com.aspose.cells/cells) إلى كائن مصفوفة ثنائية الأبعاد. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | يصدّر نوع قيمة الخلية في مجموعة [Cells](../../com.aspose.cells/cells) إلى كائن مصفوفة ثنائية الأبعاد. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | يجد الخلية التي تحتوي على الكائن المدخل. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | يجد الخلية التي تحتوي على الكائن المدخل. |
| [get(int row, int column)](#get-int-int-) | يحصل على عنصر [Cell](../../com.aspose.cells/cell) عند فهرس صف الخلية المحدد وفهرس العمود. |
| [get(String cellName)](#get-java.lang.String-) | يحصل على عنصر [Cell](../../com.aspose.cells/cell) عند اسم الخلية المحدد. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | احصل على نمط العرض للخلية المعطاة. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | احصل على نمط العرض للخلية المعطاة. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | احصل على نمط الخلية المعطاة. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | يحصل على جميع الخلايا التي تحتوي على صورة مدمجة. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | يحصل على ارتفاع العمود الأصلي بوحدة النقطة إذا كان العمود مخفيًا |
| [getColumnWidth(int column)](#getColumnWidth-int-) | يحصل على عرض (بوحدة الأحرف) العمود المحدد في العرض العادي |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | يحصل على عرض العمود. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | يحصل على عرض العمود المحدد في العرض العادي، بوحدات البوصة. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | يحصل على عرض العمود المحدد في العرض العادي، بوحدات البكسل. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | يحصل على عرض العمود المحدد في العرض العادي، بوحدات البكسل. |
| [getColumns()](#getColumns--) | يحصل على مجموعة كائنات [Column](../../com.aspose.cells/column) التي تمثل الأعمدة الفردية في ورقة العمل هذه. |
| [getCount()](#getCount--) | يحصل على العدد الإجمالي لكائنات Cell المُنشأة. |
| [getCountLarge()](#getCountLarge--) | يحصل على العدد الإجمالي لكائنات Cell المُنشأة. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | احصل على جميع الخلايا التي تشير إلى الخلية المحددة. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على الخلية المحددة. |
| [getFirstCell()](#getFirstCell--) | يحصل على الخلية الأولى في ورقة العمل هذه. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | يحصل على فهرس الصف الأول للخلية التي تحتوي على بيانات في العمود المحدد. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | يحصل على مستوى المخطط (مستند إلى الصفر) للعمود. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | يحصل على مستوى المخطط (مستند إلى الصفر) للصف. |
| [getLastCell()](#getLastCell--) | يحصل على الخلية الأخيرة في ورقة العمل هذه. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | يحصل على فهرس الصف الأخير للخلية التي تحتوي على بيانات في العمود المحدد. |
| [getMaxColumn()](#getMaxColumn--) | الحد الأقصى لفهرس العمود لتلك الخلايا التي تم إنشاؤها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه). |
| [getMaxDataColumn()](#getMaxDataColumn--) | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات. |
| [getMaxDataRow()](#getMaxDataRow--) | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | يحصل على النطاق الأقصى الذي يشمل البيانات والخلايا المدمجة والأشكال. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | يحصل على الحد الأقصى لمستوى مخطط العمود المجمّع (مستند إلى الصفر). |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | يحصل على الحد الأقصى لمستوى مخطط الصف المجمّع (مستند إلى الصفر). |
| [getMaxRow()](#getMaxRow--) | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط. |
| [getMemorySetting()](#getMemorySetting--) | يحصل على خيار استخدام الذاكرة لهذه الخلايا. |
| [getMergedAreas()](#getMergedAreas--) | يحصل على جميع الخلايا المدمجة. |
| [getMergedCells()](#getMergedCells--) | يحصل على مجموعة الخلايا المدمجة. |
| [getMinColumn()](#getMinColumn--) | الحد الأدنى لمؤشر العمود لتلك الخلايا التي تم إنشاء كائناتها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه). |
| [getMinDataColumn()](#getMinDataColumn--) | الحد الأدنى لمؤشر العمود للخلية التي تحتوي على بيانات. |
| [getMinDataRow()](#getMinDataRow--) | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات. |
| [getMinRow()](#getMinRow--) | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط. |
| [getMultiThreadReading()](#getMultiThreadReading--) | يحصل على ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة متعددة الخيوط. |
| [getOdsCellFields()](#getOdsCellFields--) | يحصل على قائمة الحقول في ods. |
| [getPreserveString()](#getPreserveString--) | يحصل على قيمة تشير إلى ما إذا كانت جميع قيم ورقة العمل محفوظة كسلاسل نصية. |
| [getRanges()](#getRanges--) | يحصل على مجموعة كائنات [Range](../../com.aspose.cells/range) التي تم إنشاؤها في وقت التشغيل. |
| [getRowEnumerator()](#getRowEnumerator--) | يحصل على عداد الصفوف. |
| [getRowHeight(int row)](#getRowHeight-int-) | يحصل على ارتفاع صف محدد، بوحدة النقاط. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | يحصل على ارتفاع الصف. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | يحصل على ارتفاع صف محدد بوحدة البكسل. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | يحصل على ارتفاع الصف الأصلي بوحدة النقطة إذا كان الصف مخفيًا. |
| [getRows()](#getRows--) | يحصل على مجموعة كائنات [Row](../../com.aspose.cells/row) التي تمثل الصفوف الفردية في ورقة العمل هذه. |
| [getStandardHeight()](#getStandardHeight--) | يحصل على ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة النقاط. |
| [getStandardHeightInch()](#getStandardHeightInch--) | يحصل على ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البوصة. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | يحصل على ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البكسل. |
| [getStandardWidth()](#getStandardWidth--) | يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [getStandardWidthInch()](#getStandardWidthInch--) | يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | يحصل على عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل. |
| [getStyle()](#getStyle--) | يحصل على النمط الافتراضي لورقة العمل. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | احصل على العرض في نوع العرض المختلف. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | يحصل على ارتفاع الصف المحدد. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | يقوم بتجميع الأعمدة. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | يقوم بتجميع الأعمدة. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | يقوم بتجميع الصفوف. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | يقوم بتجميع الصفوف. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | يخفي عمودًا. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | إخفاء عدة أعمدة. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | يطوي الصفوف/الأعمدة المجمعة. |
| [hideRow(int row)](#hideRow-int-) | يخفي صفًا. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | إخفاء عدة صفوف. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | يستورد مصفوفة من القيم المزدوجة إلى ورقة عمل. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | يستورد مصفوفة ثنائية الأبعاد من القيم المزدوجة إلى ورقة عمل. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | يستورد مصفوفة من الأعداد الصحيحة إلى ورقة عمل. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | يستورد مصفوفة ثنائية الأبعاد من الأعداد الصحيحة إلى ورقة عمل. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | يستورد مصفوفة من السلاسل النصية إلى ورقة عمل. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | يستورد مصفوفة ثنائية الأبعاد من السلاسل النصية إلى ورقة عمل. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | يستورد قائمة مصفوفية من البيانات إلى ورقة عمل. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | استيراد ملف CSV إلى الخلايا. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | استيراد ملف CSV إلى الخلايا. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | استيراد ملف CSV إلى الخلايا. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | استيراد ملف CSV إلى الخلايا. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | يستورد كائنات مخصصة. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | يستورد كائنات مخصصة. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | استيراد البيانات من جدول بيانات مخصص. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | يستورد مصفوفة من الصيغ إلى ورقة عمل. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | يستورد مصفوفة من البيانات إلى ورقة عمل. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | يستورد مصفوفة من البيانات إلى ورقة عمل. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | يستورد البيانات من كائن ResultSet إلى ورقة العمل. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | يستورد البيانات من كائن ResultSet إلى ورقة العمل. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | يستورد البيانات من كائن ResultSet إلى ورقة العمل. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | يستورد البيانات من كائن ResultSet إلى ورقة العمل. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | يستورد البيانات من كائن ResultSet إلى ورقة العمل. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | يستورد البيانات من كائن ResultSet إلى ورقة العمل. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | يستورد البيانات من كائن ResultSet إلى ورقة العمل. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | يستورد البيانات من كائن ResultSet إلى ورقة العمل. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | يستورد مصفوفة ثنائية الأبعاد من البيانات إلى ورقة عمل. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | يستورد مصفوفة ثنائية الأبعاد من البيانات إلى ورقة عمل. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | يستورد مصفوفة ثنائية الأبعاد من البيانات إلى ورقة عمل. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | يستورد مصفوفة ثنائية الأبعاد من البيانات إلى ورقة عمل. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | يدرج عمودًا جديدًا في ورقة العمل. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | يدرج عمودًا جديدًا في ورقة العمل. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | يدرج بعض الأعمدة في ورقة العمل. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | يدرج بعض الأعمدة في ورقة العمل. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | يدرج بعض الأعمدة في ورقة العمل. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | إدراج نطاق مقطوع. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [insertRow(int rowIndex)](#insertRow-int-) | يدرج صفًا جديدًا في ورقة العمل. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | يدرج عدة صفوف في ورقة العمل. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | يدرج عدة صفوف في ورقة العمل. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | يدرج عدة صفوف في ورقة العمل. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | يتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | يتحقق مما إذا كان العمود في الفهرس المحدد مخفيًا. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | يشير إلى ما إذا كان الصف مخفيًا افتراضيًا. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | تحقق مما إذا كان يمكن حذف النطاق. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | يتحقق مما إذا كان الصف في الفهرس المحدد مخفيًا. |
| [iterator()](#iterator--) | يحصل على مُعدِّد الخلايا. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | رابط إلى خريطة XML. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | ينقل النطاق. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | يزيل الصفوف المكررة في الورقة. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | يزيل القيم المكررة في النطاق. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | يزيل البيانات المكررة في النطاق. |
| [removeFormulas()](#removeFormulas--) | يزيل جميع الصيغ ويستبدلها بقيمة الصيغة. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | يسترجع إعدادات المجاميع الفرعية للنطاق. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | يضبط عرض العمود المحدد في العرض العادي. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | يضبط عرض العمود بوحدة البوصة في العرض العادي. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | يضبط عرض العمود بوحدة البكسل في العرض العادي. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | يشير إلى ما إذا كان الصف مخفيًا افتراضيًا. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | يضبط خيار استخدام الذاكرة لهذه الخلايا. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | يضبط ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة متعددة الخيوط. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | يضبط قيمة تشير إلى ما إذا كانت جميع قيم ورقة العمل محفوظة كسلاسل نصية. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | يضبط ارتفاع الصف المحدد. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | يضبط ارتفاع الصف بوحدة البوصة. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | يضبط ارتفاع الصف بوحدة البكسل. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | يضبط ارتفاع الصف الافتراضي في هذه ورقة العمل، بوحدة النقاط. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | يضبط ارتفاع الصف الافتراضي في هذه ورقة العمل، بوحدة البوصة. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | يضبط ارتفاع الصف الافتراضي في هذه ورقة العمل، بوحدة البكسل. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | يضبط النمط الافتراضي لورقة العمل. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | يضبط عرض العمود في عرض مختلف. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | يوسع الصفوف/الأعمدة المجمعة. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | ينشئ المجاميع الفرعية للنطاق. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | ينشئ المجاميع الفرعية للنطاق. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | يقسم المحتوى في العمود المحدد إلى أعمدة متعددة.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | يفك دمج نطاق محدد من الخلايا المدمجة. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | يفك تجميع الأعمدة. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | يفك تجميع الصفوف. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | يفك تجميع الصفوف. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | يكشف عن عمود |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | يكشف عن عدة أعمدة. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | يكشف عن صف. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | يكشف عن الصفوف المخفية. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


يضيف مرجع كائن نطاق إلى الخلايا

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | كائن النطاق سيكون موجودًا في الخلايا |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


يطبق التنسيقات على عمود كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | The column index. |
| style | [Style](../../com.aspose.cells/style) | كائن النمط الذي سيتم تطبيقه. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامات تشير إلى خصائص التنسيق المطبقة. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


يطبق التنسيقات على صف كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| style | [Style](../../com.aspose.cells/style) | كائن النمط الذي سيتم تطبيقه. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامات تشير إلى خصائص التنسيق المطبقة. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


يطبق التنسيقات على ورقة عمل كاملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | كائن النمط الذي سيتم تطبيقه. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامات تشير إلى خصائص التنسيق المطبقة. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


يحصل على عنصر [Cell](../../com.aspose.cells/cell) أو null عند فهرس صف الخلية والعمود المحددين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |
| عمود | int | فهرس العمود |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


يحصل على عنصر [Column](../../com.aspose.cells/column) أو null عند فهرس العمود المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | The column index. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


يحصل على عنصر [Row](../../com.aspose.cells/row) أو null عند فهرس صف الخلية المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


يمسح جميع بيانات ورقة العمل.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


يمسح محتويات نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | النطاق المراد مسحه. |

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

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


يمسح تنسيق نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | النطاق المراد مسحه. |

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

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


يمسح جميع النطاقات المدمجة.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


يمسح محتويات وتنسيق نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | النطاق المراد مسحه. |

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

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


يحوّل جميع البيانات النصية في ورقة العمل إلى قيمة رقمية إذا كان ذلك ممكنًا.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


ينسخ البيانات والتنسيقات لعمود كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | كائن خلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | int | فهرس عمود المصدر. |
| destinationColumnIndex | int | فهرس عمود الوجهة. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


ينسخ البيانات وتنسيقات الأعمدة الكاملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | كائن خلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | int | فهرس عمود المصدر. |
| destinationColumnIndex | int | فهرس عمود الوجهة. |
| columnNumber | int | رقم العمود المنسوخ. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


ينسخ البيانات والتنسيقات لعمود كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | كائن خلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | int | فهرس عمود المصدر. |
| destinationColumnIndex | int | فهرس عمود الوجهة. |
| columnNumber | int | رقم العمود المنسوخ. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | خيارات اللصق. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


ينسخ البيانات وتنسيقات الأعمدة الكاملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | كائن خلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | int | فهرس عمود المصدر. |
| sourceTotalColumns | int | عدد أعمدة المصدر. |
| destinationColumnIndex | int | فهرس عمود الوجهة. |
| destinationTotalColumns | int | عدد أعمدة الوجهة. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


ينسخ البيانات وتنسيقات صف كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | كائن خلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | int | فهرس صف المصدر. |
| destinationRowIndex | int | فهرس صف الوجهة. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


ينسخ البيانات وتنسيقات بعض الصفوف الكاملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | كائن خلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | int | فهرس صف المصدر. |
| destinationRowIndex | int | فهرس صف الوجهة. |
| rowNumber | int | رقم الصف المنسوخ. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


ينسخ البيانات وتنسيقات بعض الصفوف الكاملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | كائن خلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | int | فهرس صف المصدر. |
| destinationRowIndex | int | فهرس صف الوجهة. |
| rowNumber | int | رقم الصف المنسوخ. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | خيارات النسخ. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


ينسخ البيانات وتنسيقات بعض الصفوف الكاملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | كائن خلايا المصدر يحتوي على البيانات والتنسيقات للنسخ. |
| sourceRowIndex | int | فهرس صف المصدر. |
| destinationRowIndex | int | فهرس صف الوجهة. |
| rowNumber | int | رقم الصف المنسوخ. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | خيارات النسخ. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | خيارات اللصق. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


ينشئ كائن [Range](../../com.aspose.cells/range) من صفوف الخلايا أو أعمدة الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول أو فهرس العمود الأول، يبدأ من الصفر. |
| عدد | int | العدد الإجمالي للصفوف أو الأعمدة، يبدأ من الواحد. |
| isVertical | boolean | صحيح - النطاق تم إنشاؤه من أعمدة الخلايا. خطأ - النطاق تم إنشاؤه من صفوف الخلايا. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


ينشئ كائن [Range](../../com.aspose.cells/range) من نطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول من هذا النطاق |
| firstColumn | int | العمود الأول من هذا النطاق |
| totalRows | int | عدد الصفوف |
| totalColumns | int | عدد الأعمدة |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


ينشئ كائن [Range](../../com.aspose.cells/range) من عنوان النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العنوان | java.lang.String | عنوان النطاق. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


ينشئ كائن [Range](../../com.aspose.cells/range) من نطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftCell | java.lang.String | اسم الخلية العلوية اليسرى. |
| lowerRightCell | java.lang.String | اسم الخلية السفلية اليمنى. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | خيارات حذف النطاق. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو كائن آخر.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو بعض الكائنات الخاصة مثل التعليق المرئي، جدول محوري.

**Remarks**

بالنسبة للصفوف الفارغة التي سيتم حذفها، ليس من الضروري فقط أن تكون [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) صحيحة، بل يجب أيضًا عدم وجود أي تعليق مرئي معرف لأي خلية في تلك الصفوف، ولا جدول محوري يمتد نطاقه إلى تلك الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | خيارات حذف النطاق. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


يحذف عمودًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود الذي سيتم حذفه. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


يحذف عمودًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود الذي سيتم حذفه. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


يحذف عدة أعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود الأول الذي سيتم حذفه. |
| totalColumns | int | عدد الأعمدة التي سيتم حذفها. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


يحذف عدة أعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود الأول الذي سيتم حذفه. |
| totalColumns | int | عدد الأعمدة التي سيتم حذفها. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | خيارات عملية الحذف |

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
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). خيار إزاحة الخلايا. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


يحذف صفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف الذي سيتم حذفه. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


يحذف صفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف الذي سيتم حذفه. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


يحذف عدة صفوف.

**Remarks**

إذا كان النطاق المحذوف يحتوي على الجزء العلوي (ليس كاملًا) من الجدول (ListObject)، لا يمكن حذف النطاق ولن يتم اتخاذ أي إجراء. يعمل بنفس الطريقة مع MS Excel.

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
| rowIndex | int | فهرس الصف الأول الذي سيتم حذفه. |
| totalRows | int | عدد الصفوف التي سيتم حذفها. |
| updateReference | boolean | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


يحذف عدة صفوف في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف الأول الذي سيتم حذفه. |
| totalRows | int | عدد الصفوف التي سيتم حذفها. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | خيارات عملية الحذف |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


يحصل على الخلية الأخيرة في هذا العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


يحصل على الخلية الأخيرة ذات أعلى فهرس عمود في هذا النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endColumn | int | فهرس العمود النهائي. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


يحصل على الخلية الأخيرة في هذا الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


يحصل على الخلية الأخيرة ذات أعلى فهرس صف في هذا النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endColumn | int | فهرس العمود النهائي. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
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


يصدّر البيانات في مجموعة [Cells](../../com.aspose.cells/cells) إلى كائن مصفوفة ثنائية الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | int | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | int | عدد الصفوف التي سيتم تصديرها |
| totalColumns | int | عدد الأعمدة التي سيتم تصديرها |

**Returns:**
java.lang.Object[][] - كائن مصفوفة قيم الخلايا المُصدَّرة.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


يصدّر نوع قيمة الخلية في مجموعة [Cells](../../com.aspose.cells/cells) إلى كائن مصفوفة ثنائية الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | int | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | int | عدد الصفوف التي سيتم تصديرها. |
| totalColumns | int | عدد الأعمدة التي سيتم تصديرها. |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype). كائن مصفوفة مُصدَّر يمثل أنواع قيم الخلايا.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


يجد الخلية التي تحتوي على الكائن المدخل.

**Remarks**

يعيد null (Nothing) إذا لم يتم العثور على أي خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ما | java.lang.Object | الكائن المراد البحث عنه. يجب أن يكون النوع int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | الخلية السابقة التي تحمل نفس الكائن. يمكن تعيين هذه المعلمة إلى null إذا كان البحث من البداية. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


يجد الخلية التي تحتوي على الكائن المدخل.

**Remarks**

يعيد null (Nothing) إذا لم يتم العثور على أي خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ما | java.lang.Object | الكائن المراد البحث عنه. يجب أن يكون النوع int,double,DateTime,string,bool. |
| previousCell | [Cell](../../com.aspose.cells/cell) | الخلية السابقة التي تحمل نفس الكائن. يمكن تعيين هذه المعلمة إلى null إذا كان البحث من البداية. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | خيارات البحث |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


يحصل على عنصر [Cell](../../com.aspose.cells/cell) عند فهرس صف الخلية المحدد وفهرس العمود.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


يحصل على عنصر [Cell](../../com.aspose.cells/cell) عند اسم الخلية المحدد.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية، بما في ذلك حرف العمود ورقم الصف، على سبيل المثال A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


احصل على نمط العرض للخلية المعطاة.

**Remarks**

نفس الشيء مع [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--)، ونفس الشيء عند استخدام [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) لـ [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف للخلية المحددة |
| عمود | int | عمود الخلية المحددة |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


احصل على نمط العرض للخلية المعطاة.

**Remarks**

إذا كانت الخلية متأثرة أيضًا بإعدادات أخرى مثل التنسيق الشرطي، كائنات القوائم، إلخ، فقد يكون نمط العرض مختلفًا عن [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-). وبما أن هذه الإعدادات قد تُطبق أيضًا على الخلايا الفارغة (غير الموجودة)، فإن استخدام هذه الطريقة يمكن أن يتجنب إنشاء تلك الخلايا الفارغة وبالتالي يكون الأداء أفضل من الحصول على كائن Cell من Cells ثم استدعاء [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف للخلية المحددة |
| عمود | int | عمود الخلية المحددة |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). يحدد أي الحدود تحتاج إلى الفحص والتعديل وفقًا لحدود الخلايا المجاورة. يرجى مراجعة الوصف لنفس المعلمة في [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


احصل على نمط الخلية المعطاة.

**Remarks**

النمط المُرجَع هو فقط ما تم تعيينه للخلية أو ما ورث من صف/عمود الخلية، ولا يشمل الخصائص المطبقة بواسطة إعدادات أخرى مثل التنسيقات الشرطية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |
| عمود | int | عمود |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


يحصل على جميع الخلايا التي تحتوي على صورة مدمجة.

**Remarks**

إذا لم توجد صورة تم تعيينها كـ "Place in Cell" في ورقة العمل هذه، سيتم إرجاع null.

**Returns:**
java.util.Iterator - مُعدِّد لتعداد جميع كائنات Cell التي تحتوي على صورة مدمجة
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnOriginalWidthPoint(int column) {#getColumnOriginalWidthPoint-int-}
```
public double getColumnOriginalWidthPoint(int column)
```


يحصل على ارتفاع العمود الأصلي بوحدة النقطة إذا كان العمود مخفيًا

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن قديمة. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetColumnWidth(int ,bool , CellsUnitType ). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | The row index. |

**Returns:**
double - عرض العمود في العرض العادي.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


يحصل على عرض (بوحدة الأحرف) العمود المحدد في العرض العادي

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود |

**Returns:**
double - عرض العمود. في جداول البيانات، يُقاس عرض العمود بعدد الأحرف لعرض أقصى رقم من الأرقام 0~9 كما يُعرض في خط النمط العادي.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


يحصل على عرض العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | The column index. |
| isOriginal | boolean | يشير إلى ما إذا كان يتم الحصول على العرض الأصلي. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


يحصل على عرض العمود المحدد في العرض العادي، بوحدات البوصة.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن قديمة. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetColumnWidth(int ,bool , CellsUnitType ). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود |

**Returns:**
double - عرض العمود في العرض العادي.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


يحصل على عرض العمود المحدد في العرض العادي، بوحدات البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود |

**Returns:**
int - عرض العمود في العرض العادي.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


يحصل على عرض العمود المحدد في العرض العادي، بوحدات البكسل.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن قديمة. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetColumnWidth(int ,bool , CellsUnitType ). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود |
| الأصلي | boolean | يشير إلى ما إذا كان يتم إرجاع العرض الأصلي حتى عندما يكون العمود مخفيًا |

**Returns:**
int - عرض العمود في العرض العادي.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


يحصل على مجموعة كائنات [Column](../../com.aspose.cells/column) التي تمثل الأعمدة الفردية في ورقة العمل هذه.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على العدد الإجمالي لكائنات Cell المُنشأة.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


يحصل على العدد الإجمالي لكائنات Cell المُنشأة.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


احصل على جميع الخلايا التي تشير إلى الخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isAll | boolean | يشير إلى ما إذا كان يتم فحص أوراق عمل أخرى |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
com.aspose.cells.Cell[] -
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على الخلية المحددة.

**Remarks**

لاستخدام هذه الطريقة، يرجى التأكد من أن دفتر العمل تم تعيينه بقيمة true للخاصية [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) وتم حسابه بالكامل باستخدام هذا الإعداد. إذا لم يكن هناك إشارة صيغة إلى هذه الخلية، سيتم إرجاع null. لمزيد من التفاصيل ومثال، يرجى مراجعة [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف للخلية المحددة |
| عمود | int | فهرس العمود للخلية المحددة. |
| recursive | boolean | ما إذا كان يُرجع تلك التبعيات التي لا تشير إلى الخلية المحددة مباشرةً بل تشير إلى فروع أخرى لتلك الخلية. |

**Returns:**
java.util.Iterator - مُعدد لتعداد جميع التبعيات (كائنات Cell)
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


يحصل على الخلية الأولى في ورقة العمل هذه.

**Remarks**

يرجع null إذا لم يكن هناك بيانات في ورقة العمل.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


يحصل على فهرس الصف الأول للخلية التي تحتوي على بيانات في العمود المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |

**Returns:**
int - فهرس الصف الأول.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


يحصل على مستوى المخطط (مستند إلى الصفر) للعمود.

**Remarks**

إذا لم يكن العمود مُجَمَّعًا، يُرجع صفرًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | مؤشر العمود |

**Returns:**
int - مستوى المخطط للعمود
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


يحصل على مستوى المخطط (مستند إلى الصفر) للصف.

**Remarks**

إذا لم يكن الصف مُجَمَّعًا، يُرجع صفرًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | The row index. |

**Returns:**
int - مستوى المخطط (بدءًا من الصفر) للصف.
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


يحصل على الخلية الأخيرة في ورقة العمل هذه.

**Remarks**

يرجع null إذا لم يكن هناك بيانات في ورقة العمل.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


يحصل على فهرس الصف الأخير للخلية التي تحتوي على بيانات في العمود المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |

**Returns:**
int - فهرس الصف الأخير.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


الحد الأقصى لفهرس العمود لتلك الخلايا التي تم إنشاؤها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه).

**Remarks**

أرجع -1 إذا لم يتم إنشاء أي خلية.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات.

**Remarks**

\-1 سيتم إرجاعه إذا لم توجد خلية تحتوي على بيانات. تحتاج هذه الخاصية إلى تكرار وفحص جميع الخلايا في ورقة العمل بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ولا ينبغي استدعاؤها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات.

**Remarks**

أرجع -1 إذا لم توجد خلية تحتوي على بيانات. تحتاج هذه الخاصية إلى تكرار وفحص الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ولا ينبغي استدعاؤها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


يحصل على النطاق الأقصى الذي يشمل البيانات والخلايا المدمجة والأشكال.

**Remarks**

يرجع null إذا كانت ورقة العمل فارغة منذ Aspose.Cells 21.5.2.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


يحصل على الحد الأقصى لمستوى مخطط العمود المجمّع (مستند إلى الصفر).

**Returns:**
int - الحد الأقصى لمستوى مخطط العمود المُجَمَّع (بدءًا من الصفر)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


يحصل على الحد الأقصى لمستوى مخطط الصف المجمّع (مستند إلى الصفر).

**Returns:**
int - الحد الأقصى لمستوى مخطط الصف المُجَمَّع (بدءًا من الصفر)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط.

**Remarks**

أرجع -1 إذا لم توجد خلية تحتوي على بيانات أو نمط في ورقة العمل. تحتاج هذه الخاصية إلى تكرار وفحص الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ولا ينبغي استدعاؤها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


يحصل على خيار استخدام الذاكرة لهذه الخلايا.

انظر [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

القيود الملحوظة والعمليات الموصى بها لبعض الأنماط:

| الوضع | ملاحظات | مدعوم |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | عند استخدام هذا الوضع لأي ورقة عمل في دفتر واحد، يجب استدعاء [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) في نهاية العمل لإطلاق جميع الموارد مثل الملفات المؤقتة. |
 
الوصول العشوائي إلى الخلايا سيؤدي إلى أداء ضعيف لأن البيانات تحتاج إلى القراءة/التحديث عشوائيًا وبشكل متكرر (لذلك سيتغير المؤشر في الملف وفقًا لذلك وستُطلب عمليات إدخال/إخراج متكررة). إذا أمكن، يرجى دائمًا الوصول إلى البيانات بشكل متسلسل (صفًا بصف).
 
عند تغيير بيانات صف/خلية واحدة، قد تتأثر بيانات الخلايا/الصفوف الأخرى (مثل تحريك البيانات إلى أماكن أخرى لتخصيص مساحة كافية للبيانات المتغيرة). لذا كل تغيير في أي بيانات يتطلب مزامنة الكائنات الموجودة الأخرى (مثل كائن الصف أو الخلية). لذلك، للحصول على أداء أفضل، يرجى عدم الحفاظ على عدة صفوف/خلايا في الوقت نفسه. معالجة كل واحدة على حدة سيقلل من مزامنة البيانات وبالتالي يمكن تحسين الأداء قليلاً. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


يحصل على جميع الخلايا المدمجة.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


يحصل على مجموعة الخلايا المدمجة.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetMergedAreas(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


الحد الأدنى لمؤشر العمود لتلك الخلايا التي تم إنشاء كائناتها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه).

**Remarks**

هذه الخاصية تحتاج إلى التكرار والتحقق من الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ويجب عدم استدعائها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


الحد الأدنى لمؤشر العمود للخلية التي تحتوي على بيانات.

**Remarks**

\-1 سيتم إرجاعه إذا لم توجد خلية تحتوي على بيانات. تحتاج هذه الخاصية إلى تكرار وفحص جميع الخلايا في ورقة العمل بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ولا ينبغي استدعاؤها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات.

**Remarks**

أرجع -1 إذا لم توجد خلية تحتوي على بيانات. تحتاج هذه الخاصية إلى تكرار وفحص الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ولا ينبغي استدعاؤها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط.

**Remarks**

هذه الخاصية تحتاج إلى التكرار والتحقق من الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ويجب عدم استدعائها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


يحدد ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة متعددة الخيوط. القيمة الافتراضية لهذه الخاصية هي false.

**Remarks**

إذا كان هناك عدة خيوط لقراءة كائنات Row/Cell في هذه المجموعة بشكل متزامن، يجب ضبط هذه الخاصية على true، وإلا قد يتم إنتاج نتيجة غير متوقعة. قد يؤدي دعم القراءة متعددة الخيوط إلى تدهور الأداء عند الوصول إلى كائنات Row/Cell من هذه المجموعة. يرجى ملاحظة أن بعض الميزات لا يمكنها دعم القراءة متعددة الخيوط، مثل تنسيق القيم (عن طريق [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), إلخ). لذلك، حتى إذا تم ضبط هذه الخاصية على true، قد لا تزال تلك APIs تعطي نتائج غير متوقعة للقراءة متعددة الخيوط.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


يحصل على قائمة الحقول في ods.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


يُعيد قيمة تُشير إلى ما إذا كانت جميع قيم ورقة العمل محفوظة كسلاسل نصية. القيمة الافتراضية هي false.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


يحصل على مجموعة كائنات [Range](../../com.aspose.cells/range) التي تم إنشاؤها في وقت التشغيل.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


يحصل على عداد الصفوف.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة RowCollection.GetEnumerator(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ مايو 2023. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

**Returns:**
java.util.Iterator - مُعدِّد الصفوف.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


يحصل على ارتفاع صف محدد، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |

**Returns:**
double - ارتفاع الصف
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


يحصل على ارتفاع الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| isOriginal | boolean | ما إذا كان يُعيد ارتفاع الصف الأصلي أو 0 للصف المخفي. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). نوع الوحدة لقيمة الارتفاع المُرجعة |

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
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


يحصل على ارتفاع الصف الأصلي بوحدة النقطة إذا كان الصف مخفيًا.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة Cells.GetRowHeight(int,bool,CellsUnitType). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2024. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


يحصل على مجموعة كائنات [Row](../../com.aspose.cells/row) التي تمثل الصفوف الفردية في ورقة العمل هذه.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


يحصل على ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة النقاط.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


يحصل على ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البوصة.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


يحصل على ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البكسل.

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
### getStyle() {#getStyle--}
```
public Style getStyle()
```


يحصل على النمط الافتراضي لورقة العمل.

**Returns:**
[Style](../../com.aspose.cells/style)
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
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


يحصل على ارتفاع الصف المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |

**Returns:**
double - ارتفاع الصف.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


يحصل على ارتفاع صف محدد بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف |

**Returns:**
double - ارتفاع الصف
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

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


يقوم بتجميع الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول لتجميعه. |
| lastIndex | int | فهرس الصف الأخير لتجميعه. |
| isHidden | boolean | يحدد ما إذا كانت الصفوف المجمعة مخفية. |

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

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


إخفاء عدة أعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| totalColumns | int | رقم العمود. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


يطوي الصفوف/الأعمدة المجمعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isVertical | boolean | True، طي الصفوف المجمعة. |
| الفهرس | int | فهرس الصف/العمود |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


يخفي صفًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


إخفاء عدة صفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| totalRows | int | رقم الصف. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


يستورد مصفوفة من القيم المزدوجة إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| doubleArray | double[] | مصفوفة مزدوجة. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| isVertical | boolean | يحدد استيراد البيانات عمودياً أو أفقياً. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


يستورد مصفوفة ثنائية الأبعاد من القيم المزدوجة إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| doubleArray | double[][] | مصفوفة مزدوجة ثنائية الأبعاد. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


يستورد مصفوفة من الأعداد الصحيحة إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| intArray | int[] | مصفوفة أعداد صحيحة. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| isVertical | boolean | يحدد استيراد البيانات عمودياً أو أفقياً. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


يستورد مصفوفة ثنائية الأبعاد من الأعداد الصحيحة إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| intArray | int[][] | مصفوفة أعداد صحيحة ثنائية الأبعاد. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


يستورد مصفوفة من السلاسل النصية إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringArray | java.lang.String[] | مصفوفة سلاسل. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| isVertical | boolean | يحدد استيراد البيانات عمودياً أو أفقياً. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


يستورد مصفوفة ثنائية الأبعاد من السلاسل النصية إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringArray | java.lang.String[][] | مصفوفة سلاسل ثنائية الأبعاد. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


يستورد قائمة مصفوفية من البيانات إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayList | java.util.ArrayList | قائمة بيانات arraylist. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| isVertical | boolean | يحدد استيراد البيانات عمودياً أو أفقياً. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


استيراد ملف CSV إلى الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق ملف CSV. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | خيارات التحميل لقراءة ملف نصي |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


استيراد ملف CSV إلى الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | دفق ملف CSV. |
| splitter | java.lang.String | المقسم |
| convertNumericData | boolean | ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


استيراد ملف CSV إلى الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف CSV. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | خيارات التحميل لقراءة ملف نصي |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


استيراد ملف CSV إلى الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف CSV. |
| splitter | java.lang.String | المقسم |
| convertNumericData | boolean | ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


يستورد كائنات مخصصة.

**Remarks**

يجب أن تكون الكائنات المخصصة من نفس النوع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قائمة | java.util.Collection | الكائن المخصص |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | خيارات الاستيراد. |

**Returns:**
int - إجمالي عدد الصفوف المستوردة.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


يستورد كائنات مخصصة.

**Remarks**

يجب أن تكون الكائنات المخصصة من نفس النوع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قائمة | java.util.Collection | الكائن المخصص |
| propertyNames | java.lang.String[] | أسماء الخصائص. إذا كانت null، سنستورد جميع خصائص الكائن. |
| isPropertyNameShown | boolean | يشير إلى ما إذا كان اسم الخاصية سيُستورد إلى الصف الأول. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| rowNumber | int | عدد الصفوف التي سيتم استيرادها. |
| insertRows | boolean | يشير إلى ما إذا كانت الصفوف الإضافية تُضاف لتناسب البيانات. |
| dateFormatString | java.lang.String | سلسلة تنسيق التاريخ للخلايا. |
| convertStringToNumber | boolean | يشير إلى ما إذا كانت هذه الطريقة ستحاول تحويل السلسلة إلى رقم. |

**Returns:**
int - إجمالي عدد الصفوف المستوردة.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


استيراد البيانات من جدول بيانات مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | جدول البيانات المخصص. |
| firstRow | int | فهرس الصف الأول. |
| firstColumn | int | فهرس العمود الأول. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | خيارات الاستيراد |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


يستورد مصفوفة من الصيغ إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringArray | java.lang.String[] | مصفوفة الصيغة. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| isVertical | boolean | يحدد استيراد البيانات عمودياً أو أفقياً. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


يستورد مصفوفة من البيانات إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| objArray | java.lang.Object[] | مصفوفة البيانات. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| isVertical | boolean | يحدد استيراد البيانات عمودياً أو أفقياً. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


يستورد مصفوفة من البيانات إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| objArray | java.lang.Object[] | مصفوفة البيانات. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| isVertical | boolean | يحدد استيراد البيانات عمودياً أو أفقياً. |
| تخطي | int | تم تخطي عدد الصفوف أو الأعمدة. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


يستورد البيانات من كائن ResultSet إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | كائن ResultSet للاستيراد منه. |
| rowIndex | int | فهرس الصف الابتدائي في ورقة العمل. |
| columnIndex | int | فهرس العمود الابتدائي في ورقة العمل. |
| isFieldNameShown | boolean | يشير إلى ما إذا كان اسم الحقل في resultset سيُستورد إلى الصف الأول. |

**Returns:**
int - عدد الصفوف التي تم استيرادها فعليًا.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


يستورد البيانات من كائن ResultSet إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | كائن ResultSet للاستيراد منه. |
| rowIndex | int | فهرس الصف الابتدائي في ورقة العمل. |
| columnIndex | int | فهرس العمود الابتدائي في ورقة العمل. |
| isFieldNameShown | boolean | يشير إلى ما إذا كان اسم الحقل في resultset سيُستورد إلى الصف الأول. |
| customDateFormatString | java.lang.String | سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيمة تاريخ. |
| convertStringToNumber | boolean | يشير إلى ما إذا كانت هذه الطريقة ستحاول تحويل السلسلة إلى رقم. |

**Returns:**
int - عدد الصفوف التي تم استيرادها فعليًا.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


يستورد البيانات من كائن ResultSet إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | كائن ResultSet للاستيراد منه. |
| rowIndex | int | فهرس الصف الابتدائي في ورقة العمل. |
| columnIndex | int | فهرس العمود الابتدائي في ورقة العمل. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | خيارات الاستيراد |

**Returns:**
int - عدد الصفوف التي تم استيرادها فعليًا.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


يستورد البيانات من كائن ResultSet إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | كائن ResultSet للاستيراد منه. |
| rowIndex | int | فهرس الصف الابتدائي في ورقة العمل. |
| columnIndex | int | فهرس العمود الابتدائي في ورقة العمل. |
| rowNum | int | عدد الصفوف للاستيراد. -1 لاستيراد جميع السجلات في resultset المحدد. |
| columnNum | int | عدد الأعمدة للاستيراد. -1 لاستيراد جميع الأعمدة في resultset المحدد. |
| isFieldNameShown | boolean | يشير إلى ما إذا كان اسم الحقل في resultset سيُستورد إلى الصف الأول. |

**Returns:**
int - عدد الصفوف التي تم استيرادها فعليًا.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


يستورد البيانات من كائن ResultSet إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | كائن ResultSet للاستيراد منه. |
| rowIndex | int | فهرس الصف الابتدائي في ورقة العمل. |
| columnIndex | int | فهرس العمود الابتدائي في ورقة العمل. |
| rowNum | int | عدد الصفوف للاستيراد. -1 لاستيراد جميع السجلات في resultset المحدد. |
| columnNum | int | عدد الأعمدة للاستيراد. -1 لاستيراد جميع الأعمدة في resultset المحدد. |
| isFieldNameShown | boolean | يشير إلى ما إذا كان اسم الحقل في resultset سيُستورد إلى الصف الأول. |
| customDateFormatString | java.lang.String | سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيمة تاريخ. |
| convertStringToNumber | boolean | يشير إلى ما إذا كانت هذه الطريقة ستحاول تحويل السلسلة إلى رقم. |

**Returns:**
int - عدد الصفوف التي تم استيرادها فعليًا.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


يستورد البيانات من كائن ResultSet إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | كائن ResultSet للاستيراد منه. |
| startCell | java.lang.String | اسم الخلية الابتدائية لإدراج resultset، مثل "A1". |
| isFieldNameShown | boolean | يشير إلى ما إذا كان اسم الحقل في resultset سيُستورد إلى الصف الأول. |

**Returns:**
int - عدد الصفوف التي تم استيرادها فعليًا.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


يستورد البيانات من كائن ResultSet إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | كائن ResultSet للاستيراد منه. |
| startCell | java.lang.String | اسم الخلية الابتدائية لإدراج resultset، مثل "A1". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | خيارات الاستيراد |

**Returns:**
int - عدد الصفوف التي تم استيرادها فعليًا.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


يستورد البيانات من كائن ResultSet إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | كائن ResultSet للاستيراد منه. |
| startCell | java.lang.String | اسم الخلية الابتدائية لإدراج resultset، مثل "A1". |
| rowNum | int | عدد الصفوف للاستيراد. -1 لاستيراد جميع السجلات في resultset المحدد. |
| columnNum | int | عدد الأعمدة للاستيراد. -1 لاستيراد جميع الأعمدة في resultset المحدد. |
| isFieldNameShown | boolean | يشير إلى ما إذا كان اسم الحقل في resultset سيُستورد إلى الصف الأول. |

**Returns:**
int - عدد الصفوف التي تم استيرادها فعليًا.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


يستورد مصفوفة ثنائية الأبعاد من البيانات إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| objArray | java.lang.Object[][] | مصفوفة بيانات ثنائية الأبعاد. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


يستورد مصفوفة ثنائية الأبعاد من البيانات إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| objArray | java.lang.Object[][] | مصفوفة بيانات ثنائية الأبعاد. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| convertStringToNumber | boolean | يشير إلى ما إذا كانت هذه الطريقة ستحاول تحويل السلسلة إلى رقم. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


يستورد مصفوفة ثنائية الأبعاد من البيانات إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| objArray | java.lang.Object[][] | مصفوفة بيانات ثنائية الأبعاد. |
| أنماط | java.lang.Object[][] | نمط بيانات ثنائي الأبعاد. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| convertStringToNumber | boolean | يشير إلى ما إذا كانت هذه الطريقة ستحاول تحويل السلسلة إلى رقم. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


يستورد مصفوفة ثنائية الأبعاد من البيانات إلى ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| objArray | java.lang.Object[][] | مصفوفة بيانات ثنائية الأبعاد. |
| أنماط | java.lang.Object[][] | نمط بيانات ثنائي الأبعاد. |
| firstRow | int | رقم الصف للخلية الأولى التي يتم الاستيراد فيها. |
| firstColumn | int | رقم العمود للخلية الأولى التي يتم الاستيراد فيها. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | خيارات تحويل قيم السلاسل. |

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

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


يدرج بعض الأعمدة في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| totalColumns | int | عدد الأعمدة. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | خيارات عملية الإدراج. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


إدراج نطاق مقطوع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | نطاق القطع. |
| صف | int | الصف. |
| عمود | int | العمود. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). يوضح كيفية إزاحة الكائنات الأخرى في النطاق المستهدف عند إدراج النطاق المقصوص. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | إزاحة المنطقة. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). خيار إزاحة الخلايا. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | إزاحة المنطقة. |
| shiftNumber | int | عدد الصفوف أو الأعمدة التي سيتم إدراجها. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). خيار إزاحة الخلايا. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | إزاحة المنطقة. |
| shiftNumber | int | عدد الصفوف أو الأعمدة التي سيتم إدراجها. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). خيار إزاحة الخلايا. |
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

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


يدرج عدة صفوف في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| totalRows | int | عدد الصفوف التي سيتم إدراجها. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | خيارات عملية الإدراج. |

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
### isDefaultColumnHidden() {#isDefaultColumnHidden--}
```
public boolean isDefaultColumnHidden()
```




**Returns:**
boolean
### isDefaultRowHeightMatched() {#isDefaultRowHeightMatched--}
```
public boolean isDefaultRowHeightMatched()
```


يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


يشير إلى ما إذا كان الصف مخفيًا افتراضيًا.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


تحقق مما إذا كان يمكن حذف النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس صف البداية للنطاق. |
| startColumn | int | فهرس عمود البداية للنطاق. |
| totalRows | int | عدد الصفوف في النطاق. |
| totalColumns | int | عدد الأعمدة في النطاق. |

**Returns:**
boolean -
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


يحصل على مُعدِّد الخلايا.

**Remarks**

عند تجوال العناصر باستخدام الـ Enumerator المُرجَع، يجب عدم تعديل مجموعة الخلايا (مثل العمليات التي قد تُنشئ خلية/صف جديد أو تحذف خلية/صف موجود). وإلا قد لا يتمكن الـ enumerator من تجوال جميع الخلايا بشكل صحيح (قد يتم تجوال بعض العناصر أكثر من مرة أو يتم تخطيها).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - مُعدِّد الخلايا
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


رابط إلى خريطة XML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| mapName | java.lang.String | اسم خريطة XML |
| صف | int | صف الخلية الوجهة |
| عمود | int | عمود الخلية الوجهة |
| المسار | java.lang.String | مسار عنصر XML في خريطة XML |

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

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


يدمج نطاقًا محددًا من الخلايا في خلية واحدة.

**Remarks**

قم بالإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق. إذا كان mergeConflict صحيحًا وتعارض النطاق المدمج مع خلايا مدمجة أخرى، سيتم إزالة الخلايا المدمجة الأخرى تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول في هذا النطاق (مؤشر صفر) |
| firstColumn | int | العمود الأول في هذا النطاق (مؤشر صفر) |
| totalRows | int | عدد الصفوف (مؤشر واحد) |
| totalColumns | int | عدد الأعمدة (مستند إلى الواحد) |
| mergeConflict | boolean | نطاقات مدمجة متعارضة. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


يدمج نطاقًا محددًا من الخلايا في خلية واحدة.

**Remarks**

قم بالإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق. إذا كان mergeConflict صحيحًا وتعارض النطاق المدمج مع خلايا مدمجة أخرى، سيتم إزالة الخلايا المدمجة الأخرى تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول في هذا النطاق (مؤشر صفر) |
| firstColumn | int | العمود الأول في هذا النطاق (مؤشر صفر) |
| totalRows | int | عدد الصفوف (مؤشر واحد) |
| totalColumns | int | عدد الأعمدة (مستند إلى الواحد) |
| checkConflict | boolean | يشير إلى ما إذا كان فحص الخلايا المدمجة يتقاطع مع خلايا مدمجة أخرى |
| mergeConflict | boolean | نطاقات مدمجة متعارضة. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


ينقل النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | النطاق الذي يجب تحريكه. |
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




### removeDuplicates() {#removeDuplicates--}
```
public void removeDuplicates()
```


يزيل الصفوف المكررة في الورقة.

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


يزيل القيم المكررة في النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية. |
| startColumn | int | عمود البداية |
| endRow | int | فهرس صف النهاية. |
| endColumn | int | فهرس عمود النهاية. |

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


يزيل البيانات المكررة في النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية. |
| startColumn | int | عمود البداية |
| endRow | int | فهرس صف النهاية. |
| endColumn | int | فهرس عمود النهاية. |
| hasHeaders | boolean | يشير إلى ما إذا كان النطاق يحتوي على رؤوس. |
| columnOffsets | int[] | إزاحات العمود. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


يزيل جميع الصيغ ويستبدلها بقيمة الصيغة.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


يسترجع إعدادات المجاميع الفرعية للنطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


يضبط عرض العمود المحدد في العرض العادي.

**Remarks**

في جداول البيانات، يتم قياس عرض العمود كعدد الأحرف لعرض الرقم الأقصى للأرقام 0~9 كما يتم عرضها في خط النمط العادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| العرض | double | عرض العمود بوحدة الأحرف. يجب أن يكون عرض العمود بين 0 و 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


يضبط عرض العمود بوحدة البوصة في العرض العادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| inches | double | عدد البوصات. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


يضبط عرض العمود بوحدة البكسل في العرض العادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| pixels | int | عدد البكسلات. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


يشير إلى ما إذا كان الصف مخفيًا افتراضيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


يضبط خيار استخدام الذاكرة لهذه الخلايا.

انظر [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

القيود الملحوظة والعمليات الموصى بها لبعض الأنماط:

| الوضع | ملاحظات | مدعوم |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | عند استخدام هذا الوضع لأي ورقة عمل في دفتر واحد، يجب استدعاء [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) في نهاية العمل لإطلاق جميع الموارد مثل الملفات المؤقتة. |
 
الوصول العشوائي إلى الخلايا سيؤدي إلى أداء ضعيف لأن البيانات تحتاج إلى القراءة/التحديث عشوائيًا وبشكل متكرر (لذلك سيتغير المؤشر في الملف وفقًا لذلك وستُطلب عمليات إدخال/إخراج متكررة). إذا أمكن، يرجى دائمًا الوصول إلى البيانات بشكل متسلسل (صفًا بصف).
 
عند تغيير بيانات صف/خلية واحدة، قد تتأثر بيانات الخلايا/الصفوف الأخرى (مثل تحريك البيانات إلى أماكن أخرى لتخصيص مساحة كافية للبيانات المتغيرة). لذا كل تغيير في أي بيانات يتطلب مزامنة الكائنات الموجودة الأخرى (مثل كائن الصف أو الخلية). لذلك، للحصول على أداء أفضل، يرجى عدم الحفاظ على عدة صفوف/خلايا في الوقت نفسه. معالجة كل واحدة على حدة سيقلل من مزامنة البيانات وبالتالي يمكن تحسين الأداء قليلاً. | v25.7     |

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


يضبط ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة المتعددة الخيوط Multi-Thread. القيمة الافتراضية لهذه الخاصية هي false.

**Remarks**

إذا كان هناك عدة خيوط لقراءة كائنات Row/Cell في هذه المجموعة بشكل متزامن، يجب ضبط هذه الخاصية على true، وإلا قد يتم إنتاج نتيجة غير متوقعة. قد يؤدي دعم القراءة متعددة الخيوط إلى تدهور الأداء عند الوصول إلى كائنات Row/Cell من هذه المجموعة. يرجى ملاحظة أن بعض الميزات لا يمكنها دعم القراءة متعددة الخيوط، مثل تنسيق القيم (عن طريق [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), إلخ). لذلك، حتى إذا تم ضبط هذه الخاصية على true، قد لا تزال تلك APIs تعطي نتائج غير متوقعة للقراءة متعددة الخيوط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت جميع قيم ورقة العمل محفوظة كسلاسل. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


يضبط ارتفاع الصف المحدد.

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

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


يضبط ارتفاع الصف الافتراضي في هذه ورقة العمل، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


يضبط ارتفاع الصف الافتراضي في هذه ورقة العمل، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


يضبط ارتفاع الصف الافتراضي في هذه ورقة العمل، بوحدة البكسل.

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

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


يضبط النمط الافتراضي لورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


يضبط عرض العمود في عرض مختلف.

**Remarks**

إذا كان نوع العرض الحالي هو [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW)، يكون عرض العمود مساويًا للعرض المطبوع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | The column index. |
| pixels | int | العرض بوحدة البكسل. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


يوسع الصفوف/الأعمدة المجمعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isVertical | boolean | صحيح، يوسع الصفوف المجمعة. |
| الفهرس | int | فهرس الصف/العمود |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


ينشئ المجاميع الفرعية للنطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق |
| groupBy | int | الحقل لتجميعه، كإزاحة عددية تبدأ من الصفر |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). دالة المجموع الفرعي. |
| totalList | int[] | مصفوفة من إزاحات الحقول التي تبدأ من الصفر، تشير إلى الحقول التي تُضاف إليها المجاميع الفرعية. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


ينشئ المجاميع الفرعية للنطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق |
| groupBy | int | الحقل لتجميعه، كإزاحة عددية تبدأ من الصفر |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). دالة المجموع الفرعي. |
| totalList | int[] | مصفوفة من إزاحات الحقول التي تبدأ من الصفر، تشير إلى الحقول التي تُضاف إليها المجاميع الفرعية. |
| replace | boolean | يشير إلى ما إذا كان سيستبدل المجاميع الفرعية الحالية |
| pageBreaks | boolean | يشير إلى ما إذا كان سيضيف فاصل صفحة بين المجموعات |
| summaryBelowData | boolean | يشير إلى ما إذا كان سيضيف ملخصًا أسفل البيانات. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


يقسم المحتوى في العمود المحدد إلى أعمدة متعددة..

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |
| totalRows | int | عدد الصفوف. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | خيارات التقسيم. |

**Returns:**
int - إجمالي عدد الأعمدة لقيم التقسيم.
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

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


يفك تجميع الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول الذي سيتم فك تجميعه. |
| lastIndex | int | فهرس الصف الأخير الذي سيتم فك تجميعه. |
| isAll | boolean | صحيح، يزيل جميع معلومات التجميع. وإلا، يزيل معلومات المجموعة الخارجية. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


يكشف عن عمود

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| العرض | double | عرض العمود. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


يكشف عن عدة أعمدة.

**Remarks**

يطبق عرض العمود فقط على الأعمدة المخفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| totalColumns | int | رقم العمود |
| العرض | double | عرض العمود. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


يكشف عن صف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| الارتفاع | double | ارتفاع الصف. سيتغير ارتفاع الصف فقط عندما يكون الصف مخفيًا وتكون قيمة الارتفاع المعطاة موجبة. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


يكشف عن الصفوف المخفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| totalRows | int | رقم الصف. |
| الارتفاع | double | ارتفاع الصف. سيتغير ارتفاع الصف فقط عندما يكون الصف مخفيًا وتكون قيمة الارتفاع المعطاة موجبة. |

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

