---
title: "Cells"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücreyle ilgili nesnelerin bir koleksiyonunu kapsüller, örneğin ...vb."
type: docs
url: /tr/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

Hücreyle ilgili nesnelerin bir koleksiyonunu kapsüller, örneğin [Cell](../../com.aspose.cells/cell), [Row](../../com.aspose.cells/row), ...vb.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | Hücrelere bir aralık nesnesi referansı ekler |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tüm bir sütun için biçimleri uygular. |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tüm bir satır için biçimleri uygular. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tüm bir çalışma sayfası için biçimleri uygular. |
| [checkCell(int row, int column)](#checkCell-int-int-) | Belirtilen hücre satır indeksi ve sütun indeksi için [Cell](../../com.aspose.cells/cell) öğesini veya null değerini alır. |
| [checkColumn(int columnIndex)](#checkColumn-int-) | Belirtilen sütun indeksi için [Column](../../com.aspose.cells/column) öğesini veya null değerini alır. |
| [checkRow(int row)](#checkRow-int-) | Belirtilen hücre satır indeksi için [Row](../../com.aspose.cells/row) öğesini veya null değerini alır. |
| [clear()](#clear--) | Çalışma sayfasının tüm verilerini temizler. |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | Bir aralığın içeriğini temizler. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Bir aralığın içeriğini temizler. |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | Bir aralığın biçimlendirmesini temizler. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Bir aralığın biçimlendirmesini temizler. |
| [clearMergedCells()](#clearMergedCells--) | Tüm birleştirilmiş aralıkları temizler. |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | Çalışma sayfasındaki tüm metin verilerini mümkünse sayısal değere dönüştürür. |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | Tüm bir sütunun verilerini ve biçimlerini kopyalar. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | Tam sütunların veri ve biçimlerini kopyalar. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | Tüm bir sütunun verilerini ve biçimlerini kopyalar. |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | Tüm sütunların veri ve biçimlerini kopyalar. |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | Tam bir satırın veri ve biçimlerini kopyalar. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | Bazı tam satırların veri ve biçimlerini kopyalar. |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | Bazı tam satırların veri ve biçimlerini kopyalar. |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | Bazı tam satırların veri ve biçimlerini kopyalar. |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | Hücre satırlarından veya hücre sütunlarından bir [Range](../../com.aspose.cells/range) nesnesi oluşturur. |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | Hücre aralığından bir [Range](../../com.aspose.cells/range) nesnesi oluşturur. |
| [createRange(String address)](#createRange-java.lang.String-) | Aralık adresinden bir [Range](../../com.aspose.cells/range) nesnesi oluşturur. |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | Hücre aralığından bir [Range](../../com.aspose.cells/range) nesnesi oluşturur. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Veri içermeyen tüm boş sütunları sil. |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | Veri içermeyen tüm boş sütunları sil. |
| [deleteBlankRows()](#deleteBlankRows--) | Veri veya başka bir nesne içermeyen tüm boş satırları sil. |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | Veri veya görünür yorum, pivot tablo gibi bazı özel nesneler içermeyen tüm boş satırları sil. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Bir sütun siler. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Bir sütun siler. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Birkaç sütun siler. |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | Birkaç sütun siler. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Bir hücre aralığını siler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Bir satır siler. |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | Bir satır siler. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Birden fazla satır siler. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Çalışma sayfasındaki birden fazla satırı siler. |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | Çalışma sayfasındaki birden fazla satırı siler. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | Bu sütundaki son hücreyi alır. |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | Bu aralıktaki en yüksek sütun indeksine sahip son hücreyi alır. |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | Bu satırdaki son hücreyi alır. |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | Bu aralıktaki en yüksek satır indeksine sahip son hücreyi alır. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | [Cells](../../com.aspose.cells/cells) koleksiyonundaki verileri iki boyutlu dizi nesnesine dışa aktarır. |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | [Cells](../../com.aspose.cells/cells) koleksiyonundaki hücre değer tipini iki boyutlu dizi nesnesine dışa aktarır. |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | Girdi nesnesini içeren hücreyi bulur. |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | Girdi nesnesini içeren hücreyi bulur. |
| [get(int row, int column)](#get-int-int-) | Belirtilen hücre satır indeksi ve sütun indeksindeki [Cell](../../com.aspose.cells/cell) öğesini alır. |
| [get(String cellName)](#get-java.lang.String-) | Belirtilen hücre adındaki [Cell](../../com.aspose.cells/cell) öğesini alır. |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | Verilen hücrenin görüntü stilini al. |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | Verilen hücrenin görüntü stilini al. |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | Verilen hücrenin stilini al. |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | Gömülü resim içeren tüm hücreleri alır. |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | Sütun gizli ise, orijinal sütunun yüksekliğini puan biriminde alır. |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Normal görünümde belirtilen sütunun genişliğini (karakter biriminde) alır. |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | Sütun genişliğini alır. |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Normal görünümde belirtilen sütunun genişliğini inç biriminde alır. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Normal görünümde belirtilen sütunun genişliğini piksel biriminde alır. |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | Normal görünümde belirtilen sütunun genişliğini piksel biriminde alır. |
| [getColumns()](#getColumns--) | Bu çalışma sayfasındaki bireysel sütunları temsil eden [Column](../../com.aspose.cells/column) nesnelerinin koleksiyonunu alır. |
| [getCount()](#getCount--) | Örneklenmiş Cell nesnelerinin toplam sayısını alır. |
| [getCountLarge()](#getCountLarge--) | Örneklenmiş Cell nesnelerinin toplam sayısını alır. |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | Belirli hücreye referans veren tüm hücreleri al. |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | Hesaplanan sonucu belirli hücreye bağlı olan tüm hücreleri alır. |
| [getFirstCell()](#getFirstCell--) | Bu çalışma sayfasındaki ilk hücreyi alır. |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | Belirtilen sütunda veri içeren hücrenin ilk satır indeksini alır. |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | Sütunun taslak seviyesini (sıfır tabanlı) alır. |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | Satırın taslak seviyesini (sıfır tabanlı) alır. |
| [getLastCell()](#getLastCell--) | Bu çalışma sayfasındaki son hücreyi alır. |
| [getLastDataRow(int column)](#getLastDataRow-int-) | Belirtilen sütunda veri içeren hücrenin son satır indeksini alır. |
| [getMaxColumn()](#getMaxColumn--) | Koleksiyonda örneklenmiş hücrelerin maksimum sütun indeksi (tüm sütun için stil tanımlı ancak içinde hücre örneklenmemiş sütunu içermez). |
| [getMaxDataColumn()](#getMaxDataColumn--) | Veri içeren hücrenin maksimum sütun indeksi. |
| [getMaxDataRow()](#getMaxDataRow--) | Veri içeren hücrenin maksimum satır indeksi. |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | Veri, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığı alır. |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | Maksimum gruplanmış sütun taslak seviyesini (sıfır tabanlı) alır. |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | Maksimum gruplanmış satır taslak seviyesini (sıfır tabanlı) alır. |
| [getMaxRow()](#getMaxRow--) | Veri veya stil içeren hücrenin maksimum satır indeksi. |
| [getMemorySetting()](#getMemorySetting--) | Bu hücreler için bellek kullanımı seçeneğini alır. |
| [getMergedAreas()](#getMergedAreas--) | Tüm birleştirilmiş hücreleri alır. |
| [getMergedCells()](#getMergedCells--) | Birleştirilmiş hücrelerin koleksiyonunu alır. |
| [getMinColumn()](#getMinColumn--) | Koleksiyonda örneklenmiş olan hücrelerin minimum sütun indeksi (tüm sütun için stil tanımlı olup, içinde hücre örneklenmemiş sütunu içermez). |
| [getMinDataColumn()](#getMinDataColumn--) | Veri içeren hücrenin minimum sütun indeksi. |
| [getMinDataRow()](#getMinDataRow--) | Veri içeren hücrenin minimum satır indeksi. |
| [getMinRow()](#getMinRow--) | Veri veya stil içeren hücrenin minimum satır indeksi. |
| [getMultiThreadReading()](#getMultiThreadReading--) | Hücre veri modelinin Çoklu İş Parçacığı okumasını destekleyip desteklemeyeceğini alır. |
| [getOdsCellFields()](#getOdsCellFields--) | ods alanlarının listesini alır. |
| [getPreserveString()](#getPreserveString--) | Tüm çalışma sayfası değerlerinin dize olarak korunup korunmadığını gösteren bir değeri alır. |
| [getRanges()](#getRanges--) | Çalışma zamanında oluşturulan [Range](../../com.aspose.cells/range) nesnelerinin koleksiyonunu alır. |
| [getRowEnumerator()](#getRowEnumerator--) | Satırların yineleyicisini alır. |
| [getRowHeight(int row)](#getRowHeight-int-) | Belirtilen satırın yüksekliğini, nokta biriminde alır. |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | Satır yüksekliğini alır. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Belirtilen satırın yüksekliğini inç biriminde alır. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Belirtilen satırın yüksekliğini piksel biriminde alır. |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | Satır gizli ise orijinal satır yüksekliğini nokta biriminde alır. |
| [getRows()](#getRows--) | Bu çalışma sayfasındaki bireysel satırları temsil eden [Row](../../com.aspose.cells/row) nesnelerinin koleksiyonunu alır. |
| [getStandardHeight()](#getStandardHeight--) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini nokta biriminde alır. |
| [getStandardHeightInch()](#getStandardHeightInch--) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini inç biriminde alır. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini piksel biriminde alır. |
| [getStandardWidth()](#getStandardWidth--) | Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde alır. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde alır. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde alır. |
| [getStyle()](#getStyle--) | Çalışma sayfasının varsayılan stilini alır. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Farklı görünüm türlerinde genişliği al. |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | Belirtilen bir satırın yüksekliğini alır. |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | Belirtilen satırın yüksekliğini inç biriminde alır. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Sütunları gruplar. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Sütunları gruplar. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Satırları gruplar. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Satırları gruplar. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Bir sütunu gizler. |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | Birden fazla sütunu gizler. |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | Gruplanmış satırları/sütunları daraltır. |
| [hideRow(int row)](#hideRow-int-) | Bir satırı gizler. |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | Birden fazla satırı gizler. |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | Bir çalışma sayfasına double dizisini içe aktarır. |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | Bir çalışma sayfasına iki boyutlu double dizisini içe aktarır. |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | Bir çalışma sayfasına integer dizisini içe aktarır. |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | Bir çalışma sayfasına iki boyutlu integer dizisini içe aktarır. |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | Bir çalışma sayfasına string dizisini içe aktarır. |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | Bir çalışma sayfasına iki boyutlu string dizisini içe aktarır. |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | Bir çalışma sayfasına veri arraylist'ini içe aktarır. |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | Hücrelere bir CSV dosyası içe aktar. |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | Hücrelere bir CSV dosyası içe aktar. |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | Hücrelere bir CSV dosyası içe aktar. |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | Hücrelere bir CSV dosyası içe aktar. |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | Özel nesneleri içe aktarır. |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | Özel nesneleri içe aktarır. |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | Özel veri tablosundan verileri içe aktar. |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | Bir çalışma sayfasına formül dizisini içe aktarır. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | Bir çalışma sayfasına veri dizisini içe aktarır. |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | Bir çalışma sayfasına veri dizisini içe aktarır. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır. |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır. |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır. |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır. |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | Bir çalışma sayfasına iki boyutlu veri dizisini içe aktarır. |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | Bir çalışma sayfasına iki boyutlu veri dizisini içe aktarır. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | Bir çalışma sayfasına iki boyutlu veri dizisini içe aktarır. |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | Bir çalışma sayfasına iki boyutlu veri dizisini içe aktarır. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Çalışma sayfasına yeni bir sütun ekler. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Çalışma sayfasına yeni bir sütun ekler. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Çalışma sayfasına bazı sütunlar ekler. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Çalışma sayfasına bazı sütunlar ekler. |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | Çalışma sayfasına bazı sütunlar ekler. |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | Kesilmiş aralığı ekle. |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [insertRow(int rowIndex)](#insertRow-int-) | Çalışma sayfasına yeni bir satır ekler. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Çalışma sayfasına birden fazla satır ekler. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Çalışma sayfasına birden fazla satır ekler. |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | Çalışma sayfasına birden fazla satır ekler. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Verilen sütunun boş olup olmadığını (herhangi bir veri içermediğini) kontrol eder. |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Belirtilen indeksteki sütunun gizli olup olmadığını kontrol eder. |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | Satır yüksekliğinin ve varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | Satırın varsayılan olarak gizli olup olmadığını gösterir. |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | Aralığın silinebilir olup olmadığını kontrol eder. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Belirtilen indeksteki satırın gizli olup olmadığını kontrol eder. |
| [iterator()](#iterator--) | Hücre enumeratörünü alır. |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | Bir XML haritasına bağlantı. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Belirtilen hücre aralığını tek bir hücrede birleştirir. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | Belirtilen hücre aralığını tek bir hücrede birleştirir. |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | Belirtilen hücre aralığını tek bir hücrede birleştirir. |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | Aralığı taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | Sayfadaki yinelenen satırları kaldırır. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Aralıktaki yinelenen değerleri kaldırır. |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | Aralığın yinelenen verilerini kaldırır. |
| [removeFormulas()](#removeFormulas--) | Tüm formülleri kaldırır ve formül değerleriyle değiştirir. |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | Aralığın ara toplam ayarlarını alır. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Normal görünümde belirtilen sütunun genişliğini ayarlar. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Normal görünümde sütun genişliğini inç biriminde ayarlar. |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | Normal görünümde sütun genişliğini piksel biriminde ayarlar. |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | Satır yüksekliğinin ve varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | Satırın varsayılan olarak gizli olup olmadığını gösterir. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Bu hücreler için bellek kullanımı seçeneğini ayarlar. |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | Hücre veri modelinin çoklu iş parçacıklı okuma destekleyip desteklemeyeceğini ayarlar. |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | Tüm çalışma sayfası değerlerinin dize olarak korunup korunmayacağını belirten bir değeri ayarlar. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Belirtilen satırın yüksekliğini ayarlar. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Satır yüksekliğini inç biriminde ayarlar. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Satır yüksekliğini piksel biriminde ayarlar. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini nokta biriminde ayarlar. |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini inç biriminde ayarlar. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini piksel biriminde ayarlar. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde ayarlar. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde ayarlar. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde ayarlar. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Çalışma sayfasının varsayılan stilini ayarlar. |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | Sütunun genişliğini farklı görünümde ayarlar. |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | Gruplanmış satırları/sütunları genişletir. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | Aralık için alt toplamlar oluşturur. |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | Aralık için alt toplamlar oluşturur. |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | Belirtilen sütundaki içeriği birden çok sütuna böler.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Birleştirilmiş hücrelerin belirtilen aralığının birleştirmesini kaldırır. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Sütunların gruplamasını kaldırır. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Satırların gruplamasını kaldırır. |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | Satırların gruplamasını kaldırır. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Bir sütunun gizliliğini kaldırır |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | Birden çok sütunun gizliliğini kaldırır. |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | Bir satırın gizliliğini kaldırır. |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | Gizli satırların gizliliğini kaldırır. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


Hücrelere bir aralık nesnesi referansı ekler

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | Aralık nesnesi hücrelerde bulunacak |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


Tüm bir sütun için biçimleri uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| style | [Style](../../com.aspose.cells/style) | Uygulanacak stil nesnesi. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


Tüm bir satır için biçimleri uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| style | [Style](../../com.aspose.cells/style) | Uygulanacak stil nesnesi. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tüm bir çalışma sayfası için biçimleri uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Uygulanacak stil nesnesi. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


Belirtilen hücre satır indeksi ve sütun indeksi için [Cell](../../com.aspose.cells/cell) öğesini veya null değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |
| sütun | int | Sütun indeksi |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


Belirtilen sütun indeksi için [Column](../../com.aspose.cells/column) öğesini veya null değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


Belirtilen hücre satır indeksi için [Row](../../com.aspose.cells/row) öğesini veya null değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Çalışma sayfasının tüm verilerini temizler.

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


Bir aralığın içeriğini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Temizlenecek aralık. |

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

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


Bir aralığın biçimlendirmesini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Temizlenecek aralık. |

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

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


Tüm birleştirilmiş aralıkları temizler.

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


Bir aralığın içeriğini ve biçimlendirmesini temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | Temizlenecek aralık. |

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

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


Çalışma sayfasındaki tüm metin verilerini mümkünse sayısal değere dönüştürür.

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Tüm bir sütunun verilerini ve biçimlerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Kaynak Hücreler nesnesi kopyalanacak veri ve biçimleri içerir. |
| sourceColumnIndex | int | Kaynak sütun indeksi. |
| destinationColumnIndex | int | Hedef sütun indeksi. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Tam sütunların veri ve biçimlerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Kaynak Hücreler nesnesi kopyalanacak veri ve biçimleri içerir. |
| sourceColumnIndex | int | Kaynak sütun indeksi. |
| destinationColumnIndex | int | Hedef sütun indeksi. |
| columnNumber | int | Kopyalanan sütun numarası. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


Tüm bir sütunun verilerini ve biçimlerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Kaynak Hücreler nesnesi kopyalanacak veri ve biçimleri içerir. |
| sourceColumnIndex | int | Kaynak sütun indeksi. |
| destinationColumnIndex | int | Hedef sütun indeksi. |
| columnNumber | int | Kopyalanan sütun numarası. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | yapıştırma seçenekleri. |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


Tüm sütunların veri ve biçimlerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Kaynak Hücreler nesnesi kopyalanacak veri ve biçimleri içerir. |
| sourceColumnIndex | int | Kaynak sütun indeksi. |
| sourceTotalColumns | int | Kaynak sütunların sayısı. |
| destinationColumnIndex | int | Hedef sütun indeksi. |
| destinationTotalColumns | int | Hedef sütunların sayısı. |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Tam bir satırın veri ve biçimlerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Kaynak Hücreler nesnesi kopyalanacak veri ve biçimleri içerir. |
| sourceRowIndex | int | Kaynak satır indeksi. |
| destinationRowIndex | int | Hedef satır indeksi. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Bazı tam satırların veri ve biçimlerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Kaynak Hücreler nesnesi kopyalanacak veri ve biçimleri içerir. |
| sourceRowIndex | int | Kaynak satır indeksi. |
| destinationRowIndex | int | Hedef satır indeksi. |
| rowNumber | int | Kopyalanan satır numarası. |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


Bazı tam satırların veri ve biçimlerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Kaynak Hücreler nesnesi kopyalanacak veri ve biçimleri içerir. |
| sourceRowIndex | int | Kaynak satır indeksi. |
| destinationRowIndex | int | Hedef satır indeksi. |
| rowNumber | int | Kopyalanan satır numarası. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Kopyalama seçenekleri. |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


Bazı tam satırların veri ve biçimlerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Kaynak Hücreler nesnesi kopyalanacak veri ve biçimleri içerir. |
| sourceRowIndex | int | Kaynak satır indeksi. |
| destinationRowIndex | int | Hedef satır indeksi. |
| rowNumber | int | Kopyalanan satır numarası. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Kopyalama seçenekleri. |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | yapıştırma seçenekleri. |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


Hücre satırlarından veya hücre sütunlarından bir [Range](../../com.aspose.cells/range) nesnesi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | İlk satır indeksi veya ilk sütun indeksi, sıfır tabanlı. |
| sayı | int | Satır veya sütunların toplam sayısı, bir tabanlı. |
| isVertical | boolean | Doğru - Aralık hücrelerin sütunlarından oluşturulur. Yanlış - Aralık hücrelerin satırlarından oluşturulur. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Hücre aralığından bir [Range](../../com.aspose.cells/range) nesnesi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bu aralığın ilk satırı |
| firstColumn | int | Bu aralığın ilk sütunu |
| totalRows | int | Satır sayısı |
| totalColumns | int | Sütun sayısı |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


Aralık adresinden bir [Range](../../com.aspose.cells/range) nesnesi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adres | java.lang.String | Aralığın adresi. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


Hücre aralığından bir [Range](../../com.aspose.cells/range) nesnesi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| upperLeftCell | java.lang.String | Üst sol hücre adı. |
| lowerRightCell | java.lang.String | Alt sağ hücre adı. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Veri içermeyen tüm boş sütunları sil.

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


Veri içermeyen tüm boş sütunları sil.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Aralığı silme seçenekleri. |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Veri veya başka bir nesne içermeyen tüm boş satırları sil.

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


Veri veya görünür yorum, pivot tablo gibi bazı özel nesneler içermeyen tüm boş satırları sil.

**Remarks**

Silinecek boş satırlar için, sadece [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) ifadesinin doğru olması yeterli değildir; aynı zamanda bu satırlardaki hiçbir hücreye tanımlı görünür bir yorum olmamalı ve aralığı onlarla kesişen bir pivot tablo bulunmamalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Aralığı silme seçenekleri. |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Bir sütun siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Silinecek sütunun indeksi. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Bir sütun siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Silinecek sütunun indeksi. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Birkaç sütun siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Silinecek ilk sütunun indeksi. |
| totalColumns | int | Silinecek sütun sayısı. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


Birkaç sütun siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Silinecek ilk sütunun indeksi. |
| totalColumns | int | Silinecek sütun sayısı. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Silme işlemi için seçenekler |

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
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Hücreleri kaydırma seçeneği. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Bir satır siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Silinecek satırın indeksi. |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


Bir satır siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Silinecek satırın indeksi. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Birden fazla satır siler.

**Remarks**

Silinen aralık, tablonun (ListObject) üst kısmını (tamamını değil) içeriyorsa, aralık silinemez ve hiçbir işlem yapılmaz. Bu, MS Excel'de olduğu gibi aynı şekilde çalışır.

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
| rowIndex | int | Silinecek ilk satırın indeksi. |
| totalRows | int | Silinecek satır sayısı. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


Çalışma sayfasındaki birden fazla satırı siler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Silinecek ilk satırın indeksi. |
| totalRows | int | Silinecek satır sayısı. |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | Silme işlemi için seçenekler |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür.

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


Bu sütundaki son hücreyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


Bu aralıktaki en yüksek sütun indeksine sahip son hücreyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| endRow | int | Bitiş satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


Bu satırdaki son hücreyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


Bu aralıktaki en yüksek satır indeksine sahip son hücreyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| endRow | int | Bitiş satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
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


[Cells](../../com.aspose.cells/cells) koleksiyonundaki verileri iki boyutlu dizi nesnesine dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | int | Dışa aktarılacak satır sayısı |
| totalColumns | int | Dışa aktarılacak sütun sayısı |

**Returns:**
java.lang.Object[][] - Dışa aktarılan hücre değeri dizi nesnesi.
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


[Cells](../../com.aspose.cells/cells) koleksiyonundaki hücre değer tipini iki boyutlu dizi nesnesine dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | int | Dışa aktarılacak satır sayısı. |
| totalColumns | int | Dışa aktarılacak sütun sayısı |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype). Hücre değer türlerini temsil eden dışa aktarılmış dizi nesnesi.
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


Girdi nesnesini içeren hücreyi bulur.

**Remarks**

Hiç hücre bulunamazsa null (Nothing) döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ne | java.lang.Object | Aranacak nesne. Türü int, double, DateTime, string, bool olmalıdır. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Aynı nesneye sahip önceki hücre. Bu parametre, baştan arama yapılıyorsa null olarak ayarlanabilir. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


Girdi nesnesini içeren hücreyi bulur.

**Remarks**

Hiç hücre bulunamazsa null (Nothing) döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ne | java.lang.Object | Aranacak nesne. Türü int, double, DateTime, string, bool olmalıdır. |
| previousCell | [Cell](../../com.aspose.cells/cell) | Aynı nesneye sahip önceki hücre. Bu parametre, baştan arama yapılıyorsa null olarak ayarlanabilir. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Bulma seçenekleri |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


Belirtilen hücre satır indeksi ve sütun indeksindeki [Cell](../../com.aspose.cells/cell) öğesini alır.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


Belirtilen hücre adındaki [Cell](../../com.aspose.cells/cell) öğesini alır.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı, sütun harfi ve satır numarası dahil, örneğin A5. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


Verilen hücrenin görüntü stilini al.

**Remarks**

[Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--) ile aynı ve [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) kullanarak [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-) için de aynı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | verilen hücrenin satır indeksi |
| sütun | int | verilen hücrenin sütunu |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


Verilen hücrenin görüntü stilini al.

**Remarks**

Hücre, koşullu biçimlendirme, liste nesneleri vb. gibi diğer ayarlardan da etkileniyorsa, görüntü stili [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-) değerinden farklı olabilir. Ayrıca bu ayarlar boş (var olmayan) hücrelere de uygulanabileceği için, bu yöntemi kullanmak bu boş hücrelerin örneklenmesini önleyebilir; böylece performans, Cells üzerinden Cell örneğini alıp ardından [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-) metodunu çağırmaktan daha iyi olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | verilen hücrenin satır indeksi |
| sütun | int | verilen hücrenin sütunu |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Hangi kenarların komşu hücrelerin kenarlarına göre kontrol edilip ayarlanması gerektiğini gösterir. Aynı parametrenin açıklaması için lütfen [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-) belgesine bakın. |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


Verilen hücrenin stilini al.

**Remarks**

Döndürülen stil yalnızca hücre için ayarlanmış olan veya hücrenin satır/sütunundan devralınan stildir; koşullu biçimlendirme gibi diğer ayarlar tarafından uygulanan özellikleri içermez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | satır indeksi |
| sütun | int | sütun |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


Gömülü resim içeren tüm hücreleri alır.

**Remarks**

Bu çalışma sayfasında "Place in Cell" olarak ayarlanmış bir resim yoksa, null döndürülür.

**Returns:**
java.util.Iterator - Gömülü resim içeren tüm Cell nesnelerini numaralandırmak için Enumerator
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


Sütun gizli ise, orijinal sütunun yüksekliğini puan biriminde alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cells.GetColumnWidth(int ,bool , CellsUnitType ) yöntemini kullanın. Bu yöntem, Nisan 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Satır indeksi. |

**Returns:**
double - Normal görünümde sütun genişliği.
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Normal görünümde belirtilen sütunun genişliğini (karakter biriminde) alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
double - Sütun genişliği. Elektronik tablo için sütun genişliği, normal stilin yazı tipinde 0~9 sayılarının maksimum rakam genişliğine göre karakter sayısı olarak ölçülür.
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


Sütun genişliğini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| isOriginal | boolean | Orijinal genişliğin alınıp alınmadığını gösterir. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Normal görünümde belirtilen sütunun genişliğini inç biriminde alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cells.GetColumnWidth(int ,bool , CellsUnitType ) yöntemini kullanın. Bu yöntem, Nisan 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
double - Normal görünümde sütun genişliği.
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Normal görünümde belirtilen sütunun genişliğini piksel biriminde alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
int - Normal görünümde sütun genişliği.
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


Normal görünümde belirtilen sütunun genişliğini piksel biriminde alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cells.GetColumnWidth(int ,bool , CellsUnitType ) yöntemini kullanın. Bu yöntem, Nisan 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |
| orijinal | boolean | Sütun gizli olsa bile orijinal genişliğin döndürülüp döndürülmediğini gösterir |

**Returns:**
int - Normal görünümde sütun genişliği.
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


Bu çalışma sayfasındaki bireysel sütunları temsil eden [Column](../../com.aspose.cells/column) nesnelerinin koleksiyonunu alır.

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Örneklenmiş Cell nesnelerinin toplam sayısını alır.

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


Örneklenmiş Cell nesnelerinin toplam sayısını alır.

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


Belirli hücreye referans veren tüm hücreleri al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAll | boolean | Diğer çalışma sayfalarının kontrol edilip edilmediğini gösterir |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
com.aspose.cells.Cell[] -
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


Hesaplanan sonucu belirli hücreye bağlı olan tüm hücreleri alır.

**Remarks**

Bu yöntemi kullanmak için, çalışma kitabının [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) için true değerine ayarlandığından ve bu ayarla tamamen hesaplandığından emin olun. Bu hücreye referans veren bir formül yoksa, null döndürülür. Daha fazla detay ve örnek için lütfen [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-) belgesine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Belirli hücrenin satır indeksi |
| sütun | int | Belirli hücrenin sütun indeksi. |
| recursive | boolean | Belirli hücreye doğrudan başvurmayan, ancak o hücrenin diğer yapraklarına başvuran bağımlıların döndürülüp döndürülmeyeceği. |

**Returns:**
java.util.Iterator - Tüm bağımlıları (Cell nesneleri) numaralandırmak için yineleyici
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Bu çalışma sayfasındaki ilk hücreyi alır.

**Remarks**

Çalışma sayfasında veri yoksa null döndürür.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


Belirtilen sütunda veri içeren hücrenin ilk satır indeksini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |

**Returns:**
int - ilk satır indeksi.
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


Sütunun taslak seviyesini (sıfır tabanlı) alır.

**Remarks**

Sütun gruplanmamışsa, sıfır döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi |

**Returns:**
int - Sütunun anahat seviyesi
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


Satırın taslak seviyesini (sıfır tabanlı) alır.

**Remarks**

Satır gruplanmamışsa, sıfır döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |

**Returns:**
int - Satırın anahat seviyesi (sıfır tabanlı).
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Bu çalışma sayfasındaki son hücreyi alır.

**Remarks**

Çalışma sayfasında veri yoksa null döndürür.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


Belirtilen sütunda veri içeren hücrenin son satır indeksini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |

**Returns:**
int - son satır indeksi.
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Koleksiyonda örneklenmiş hücrelerin maksimum sütun indeksi (tüm sütun için stil tanımlı ancak içinde hücre örneklenmemiş sütunu içermez).

**Remarks**

-1 döndürülür, eğer hiç hücre oluşturulmamışsa.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Veri içeren hücrenin maksimum sütun indeksi.

**Remarks**

\-1, veri içeren hücre olmadığında döndürülür. Bu özellik, bir çalışma sayfasındaki tüm hücreleri dinamik olarak yinelemek ve kontrol etmek zorundadır, bu nedenle zaman tüketen bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlı olarak çağrılmamalıdır.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Veri içeren hücrenin maksimum satır indeksi.

**Remarks**

-1 döndürülür, eğer veri içeren hücre yoksa. Bu özellik, hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek zorundadır, bu nedenle zaman tüketen bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlı olarak çağrılmamalıdır.

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


Veri, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığı alır.

**Remarks**

Aspose.Cells 21.5.2'den itibaren, çalışma sayfası boşsa null döndürür.

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


Maksimum gruplanmış sütun taslak seviyesini (sıfır tabanlı) alır.

**Returns:**
int - En yüksek gruplanmış sütun anahat seviyesi (sıfır tabanlı)
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


Maksimum gruplanmış satır taslak seviyesini (sıfır tabanlı) alır.

**Returns:**
int - En yüksek gruplanmış satır anahat seviyesi (sıfır tabanlı)
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Veri veya stil içeren hücrenin maksimum satır indeksi.

**Remarks**

-1 döndürülür, eğer çalışma sayfasında veri veya stil içeren hücre yoksa. Bu özellik, hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek zorundadır, bu nedenle zaman tüketen bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlı olarak çağrılmamalıdır.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Bu hücreler için bellek kullanımı seçeneğini alır.

Bakınız [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Bazı modlar için dikkate değer sınırlamalar ve önerilen işlemler:

| Mod | Açıklamalar | Desteklenen |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Bu mod bir çalışma kitabındaki herhangi bir çalışma sayfası için kullanıldığında, geçici dosyalar gibi tüm kaynakları serbest bırakmak için işin sonunda [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) çağrılmalıdır. |
 
Hücrelere rastgele erişmek, verinin rastgele ve tekrar tekrar okunup güncellenmesi gerektiği için düşük performans verir (dosyadaki işaretçi buna göre değişir ve I/O işlemleri tekrar tekrar gerekir). Mümkünse, veriye her zaman sıralı olarak (satır satır) erişin.
 
Bir satır/hücrenin verisi değiştirildiğinde, diğer hücrelerin/satırların verileri de etkilenebilir (örneğin veri, değişen veri için yeterli alan ayırmak amacıyla başka yerlere kaydırılabilir/taşınabilir). Bu nedenle, her veri değişikliği, diğer mevcut nesnelerin (örneğin Satır veya Hücre nesnesi) senkronizasyonunu gerektirir. Daha iyi performans için, lütfen aynı anda birden fazla Satır/Hücre tutmayın. Onları tek tek işlemek, veri senkronizasyonunu azaltır ve performans biraz artar. | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


Tüm birleştirilmiş hücreleri alır.

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Birleştirilmiş hücrelerin koleksiyonunu alır.

**Remarks**

NOT: Bu yöntem artık eski. Bunun yerine lütfen Cells.GetMergedAreas() yöntemini kullanın. Bu yöntem, Kasım 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Koleksiyonda örneklenmiş olan hücrelerin minimum sütun indeksi (tüm sütun için stil tanımlı olup, içinde hücre örneklenmemiş sütunu içermez).

**Remarks**

Bu özellik, hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek zorundadır, bu yüzden zaman tüketen bir süreçtir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlamalı olarak çağrılmamalıdır.

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Veri içeren hücrenin minimum sütun indeksi.

**Remarks**

\-1, veri içeren hücre olmadığında döndürülür. Bu özellik, bir çalışma sayfasındaki tüm hücreleri dinamik olarak yinelemek ve kontrol etmek zorundadır, bu nedenle zaman tüketen bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlı olarak çağrılmamalıdır.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Veri içeren hücrenin minimum satır indeksi.

**Remarks**

-1 döndürülür, eğer veri içeren hücre yoksa. Bu özellik, hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek zorundadır, bu nedenle zaman tüketen bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlı olarak çağrılmamalıdır.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Veri veya stil içeren hücrenin minimum satır indeksi.

**Remarks**

Bu özellik, hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek zorundadır, bu yüzden zaman tüketen bir süreçtir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlamalı olarak çağrılmamalıdır.

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


Hücre veri modelinin Çok İşlemli (Multi-Thread) okuma desteği sağlayıp sağlamadığını alır. Bu özelliğin varsayılan değeri false'tur.

**Remarks**

Eğer bu koleksiyondaki Row/Cell nesnelerini aynı anda birden fazla iş parçacığı okuyorsa, bu özellik true olarak ayarlanmalıdır, aksi takdirde beklenmeyen sonuçlar ortaya çıkabilir. Çok İşlemli (Multi-Thread) okuma desteği, bu koleksiyondan Row/Cell nesnelerine erişim performansını düşürebilir. Lütfen bazı özelliklerin Çok İşlemli okuma desteklemediğini unutmayın, örneğin değer biçimlendirme ([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), vb.). Bu nedenle, bu özellik true olarak ayarlanmış olsa bile, bu API'ler Çok İşlemli okuma için hâlâ beklenmeyen sonuçlar verebilir.

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


ods alanlarının listesini alır.

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


Tüm çalışma sayfası değerlerinin dize olarak korunup korunmadığını gösteren bir değer alır. Varsayılan değer false'tur.

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


Çalışma zamanında oluşturulan [Range](../../com.aspose.cells/range) nesnelerinin koleksiyonunu alır.

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Satırların yineleyicisini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen RowCollection.GetEnumerator() metodunu kullanın. Bu metod Mayıs 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.util.Iterator - Satırların yineleyicisi.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Belirtilen satırın yüksekliğini, nokta biriminde alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |

**Returns:**
double - Satır yüksekliği
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


Satır yüksekliğini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| isOriginal | boolean | Gizli satır için orijinal satır yüksekliğini mi yoksa 0'ı mı döndürdüğünü belirtir. |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype). Döndürülen yükseklik değerinin birim tipi |

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
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


Satır gizli ise orijinal satır yüksekliğini nokta biriminde alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cells.GetRowHeight(int,bool,CellsUnitType) metodunu kullanın. Bu metod Nisan 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


Bu çalışma sayfasındaki bireysel satırları temsil eden [Row](../../com.aspose.cells/row) nesnelerinin koleksiyonunu alır.

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Bu çalışma sayfasındaki varsayılan satır yüksekliğini nokta biriminde alır.

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


Bu çalışma sayfasındaki varsayılan satır yüksekliğini inç biriminde alır.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Bu çalışma sayfasındaki varsayılan satır yüksekliğini piksel biriminde alır.

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
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Çalışma sayfasının varsayılan stilini alır.

**Returns:**
[Style](../../com.aspose.cells/style)
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
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


Belirtilen bir satırın yüksekliğini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |

**Returns:**
double - Satır yüksekliği.
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


Belirtilen satırın yüksekliğini inç biriminde alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi |

**Returns:**
double - Satır yüksekliği
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

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Satırları gruplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanacak ilk satır indeksi. |
| lastIndex | int | Gruplanacak son satır indeksi. |
| isHidden | boolean | Gruplanan satırların gizli olup olmadığını belirtir. |

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

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


Birden fazla sütunu gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| totalColumns | int | Sütun numarası. |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


Gruplanmış satırları/sütunları daraltır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isVertical | boolean | True, gruplandırılmış satırları daralt. |
| dizin | int | Satır/sütun indeksi |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Bir satırı gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


Birden fazla satırı gizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| totalRows | int | Satır numarası. |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


Bir çalışma sayfasına double dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| doubleArray | double[] | Double dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | boolean | Veriyi dikey ya da yatay olarak içe aktarmayı belirler. |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


Bir çalışma sayfasına iki boyutlu double dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| doubleArray | double[][] | İki boyutlu double dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


Bir çalışma sayfasına integer dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| intArray | int[] | Integer dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | boolean | Veriyi dikey ya da yatay olarak içe aktarmayı belirler. |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


Bir çalışma sayfasına iki boyutlu integer dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| intArray | int[][] | İki boyutlu integer dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Bir çalışma sayfasına string dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringArray | java.lang.String[] | String dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | boolean | Veriyi dikey ya da yatay olarak içe aktarmayı belirler. |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


Bir çalışma sayfasına iki boyutlu string dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringArray | java.lang.String[][] | İki boyutlu string dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


Bir çalışma sayfasına veri arraylist'ini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayList | java.util.ArrayList | Veri arraylist. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | boolean | Veriyi dikey ya da yatay olarak içe aktarmayı belirler. |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


Hücrelere bir CSV dosyası içe aktar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | CSV dosya akışı. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Metin dosyası okuma için yükleme seçenekleri |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Hücrelere bir CSV dosyası içe aktar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | CSV dosya akışı. |
| splitter | java.lang.String | Ayırıcı |
| convertNumericData | boolean | Metin dosyasındaki string'in sayısal veriye dönüştürülüp dönüştürülmediği. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


Hücrelere bir CSV dosyası içe aktar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | CSV dosya adı. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Metin dosyası okuma için yükleme seçenekleri |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


Hücrelere bir CSV dosyası içe aktar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | CSV dosya adı. |
| splitter | java.lang.String | Ayırıcı |
| convertNumericData | boolean | Metin dosyasındaki string'in sayısal veriye dönüştürülüp dönüştürülmediği. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


Özel nesneleri içe aktarır.

**Remarks**

Özel nesneler aynı türde olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| liste | java.util.Collection | Özel nesne |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | İçe aktarma seçenekleri. |

**Returns:**
int - İçeri aktarılan toplam satır sayısı.
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


Özel nesneleri içe aktarır.

**Remarks**

Özel nesneler aynı türde olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| liste | java.util.Collection | Özel nesne |
| propertyNames | java.lang.String[] | Özellik adları. Eğer null ise, nesnenin tüm özelliklerini içeri aktaracağız. |
| isPropertyNameShown | boolean | Özellik adının ilk satıra aktarılıp aktarılmayacağını gösterir. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| rowNumber | int | İçe aktarılacak satır sayısı. |
| insertRows | boolean | Veriye uyması için ekstra satırların eklenip eklenmeyeceğini gösterir. |
| dateFormatString | java.lang.String | Hücreler için tarih biçimi dizesi. |
| convertStringToNumber | boolean | Bu yöntemin dizeyi sayıya dönüştürmeye çalışıp çalışmayacağını gösterir. |

**Returns:**
int - İçeri aktarılan toplam satır sayısı.
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


Özel veri tablosundan verileri içe aktar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | Özel veri tablosu. |
| firstRow | int | İlk satır indeksi. |
| firstColumn | int | İlk sütun indeksi. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | İçe aktarma seçenekleri |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


Bir çalışma sayfasına formül dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringArray | java.lang.String[] | Formül dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | boolean | Veriyi dikey ya da yatay olarak içe aktarmayı belirler. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


Bir çalışma sayfasına veri dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objArray | java.lang.Object[] | Veri dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | boolean | Veriyi dikey ya da yatay olarak içe aktarmayı belirler. |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


Bir çalışma sayfasına veri dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objArray | java.lang.Object[] | Veri dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | boolean | Veriyi dikey ya da yatay olarak içe aktarmayı belirler. |
| atla | int | Atlanan satır veya sütun sayısı. |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | İçe aktarılacak ResultSet nesnesi. |
| rowIndex | int | Çalışma sayfasındaki başlangıç satır indeksi. |
| columnIndex | int | Çalışma sayfasındaki başlangıç sütun indeksi. |
| isFieldNameShown | boolean | Resultset'in alan adının ilk satıra aktarılıp aktarılmayacağını gösterir. |

**Returns:**
int - gerçekte kaç satırın içe aktarıldığı.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | İçe aktarılacak ResultSet nesnesi. |
| rowIndex | int | Çalışma sayfasındaki başlangıç satır indeksi. |
| columnIndex | int | Çalışma sayfasındaki başlangıç sütun indeksi. |
| isFieldNameShown | boolean | Resultset'in alan adının ilk satıra aktarılıp aktarılmayacağını gösterir. |
| customDateFormatString | java.lang.String | Tarih değeri içeren hücreler için tarih biçimi dizesi. |
| convertStringToNumber | boolean | Bu yöntemin dizeyi sayıya dönüştürmeye çalışıp çalışmayacağını gösterir. |

**Returns:**
int - gerçekte kaç satırın içe aktarıldığı.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | İçe aktarılacak ResultSet nesnesi. |
| rowIndex | int | Çalışma sayfasındaki başlangıç satır indeksi. |
| columnIndex | int | Çalışma sayfasındaki başlangıç sütun indeksi. |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | İçe aktarma seçenekleri |

**Returns:**
int - gerçekte kaç satırın içe aktarıldığı.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | İçe aktarılacak ResultSet nesnesi. |
| rowIndex | int | Çalışma sayfasındaki başlangıç satır indeksi. |
| columnIndex | int | Çalışma sayfasındaki başlangıç sütun indeksi. |
| rowNum | int | İçe aktarılacak satır sayısı. -1, verilen resultset'teki tüm kayıtları içe aktarmak için. |
| columnNum | int | İçe aktarılacak sütun sayısı. -1, verilen resultset'teki tüm sütunları içe aktarmak için. |
| isFieldNameShown | boolean | Resultset'in alan adının ilk satıra aktarılıp aktarılmayacağını gösterir. |

**Returns:**
int - gerçekte kaç satırın içe aktarıldığı.
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | İçe aktarılacak ResultSet nesnesi. |
| rowIndex | int | Çalışma sayfasındaki başlangıç satır indeksi. |
| columnIndex | int | Çalışma sayfasındaki başlangıç sütun indeksi. |
| rowNum | int | İçe aktarılacak satır sayısı. -1, verilen resultset'teki tüm kayıtları içe aktarmak için. |
| columnNum | int | İçe aktarılacak sütun sayısı. -1, verilen resultset'teki tüm sütunları içe aktarmak için. |
| isFieldNameShown | boolean | Resultset'in alan adının ilk satıra aktarılıp aktarılmayacağını gösterir. |
| customDateFormatString | java.lang.String | Tarih değeri içeren hücreler için tarih biçimi dizesi. |
| convertStringToNumber | boolean | Bu yöntemin dizeyi sayıya dönüştürmeye çalışıp çalışmayacağını gösterir. |

**Returns:**
int - gerçekte kaç satırın içe aktarıldığı.
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | İçe aktarılacak ResultSet nesnesi. |
| startCell | java.lang.String | Resultset'i eklemek için başlangıç hücresinin adı, örneğin "A1". |
| isFieldNameShown | boolean | Resultset'in alan adının ilk satıra aktarılıp aktarılmayacağını gösterir. |

**Returns:**
int - gerçekte kaç satırın içe aktarıldığı.
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | İçe aktarılacak ResultSet nesnesi. |
| startCell | java.lang.String | Resultset'i eklemek için başlangıç hücresinin adı, örneğin "A1". |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | İçe aktarma seçenekleri |

**Returns:**
int - gerçekte kaç satırın içe aktarıldığı.
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


Bir ResultSet nesnesindeki verileri çalışma sayfasına içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rs | java.sql.ResultSet | İçe aktarılacak ResultSet nesnesi. |
| startCell | java.lang.String | Resultset'i eklemek için başlangıç hücresinin adı, örneğin "A1". |
| rowNum | int | İçe aktarılacak satır sayısı. -1, verilen resultset'teki tüm kayıtları içe aktarmak için. |
| columnNum | int | İçe aktarılacak sütun sayısı. -1, verilen resultset'teki tüm sütunları içe aktarmak için. |
| isFieldNameShown | boolean | Resultset'in alan adının ilk satıra aktarılıp aktarılmayacağını gösterir. |

**Returns:**
int - gerçekte kaç satırın içe aktarıldığı.
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


Bir çalışma sayfasına iki boyutlu veri dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objArray | java.lang.Object[][] | İki boyutlu veri dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Bir çalışma sayfasına iki boyutlu veri dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objArray | java.lang.Object[][] | İki boyutlu veri dizisi. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| convertStringToNumber | boolean | Bu yöntemin dizeyi sayıya dönüştürmeye çalışıp çalışmayacağını gösterir. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


Bir çalışma sayfasına iki boyutlu veri dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objArray | java.lang.Object[][] | İki boyutlu veri dizisi. |
| styles | java.lang.Object[][] | İki boyutlu veri stili. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| convertStringToNumber | boolean | Bu yöntemin dizeyi sayıya dönüştürmeye çalışıp çalışmayacağını gösterir. |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


Bir çalışma sayfasına iki boyutlu veri dizisini içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objArray | java.lang.Object[][] | İki boyutlu veri dizisi. |
| styles | java.lang.Object[][] | İki boyutlu veri stili. |
| firstRow | int | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | int | İçe aktarılacak ilk hücrenin sütun numarası. |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Dize değerlerini dönüştürme seçenekleri |

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

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


Çalışma sayfasına bazı sütunlar ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |
| totalColumns | int | Sütun sayısı. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Ekleme işlemi için seçenekler. |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


Kesilmiş aralığı ekle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | Kesme aralığı. |
| satır | int | Satır. |
| sütun | int | Sütun. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Kesilen aralığı eklerken hedef aralıktaki diğer nesnelerin nasıl kaydırılacağını gösterir. |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Alanı kaydır. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Hücreleri kaydırma seçeneği. |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Alanı kaydır. |
| shiftNumber | int | Eklenecek satır veya sütun sayısı. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Hücreleri kaydırma seçeneği. |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Belirtilen hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | Alanı kaydır. |
| shiftNumber | int | Eklenecek satır veya sütun sayısı. |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype). Hücreleri kaydırma seçeneği. |
| updateReference | boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

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

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


Çalışma sayfasına birden fazla satır ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |
| totalRows | int | Eklenecek satır sayısı. |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | Ekleme işlemi için seçenekler. |

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


Satır yüksekliğinin ve varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


Satırın varsayılan olarak gizli olup olmadığını gösterir.

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


Aralığın silinebilir olup olmadığını kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Aralığın başlangıç satır indeksi. |
| startColumn | int | Aralığın başlangıç sütun indeksi. |
| totalRows | int | Aralıktaki satır sayısı. |
| totalColumns | int | Aralıktaki sütun sayısı. |

**Returns:**
boolean -
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


Hücre enumeratörünü alır.

**Remarks**

Dönen Enumerator ile öğeler dolaşılırken, hücreler koleksiyonu değiştirilmemelidir (örneğin yeni Cell/Row oluşturulmasına veya mevcut Cell/Row silinmesine neden olacak işlemler). Aksi takdirde enumerator tüm hücreleri doğru şekilde dolaşamayabilir (bazı öğeler tekrar tekrar dolaşılabilir veya atlanabilir).

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
java.util.Iterator - Hücre enumeratörü
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


Bir XML haritasına bağlantı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mapName | java.lang.String | xml haritasının adı |
| satır | int | hedef hücrenin satırı |
| sütun | int | hedef hücrenin sütunu |
| yol | java.lang.String | xml haritadaki xml öğesinin yolu |

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

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


Belirtilen hücre aralığını tek bir hücrede birleştirir.

**Remarks**

Birleştirilmiş hücreye, aralıktaki sol üst hücrenin adresi üzerinden başvurun. mergeConflict true ise ve birleştirilmiş aralık diğer birleştirilmiş hücrelerle çakışıyorsa, diğer birleştirilmiş hücreler otomatik olarak kaldırılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | int | Bu aralığın ilk sütunu (sıfır tabanlı) |
| totalRows | int | Satır sayısı (bir tabanlı) |
| totalColumns | int | Sütun sayısı (bir tabanlı) |
| mergeConflict | boolean | Birleştirme çakışması birleştirilmiş aralıklar. |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


Belirtilen hücre aralığını tek bir hücrede birleştirir.

**Remarks**

Birleştirilmiş hücreye, aralıktaki sol üst hücrenin adresi üzerinden başvurun. mergeConflict true ise ve birleştirilmiş aralık diğer birleştirilmiş hücrelerle çakışıyorsa, diğer birleştirilmiş hücreler otomatik olarak kaldırılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | int | Bu aralığın ilk sütunu (sıfır tabanlı) |
| totalRows | int | Satır sayısı (bir tabanlı) |
| totalColumns | int | Sütun sayısı (bir tabanlı) |
| checkConflict | boolean | Birleştirilmiş hücrelerin diğer birleştirilmiş hücrelerle kesişip kesişmediğini gösterir. |
| mergeConflict | boolean | Birleştirme çakışması birleştirilmiş aralıklar. |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


Aralığı taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | Taşınması gereken aralık. |
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




### removeDuplicates() {#removeDuplicates--}
```
public void removeDuplicates()
```


Sayfadaki yinelenen satırları kaldırır.

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Aralıktaki yinelenen değerleri kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satırı. |
| startColumn | int | Başlangıç sütunu |
| endRow | int | Bitiş satır indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


Aralığın yinelenen verilerini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satırı. |
| startColumn | int | Başlangıç sütunu |
| endRow | int | Bitiş satır indeksi. |
| endColumn | int | Bitiş sütun indeksi. |
| hasHeaders | boolean | Aralığın başlık içerip içermediğini gösterir. |
| columnOffsets | int[] | Sütun ofsetleri. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Tüm formülleri kaldırır ve formül değerleriyle değiştirir.

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


Aralığın ara toplam ayarlarını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Aralık |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Normal görünümde belirtilen sütunun genişliğini ayarlar.

**Remarks**

Elektronik tablo için, sütun genişliği, normal stilin yazı tipinde 0~9 sayılarının en geniş rakamının karakter sayısı olarak ölçülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| genişlik | double | Sütun genişliği karakter birimiyle. Sütun genişliği 0 ile 255 arasında olmalıdır. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Normal görünümde sütun genişliğini inç biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| inç | double | İnç sayısı. |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


Normal görünümde sütun genişliğini piksel biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| piksel | int | Piksel sayısı. |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


Satır yüksekliğinin ve varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


Satırın varsayılan olarak gizli olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Bu hücreler için bellek kullanımı seçeneğini ayarlar.

Bakınız [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Bazı modlar için dikkate değer sınırlamalar ve önerilen işlemler:

| Mod | Açıklamalar | Desteklenen |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | Bu mod bir çalışma kitabındaki herhangi bir çalışma sayfası için kullanıldığında, geçici dosyalar gibi tüm kaynakları serbest bırakmak için işin sonunda [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) çağrılmalıdır. |
 
Hücrelere rastgele erişmek, verinin rastgele ve tekrar tekrar okunup güncellenmesi gerektiği için düşük performans verir (dosyadaki işaretçi buna göre değişir ve I/O işlemleri tekrar tekrar gerekir). Mümkünse, veriye her zaman sıralı olarak (satır satır) erişin.
 
Bir satır/hücrenin verisi değiştirildiğinde, diğer hücrelerin/satırların verileri de etkilenebilir (örneğin veri, değişen veri için yeterli alan ayırmak amacıyla başka yerlere kaydırılabilir/taşınabilir). Bu nedenle, her veri değişikliği, diğer mevcut nesnelerin (örneğin Satır veya Hücre nesnesi) senkronizasyonunu gerektirir. Daha iyi performans için, lütfen aynı anda birden fazla Satır/Hücre tutmayın. Onları tek tek işlemek, veri senkronizasyonunu azaltır ve performans biraz artar. | v25.7     |

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


Hücre veri modelinin Çoklu İş Parçacığı okumasını destekleyip desteklemeyeceğini ayarlar. Bu özelliğin varsayılan değeri false'dur.

**Remarks**

Eğer bu koleksiyondaki Row/Cell nesnelerini aynı anda birden fazla iş parçacığı okuyorsa, bu özellik true olarak ayarlanmalıdır, aksi takdirde beklenmeyen sonuçlar ortaya çıkabilir. Çok İşlemli (Multi-Thread) okuma desteği, bu koleksiyondan Row/Cell nesnelerine erişim performansını düşürebilir. Lütfen bazı özelliklerin Çok İşlemli okuma desteklemediğini unutmayın, örneğin değer biçimlendirme ([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--), [Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), vb.). Bu nedenle, bu özellik true olarak ayarlanmış olsa bile, bu API'ler Çok İşlemli okuma için hâlâ beklenmeyen sonuçlar verebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


Tüm çalışma sayfası değerlerinin dize olarak korunup korunmayacağını gösteren bir değeri ayarlar. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Belirtilen satırın yüksekliğini ayarlar.

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

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Bu çalışma sayfasındaki varsayılan satır yüksekliğini nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


Bu çalışma sayfasındaki varsayılan satır yüksekliğini inç biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Bu çalışma sayfasındaki varsayılan satır yüksekliğini piksel biriminde ayarlar.

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

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Çalışma sayfasının varsayılan stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


Sütunun genişliğini farklı görünümde ayarlar.

**Remarks**

Mevcut görünüm türü [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW) ise, sütunun genişliği yazdırılan genişlikle aynıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| piksel | int | Genişlik piksel biriminde. |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


Gruplanmış satırları/sütunları genişletir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isVertical | boolean | Doğru, gruplanmış satırları genişletir. |
| dizin | int | Satır/sütun indeksi |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


Aralık için alt toplamlar oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Aralık |
| groupBy | int | Gruplamak için alan, sıfır tabanlı bir tam sayı offseti olarak |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Alt toplam işlevi. |
| totalList | int[] | Alt toplamların ekleneceği alanları gösteren, sıfır tabanlı alan offsetlerinden oluşan bir dizi. |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


Aralık için alt toplamlar oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Aralık |
| groupBy | int | Gruplamak için alan, sıfır tabanlı bir tam sayı offseti olarak |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Alt toplam işlevi. |
| totalList | int[] | Alt toplamların ekleneceği alanları gösteren, sıfır tabanlı alan offsetlerinden oluşan bir dizi. |
| replace | boolean | Mevcut alt toplamların değiştirilip değiştirilmeyeceğini gösterir |
| pageBreaks | boolean | Gruplar arasında sayfa sonu eklenip eklenmeyeceğini gösterir |
| summaryBelowData | boolean | Verinin altında özet eklenip eklenmeyeceğini gösterir. |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


Belirtilen sütundaki içeriği birden çok sütuna böler..

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |
| totalRows | int | Satır sayısı. |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | Bölme seçenekleri. |

**Returns:**
int - Bölünmüş değerlerin toplam sütun sayısı.
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

Yalnızca dış grup bilgisini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanması kaldırılacak ilk satır indeksi. |
| lastIndex | int | Gruplanması kaldırılacak son satır indeksi. |

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


Satırların gruplamasını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanması kaldırılacak ilk satır indeksi. |
| lastIndex | int | Gruplanması kaldırılacak son satır indeksi. |
| isAll | boolean | Doğru, tüm grup bilgisini kaldırır. Aksi takdirde, dış grup bilgisini kaldırır. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Bir sütunun gizliliğini kaldırır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| genişlik | double | Sütun genişliği. |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


Birden çok sütunun gizliliğini kaldırır.

**Remarks**

Sütun genişliğini yalnızca gizli sütunlara uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| totalColumns | int | Sütun numarası |
| genişlik | double | Sütun genişliği. |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


Bir satırın gizliliğini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| yükseklik | double | Satır yüksekliği. Satırın yüksekliği yalnızca satır gizli olduğunda ve verilen yükseklik değeri pozitif olduğunda değiştirilecektir. |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


Gizli satırların gizliliğini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| totalRows | int | Satır numarası. |
| yükseklik | double | Satır yüksekliği. Satırın yüksekliği yalnızca satır gizli olduğunda ve verilen yükseklik değeri pozitif olduğunda değiştirilecektir. |

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

