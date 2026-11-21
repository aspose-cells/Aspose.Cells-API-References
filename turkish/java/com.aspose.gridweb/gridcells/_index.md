---
title: "GridCells"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

Bir [GridCell](../../com.aspose.gridweb/gridcell) nesneleri koleksiyonunu kapsar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Hücrenin adını satır ve sütun indekslerine göre alır. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | Hücre satır ve sütun indekslerini adına göre alır. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Belirtilen hücre satır ve sütun indekslerinde [GridCell](../../com.aspose.gridweb/gridcell) öğesini veya null değerini alır. |
| [checkColumn(int col)](#checkColumn-int-) | Belirtilen sütun indeksinde [GridColumn](../../com.aspose.gridweb/gridcolumn) öğesini veya null değerini alır. |
| [checkRow(int i)](#checkRow-int-) | Belirtilen hücre satır indeksinde [GridRow](../../com.aspose.gridweb/gridrow) öğesini veya null değerini alır. |
| [clear()](#clear--) | Koleksiyondaki tüm hücreleri temizle. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | Bir aralığın içeriğini temizler. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Bir aralığın içeriğini temizler. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | Bir aralığın biçimlendirmesini temizler. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Bir aralığın biçimlendirmesini temizler. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Sütun indeksine göre sütun adını alır. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Sütun adına göre sütun indeksini alır. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | Bir bütün sütunun veri ve biçimlendirmesini kopyalar. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | Bir bütün sütunun veri ve biçimlendirmesini kopyalar. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | Bir bütün satırın veri ve biçimlendirmesini kopyalar. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | Bazı bütün satırların veri ve biçimlendirmesini kopyalar. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Veri içermeyen tüm boş sütunları sil. |
| [deleteBlankRows()](#deleteBlankRows--) | Veri içermeyen tüm boş satırları sil. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Bir sütun siler. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Bir sütun siler. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Birkaç sütun siler. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Bir hücre aralığını siler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Bir satır siler. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Birçok satırı siler. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Çalışma sayfasındaki birden fazla satırı siler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | [GridCells](../../com.aspose.gridweb/gridcells) koleksiyonundaki verileri iki boyutlu dizi nesnesine aktarır. |
| [get(int row, int column)](#get-int-int-) | Belirtilen hücre satır ve sütun indekslerinde [GridCell](../../com.aspose.gridweb/gridcell) öğesini alır. |
| [get(String cellName)](#get-java.lang.String-) | Belirtilen hücre adında [GridCell](../../com.aspose.gridweb/gridcell) öğesini alır. |
| [getCell(int row, int column)](#getCell-int-int-) | Belirtilen hücre satır ve sütun indekslerinde [GridCell](../../com.aspose.gridweb/gridcell) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Belirtilen sütunun genişliğini alır. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Belirtilen sütunun genişliğini inç biriminde alır. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Belirtilen sütunun genişliğini piksel biriminde alır. |
| [getColumns()](#getColumns--) | Bu çalışma sayfasındaki bireysel sütunları temsil eden [GridColumn](../../com.aspose.gridweb/gridcolumn) nesnelerinin koleksiyonunu alır. |
| [getCount()](#getCount--) | Hücre sayısını alır. |
| [getFirstCell()](#getFirstCell--) | Bu çalışma sayfasındaki ilk hücreyi alır. |
| [getLastCell()](#getLastCell--) | Bu çalışma sayfasındaki son hücreyi alır. |
| [getMaxColumn()](#getMaxColumn--) | Veri veya stil içeren hücrenin maksimum sütun indeksi. |
| [getMaxDataColumn()](#getMaxDataColumn--) | Veri içeren hücrenin maksimum sütun indeksi. |
| [getMaxDataRow()](#getMaxDataRow--) | Veri içeren hücrenin maksimum satır indeksi. |
| [getMaxRow()](#getMaxRow--) | Veri veya stil içeren hücrenin maksimum satır indeksi. |
| [getMergedCells()](#getMergedCells--) | Birleştirilmiş hücrelerin koleksiyonunu alır. |
| [getMinColumn()](#getMinColumn--) | Koleksiyonda örneklenmiş olan hücrelerin minimum sütun indeksi (tüm sütun için stil tanımlı olup, içinde hücre örneklenmemiş sütunu içermez). |
| [getMinDataColumn()](#getMinDataColumn--) | Veri içeren hücrenin minimum sütun indeksi. |
| [getMinDataRow()](#getMinDataRow--) | Veri içeren hücrenin minimum satır indeksi. |
| [getMinRow()](#getMinRow--) | Veri veya stil içeren hücrenin minimum satır indeksi. |
| [getRow(int i)](#getRow-int-) | Belirtilen hücre satır indeksinde [GridRow](../../com.aspose.gridweb/gridrow) öğesini alır. |
| [getRowEnumerator()](#getRowEnumerator--) | Satırların yineleyicisini alır |
| [getRowHeight(int row)](#getRowHeight-int-) | Belirtilen bir satırın yüksekliğini alır. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Belirtilen satırın yüksekliğini inç biriminde alır. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Belirtilen satırın yüksekliğini piksel biriminde alır. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | Satırın dış hat seviyesini alır. |
| [getRows()](#getRows--) | Bu çalışma sayfasındaki bireysel satırları temsil eden [GridRow](../../com.aspose.gridweb/gridrow) nesnelerinin koleksiyonunu alır. |
| [getStandardHeight()](#getStandardHeight--) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini, puan biriminde alır. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini, piksel biriminde alır. |
| [getStandardWidth()](#getStandardWidth--) | Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde alır. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde alır. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde alır. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Farklı görünüm türlerinde genişliği al. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Sütunları gruplar. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Sütunları gruplar. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Satırları gruplar. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Bir sütunu gizler. |
| [hideRow(int row)](#hideRow-int-) | Bir satırı gizler. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Çalışma sayfasına yeni bir sütun ekler. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Çalışma sayfasına yeni bir sütun ekler. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Çalışma sayfasına bazı sütunlar ekler. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Çalışma sayfasına bazı sütunlar ekler. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [insertRow(int rowIndex)](#insertRow-int-) | Çalışma sayfasına yeni bir satır ekler. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Çalışma sayfasına birden fazla satır ekler. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Çalışma sayfasına birden fazla satır ekler. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Verilen sütunun boş olup olmadığını (herhangi bir veri içermediğini) kontrol eder. |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Belirtilen indeksteki sütunun gizli olup olmadığını kontrol eder. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Belirtilen indeksteki satırın gizli olup olmadığını kontrol eder. |
| [iterator()](#iterator--) | Satırların yineleyicisini alır |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Belirtilen hücre aralığını tek bir hücrede birleştirir. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | Aralığı taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Aralıktaki yinelenen değerleri kaldır. |
| [removeFormulas()](#removeFormulas--) | Tüm formülleri kaldırır ve formül değerleriyle değiştirir. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | Bir hücre aralığı için kenarlıkları ayarlar. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Belirtilen sütunun genişliğini ayarlar. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Sütun genişliğini inç biriminde ayarlar. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | Sütun genişliğini piksel biriminde ayarlar. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Belirtilen satırın yüksekliğini ayarlar. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Satır yüksekliğini inç biriminde ayarlar. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Satır yüksekliğini piksel biriminde ayarlar. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | Satırın dış hat seviyesini ayarlar. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Bu çalışma sayfasında varsayılan satır yüksekliğini puan biriminde ayarlar. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Bu çalışma sayfasında varsayılan satır yüksekliğini piksel biriminde ayarlar. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde ayarlar. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde ayarlar. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde ayarlar. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | Belirtilen hücre aralığına stili uygular. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | Belirtilen hücre aralığına stili uygular. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | Belirtilen sütun indeksine göre bir çalışma sayfası aralığındaki verileri yukarıdan aşağıya artan/azalan şekilde sıralar. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | Belirtilen sütun indeksine göre bir çalışma sayfası aralığındaki verileri yukarıdan aşağıya artan/azalan şekilde sıralar. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Birleştirilmiş hücrelerin belirtilen aralığının birleştirmesini kaldırır. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Sütunların gruplamasını kaldırır. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Satırların gruplamasını kaldırır. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Bir sütunun gizliliğini kaldırır |
| [unhideRow(int row)](#unhideRow-int-) | Bir satırın gizliliğini kaldırır. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Hücrenin adını satır ve sütun indekslerine göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Hücre adı.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


Hücre satır ve sütun indekslerini adına göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücrenin adı. |
| satır | int | Çıktı satır indeksi |
| sütun | int | Çıktı sütun indeksi |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


Belirtilen hücre satır ve sütun indekslerinde [GridCell](../../com.aspose.gridweb/gridcell) öğesini veya null değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |
| sütun | int | Sütun indeksi |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


Belirtilen sütun indeksinde [GridColumn](../../com.aspose.gridweb/gridcolumn) öğesini veya null değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| col | int | Sütun indeksi. |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


Belirtilen hücre satır indeksinde [GridRow](../../com.aspose.gridweb/gridrow) öğesini veya null değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| i | int | Satır indeksi |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Koleksiyondaki tüm hücreleri temizle.

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


Bir aralığın içeriğini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Temizlenecek aralık. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Bir aralığın içeriğini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endRow | int | Bitiş satır indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


Bir aralığın biçimlendirmesini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Temizlenecek aralık. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Bir aralığın biçimlendirmesini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endRow | int | Bitiş satır indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


Bir aralığın içeriğini ve biçimlendirmesini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Temizlenecek aralık. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Bir aralığın içeriğini ve biçimlendirmesini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endRow | int | Bitiş satır indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Sütun indeksine göre sütun adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Sütun adı.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Sütun adına göre sütun indeksini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnName | java.lang.String | Sütun adı. |

**Returns:**
int - Sütun indeksi.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Bir bütün sütunun veri ve biçimlendirmesini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Kaynak Cells nesnesi kopyalanacak veri ve biçimlendirmeleri içerir. |
| sourceColumnIndex | int | Kaynak sütun indeksi. |
| destinationColumnIndex | int | Hedef sütun indeksi. |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Bir bütün sütunun veri ve biçimlendirmesini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Kaynak Cells nesnesi kopyalanacak veri ve biçimlendirmeleri içerir. |
| sourceColumnIndex | int | Kaynak sütun indeksi. |
| destinationColumnIndex | int | Hedef sütun indeksi. |
| columnNumber | int | Kopyalanan sütun numarası. |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Bir bütün satırın veri ve biçimlendirmesini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Kaynak Cells nesnesi kopyalanacak veri ve biçimlendirmeleri içerir. |
| sourceRowIndex | int | Kaynak satır indeksi. |
| destinationRowIndex | int | Hedef satır indeksi. |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Bazı bütün satırların veri ve biçimlendirmesini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Kaynak Cells nesnesi kopyalanacak veri ve biçimlendirmeleri içerir. |
| sourceRowIndex | int | Kaynak satır indeksi. |
| destinationRowIndex | int | Hedef satır indeksi. |
| rowNumber | int | Kopyalanan satır numarası. |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Veri içermeyen tüm boş sütunları sil.

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Veri içermeyen tüm boş satırları sil.

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Bir sütun siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Bir sütun siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini belirtir. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Birkaç sütun siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |
| totalColumns | int | Silinecek sütun sayısı. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini belirtir. |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Bir hücre aralığını siler ve hücreleri kaydırma seçeneğine göre kaydırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endRow | int | Bitiş satır indeksi. |
| endColumn | int | Bitiş sütun indeksi. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Hücreleri kaydırma seçeneği. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Bir satır siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Birçok satırı siler.

**Remarks**

Silinen aralık tablonun (ListObject) üst kısmını (tamamını değil) içeriyorsa, aralık silinemez ve hiçbir şey yapılmaz. MS Excel gibi çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Silinecek ilk satırın indeksi. |
| totalRows | int | Silinecek satır sayısı. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Çalışma sayfasındaki birden fazla satırı siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |
| totalRows | int | Silinecek satır sayısı. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini belirtir. |

**Returns:**
boolean -
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


[GridCells](../../com.aspose.gridweb/gridcells) koleksiyonundaki verileri iki boyutlu dizi nesnesine aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | int | Dışa aktarılacak satır sayısı |
| totalColumns | int | Dışa aktarılacak sütun sayısı |

**Returns:**
java.lang.Object[][] - Dışa aktarılan hücre değeri dizi nesnesi.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


Belirtilen hücre satır ve sütun indekslerinde [GridCell](../../com.aspose.gridweb/gridcell) öğesini alır.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


Belirtilen hücre adında [GridCell](../../com.aspose.gridweb/gridcell) öğesini alır.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı, sütun harfi ve satır numarası dahil, örneğin A5. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


Belirtilen hücre satır ve sütun indekslerinde [GridCell](../../com.aspose.gridweb/gridcell) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |
| sütun | int | Sütun indeksi |

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


Belirtilen sütunun genişliğini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
double - Sütun genişliği
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Belirtilen sütunun genişliğini inç biriminde alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
double - Sütun genişliği
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Belirtilen sütunun genişliğini piksel biriminde alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
int - Normal görünümde sütun genişliği.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


Bu çalışma sayfasındaki bireysel sütunları temsil eden [GridColumn](../../com.aspose.gridweb/gridcolumn) nesnelerinin koleksiyonunu alır.

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Hücre sayısını alır.

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Bu çalışma sayfasındaki ilk hücreyi alır.

**Remarks**

Çalışma sayfasında veri yoksa null döndürür.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Bu çalışma sayfasındaki son hücreyi alır.

**Remarks**

Çalışma sayfasında veri yoksa null döndürür.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Veri veya stil içeren hücrenin maksimum sütun indeksi.

**Remarks**

Hücre yoksa -1 döndür.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Veri içeren hücrenin maksimum sütun indeksi.

**Remarks**

\-1, veri içeren bir hücre yoksa döndürülür. Bu özellik bir çalışma sayfasındaki tüm hücreleri yinelemek ve kontrol etmek zorundadır, bu yüzden zaman tüketen bir işlemdir ve tekrarlı olarak çağrılmamalıdır.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Veri içeren hücrenin maksimum satır indeksi.

**Remarks**

Veri içeren hücre yoksa -1 döndür.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Veri veya stil içeren hücrenin maksimum satır indeksi.

**Remarks**

Çalışma sayfasında veri veya stil içeren hücre yoksa -1 döndür.

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Birleştirilmiş hücrelerin koleksiyonunu alır.

**Remarks**

Bu koleksiyonda, her öğe bir [GridCellArea](../../com.aspose.gridweb/gridcellarea) yapısıdır ve birleştirilmiş hücrelerin bir alanını temsil eder.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Koleksiyonda örneklenmiş olan hücrelerin minimum sütun indeksi (tüm sütun için stil tanımlı olup, içinde hücre örneklenmemiş sütunu içermez).

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Veri içeren hücrenin minimum sütun indeksi.

**Remarks**

\-1, veri içeren bir hücre yoksa döndürülür. Bu özellik bir çalışma sayfasındaki tüm hücreleri yinelemek ve kontrol etmek zorundadır, bu yüzden zaman tüketen bir işlemdir ve tekrarlı olarak çağrılmamalıdır.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Veri içeren hücrenin minimum satır indeksi.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Veri veya stil içeren hücrenin minimum satır indeksi.

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


Belirtilen hücre satır indeksinde [GridRow](../../com.aspose.gridweb/gridrow) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| i | int | Satır indeksi |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Satırların yineleyicisini alır

**Returns:**
java.util.Iterator - Satırların yineleyicisi.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Belirtilen bir satırın yüksekliğini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |

**Returns:**
double - Satır yüksekliği
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Belirtilen satırın yüksekliğini inç biriminde alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |

**Returns:**
double - Satır yüksekliği
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Belirtilen satırın yüksekliğini piksel biriminde alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |

**Returns:**
int - Satır yüksekliği
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


Satırın dış hat seviyesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | satır indeksi. |

**Returns:**
int - ana hat seviyesi.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


Bu çalışma sayfasındaki bireysel satırları temsil eden [GridRow](../../com.aspose.gridweb/gridrow) nesnelerinin koleksiyonunu alır.

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Bu çalışma sayfasındaki varsayılan satır yüksekliğini, puan biriminde alır.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Bu çalışma sayfasındaki varsayılan satır yüksekliğini, piksel biriminde alır.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde alır.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde alır.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde alır.

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Farklı görünüm türlerinde genişliği al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |

**Returns:**
int - sütun genişliği piksel biriminde
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Sütunları gruplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanacak ilk sütun indeksi. |
| lastIndex | int | Gruplanacak son sütun indeksi. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Sütunları gruplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanacak ilk sütun indeksi. |
| lastIndex | int | Gruplanacak son sütun indeksi. |
| isHidden | boolean | Gruplanan sütunların gizli olup olmadığını belirtir. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Satırları gruplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanacak ilk satır indeksi. |
| lastIndex | int | Gruplanacak son satır indeksi. |

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


Bir sütunu gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Bir satırı gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Çalışma sayfasına yeni bir sütun ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Çalışma sayfasına yeni bir sütun ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Çalışma sayfasına bazı sütunlar ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |
| totalColumns | int | Sütun sayısı. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Çalışma sayfasına bazı sütunlar ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |
| totalColumns | int | Sütun sayısı. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Alanı kaydır. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Hücreleri kaydırma seçeneği. |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Alanı kaydır. |
| shiftNumber | int | Eklenecek satır veya sütun sayısı. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Hücreleri kaydırma seçeneği. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini belirtir. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Çalışma sayfasına yeni bir satır ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Çalışma sayfasına birden fazla satır ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |
| totalRows | int | Eklenecek satır sayısı. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Çalışma sayfasına birden fazla satır ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |
| totalRows | int | Eklenecek satır sayısı. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Verilen sütunun boş olup olmadığını (herhangi bir veri içermediğini) kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | sütun indeksi |

**Returns:**
boolean - verilen sütun herhangi bir veri içermiyorsa true
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Belirtilen indeksteki sütunun gizli olup olmadığını kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | sütun indeksi |

**Returns:**
boolean - sütun gizli ise true.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Belirtilen indeksteki satırın gizli olup olmadığını kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | satır indeksi |

**Returns:**
boolean - satır gizli ise true
### iterator() {#iterator--}
```
public Iterator iterator()
```


Satırların yineleyicisini alır

**Returns:**
java.util.Iterator - Satırların yineleyicisi
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Belirtilen hücre aralığını tek bir hücrede birleştirir.

**Remarks**

Aralıktaki sol üst hücrenin adresi üzerinden birleştirilmiş hücreye referans ver.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | int | Bu aralığın ilk sütunu (sıfır tabanlı) |
| totalRows | int | Satır sayısı (bir tabanlı) |
| totalColumns | int | Sütun sayısı (bir tabanlı) |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


Aralığı taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Taşınması gereken aralık. |
| destRow | int | Hedef satır. |
| destColumn | int | Hedef sütun. |

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


Aralıktaki yinelenen değerleri kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satırı. |
| startColumn | int | Başlangıç sütunu |
| endRow | int | Bitiş satır indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Tüm formülleri kaldırır ve formül değerleriyle değiştirir.

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


Bir hücre aralığı için kenarlıkları ayarlar.

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Aralığın ilk satır numarası (sıfır tabanlı). |
| firstColumn | int | Aralığın ilk sütun numarası (sıfır tabanlı). |
| rowNumber | int | Satır sayısı. |
| columnNumber | int | Sütun sayısı. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). Kenarlık konumu. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Kenarlık stili. |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Belirtilen sütunun genişliğini ayarlar.

**Remarks**

Bir sütunu gizlemek için, sütun genişliğini sıfıra ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| genişlik | double | Sütun genişliği. Sütun genişliği 0 ile 255 arasında olmalıdır. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Sütun genişliğini inç biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| inç | double | İnç sayısı. |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


Sütun genişliğini piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| piksel | int | Piksel sayısı. |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Belirtilen satırın yüksekliğini ayarlar.

**Remarks**

Bir satırı gizlemek için, satır yüksekliğini sıfıra ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| yükseklik | double | Satır yüksekliği. Nokta biriminde ve 0 ile 409.5 arasında olmalıdır. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Satır yüksekliğini inç biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| inç | double | İnç sayısı. 0 ile 409.5/72 arasında olmalıdır. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Satır yüksekliğini piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| piksel | int | Piksel sayısı. |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


Satırın dış hat seviyesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | satır indeksi. |
| outlineLevel | int | ana hat seviyesi. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Bu çalışma sayfasında varsayılan satır yüksekliğini puan biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Bu çalışma sayfasında varsayılan satır yüksekliğini piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


Belirtilen hücre aralığına stili uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | int | Bu aralığın ilk sütunu (sıfır tabanlı) |
| rowNumber | int | Satır sayısı (bir tabanlı) |
| columnNumber | int | Sütun sayısı (bir tabanlı) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Ayarlanacak stil nesnesi |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


Belirtilen hücre aralığına stili uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellRange | java.lang.String | Hücre adlarının aralığı, örneğin "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Ayarlanacak stil nesnesi |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


Belirtilen sütun indeksiyle bir Çalışma Sayfası aralığında verileri yukarıdan aşağıya artan/azalan şekilde sıralar. Belirtilen satır indeksiyle bir Çalışma Sayfası aralığında verileri soldan sağa artan/azalan şekilde sıralar.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Sıralanacak ilk hücrenin satır numarası. |
| startColumn | int | Sıralanacak ilk hücrenin sütun numarası. |
| satırlar | int | İçe aktarılacak satır sayısı. |
| sütunlar | int | İçe aktarılacak sütun sayısı. |
| dizin | int | Sıralama sütununu belirten sütun indeksi. Yönlendirme yukarıdan aşağıya ise, sıralama sütununu belirten sütun indeksidir. Yönlendirme soldan sağa ise, sıralama satırını belirten satır indeksidir. |
| isAsending | boolean | sıralama düzeninin artan olup olmadığı . |
| isCaseSensitive | boolean | sıralamanın büyük/küçük harfe duyarlı olup olmadığı . |
| islefttoright | boolean | sıralama yönünün soldan sağa olup olmadığı |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


Belirtilen sütun indeksiyle bir Çalışma Sayfası aralığında verileri yukarıdan aşağıya artan/azalan şekilde sıralar. Belirtilen satır indeksiyle bir Çalışma Sayfası aralığında verileri soldan sağa artan/azalan şekilde sıralar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Sıralanacak ilk hücrenin satır numarası. |
| startColumn | int | Sıralanacak ilk hücrenin sütun numarası. |
| satırlar | int | İçe aktarılacak satır sayısı. |
| sütunlar | int | İçe aktarılacak sütun sayısı. |
| indeksler | int[] | Sıralama sütununu belirten sütun indeks dizisi. Yönlendirme üstten alta ise, sıralama sütununu belirten sütun indeksini temsil eder. Yönlendirme soldan sağa ise, sıralama satırını belirten satır indeksini temsil eder. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). sıralama düzeni dizisi . |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). sıralama yönü |
| isCaseSensitive | boolean | sıralamanın büyük/küçük harfe duyarlı olup olmadığı . |

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


Birleştirilmiş hücrelerin belirtilen aralığının birleştirmesini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | int | Bu aralığın ilk sütunu (sıfır tabanlı) |
| totalRows | int | Satır sayısı (bir tabanlı) |
| totalColumns | int | Sütun sayısı (bir tabanlı) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Sütunların gruplamasını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanması kaldırılacak ilk sütun indeksi. |
| lastIndex | int | Gruplanması kaldırılacak son sütun indeksi. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Satırların gruplamasını kaldırır.

**Remarks**

Yalnızca dış grup bilgilerini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanması kaldırılacak ilk satır indeksi. |
| lastIndex | int | Gruplanması kaldırılacak son satır indeksi. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Bir sütunun gizliliğini kaldırır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| genişlik | double | Sütun genişliği..Sütun genişliği 0 ile 255 arasında olmalıdır |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


Bir satırın gizliliğini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

