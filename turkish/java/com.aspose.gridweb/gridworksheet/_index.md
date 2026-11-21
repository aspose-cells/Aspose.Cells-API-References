---
title: "GridWorksheet"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tek bir çalışma sayfasını temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

Tek bir çalışma sayfasını temsil eden nesneyi kapsüller.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | Belirtilen AutoFilter'ın uygulandığı aralığı ayarlar. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | Belirtilen satır için özel filtre ekle. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Sütun genişliğini otomatik olarak ayarlar. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Sütun genişliğini otomatik olarak ayarlar. |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Satır yüksekliğini otomatik olarak ayarlar. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Satır yüksekliğini otomatik olarak ayarlar. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Dikdörtgen bir aralıktaki satır yüksekliğini otomatik olarak ayarlar. |
| [autoFitRows()](#autoFitRows--) | Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Bir formülü hesaplar. |
| [clearComments()](#clearComments--) | Tasarımcı elektronik tablosundaki tüm yorumları temizler. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | Başka bir çalışma sayfasından içerikleri ve biçimleri kopyalar. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | Sayfada ara toplam oluşturur. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Sayfada ara toplam oluşturur. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | Kolon için filtreyi ayarlar. filterString'i çağırmadan önce AddAutoFilter'i çağırmamız gerekir. Filtre kriteri dizesi. Virgül -> "," karakterini ayırıcı olarak kullandığımızı unutmayın, bu yüzden filtrelemek istediğiniz hücre değeri virgül içermemelidir. filterString(10,"123,456") ifadesi, 10. sütunun 123 veya 456 içermesi anlamına gelir, filterString(10,"123") ifadesi, 10. sütunun 123 içermesi anlamına gelir. Sütun indeksi değeri virgülle ayrılır, örn. 123,456,789 veya abc |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur. |
| [getActiveCell()](#getActiveCell--) | Çalışma sayfasındaki etkin hücreyi alır. |
| [getBackgroundImage()](#getBackgroundImage--) | Çalışma sayfasının arka plan resmini alır. |
| [getCells()](#getCells--) | [GridCell](../../com.aspose.gridweb/gridcell) koleksiyonunu alır. |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Çalışma sayfasının kod adını temsil eder. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | Sütun başlığını alır. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | Sütun başlığının araç ipucu metnini alır. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | Bir sütunun yalnızca okunur olup olmadığını alır. |
| [getComments()](#getComments--) | [GridComment](../../com.aspose.gridweb/gridcomment) koleksiyonunu alır. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. |
| [getDisplayZeros()](#getDisplayZeros--) | Sıfır değerler gösteriliyorsa doğru. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | İlk görünen sütun indeksini temsil eder. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | İlk görünen satır indeksini temsil eder. |
| [getFreezedPanes()](#getFreezedPanes--) | Dondurulmuş bölmeleri alır. |
| [getGridActiveCell()](#getGridActiveCell--) | Çalışma sayfasındaki etkin hücreyi alır. |
| [getHyperlinks()](#getHyperlinks--) | [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection) koleksiyonunu alır. |
| [getIndex()](#getIndex--) | Çalışma sayfası koleksiyonundaki sayfanın indeksini alır. |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | Hücrenin yalnızca okunur olup olmadığını alır. Bu, GridWeb'in genişletilmiş bir özelliğidir, gerçek Excel dosyasında tutulmaz. |
| [getName()](#getName--) | Çalışma sayfasının adını alır. |
| [getOutlineShown()](#getOutlineShown--) | Anahat gösterilip gösterilmeyeceğini belirtir. |
| [getPictures()](#getPictures--) | [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) koleksiyonunu alır. |
| [getPivotTables()](#getPivotTables--) | Çalışma sayfasındaki pivot tabloları alır. |
| [getRowCaption(int row)](#getRowCaption-int-) | Satır başlığını alır. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | Satır başlığının araç ipucu metnini alır. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | Bir satırın yalnızca okunur olup olmadığını alır. |
| [getSelected()](#getSelected--) | Bu çalışma sayfasının, çalışma kitabı açıldığında seçili olup olmadığını belirtir. |
| [getShapes()](#getShapes--) | [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) koleksiyonunu alır. |
| [getStandardHeight()](#getStandardHeight--) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini, puan biriminde alır. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini, piksel biriminde alır. |
| [getTabColor()](#getTabColor--) | Çalışma sayfası sekme rengini temsil eder. |
| [getUniqueID()](#getUniqueID--) | Denetimde UniqueID'yi alır |
| [getValidations()](#getValidations--) | Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır. |
| [getVisible()](#getVisible--) | Bu sayfanın adının denetimin sayfa sekmelerinde gösterilip gösterilmediğini belirtir. |
| [getWorkbook()](#getWorkbook--) | Çalışma sayfası koleksiyonunun [GridWorkbook](../../com.aspose.gridweb/gridworkbook) nesnesini alır. |
| [getZoom()](#getZoom--) | Yüzde olarak ölçekleme faktörünü temsil eder. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Satırları gruplar. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Izgara çizgilerinin görünür olup olmadığını gösteren bir değeri alır. Varsayılan true'dur. |
| [isProtected()](#isProtected--) | Çalışma sayfasının korumalı olup olmadığını belirtir. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | Özet satırının anahatta detay satırlarının altında konumlandırılıp konumlandırılmayacağını gösterir. |
| [moveTo(int index)](#moveTo-int-) | Sayfayı elektronik tabloda başka bir konuma taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | Satırları gizlemek veya göstermek için otomatik filtreleri yenile. |
| [removeAutoFilter()](#removeAutoFilter--) | Çalışma sayfasının otomatik filtresini kaldır. |
| [removeSubtotal()](#removeSubtotal--) | Sayfadaki CreateSubtotal yöntemiyle oluşturulan alt toplamı kaldırır. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | Uygulamak istediğiniz alanın tam sayı ofseti, ilk filtre sütununa (listeden sola; en soldaki alan alan 0) dayanır. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Çalışma sayfasındaki etkin hücreyi ayarlar. |
| [setAllCellsEditable()](#setAllCellsEditable--) | Tüm hücreleri düzenlenebilir yapar. bu bir genişletilmiş özelliktir |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Tüm hücreleri salt okunur yapar. bu bir genişletilmiş özelliktir; bu özelliğin gerçek hücrede tutulamayacağını unutmayın, korumayı sürdürmek istiyorsanız lütfen setProtect kullanın |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Çalışma sayfasının arka plan resmini ayarlar. |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | Sütun için başlığı ayarlar. lütfen bunun bir uzantı özelliği olduğunu ve Excel dosyasında tutulamayacağını unutmayın |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | Sütun başlığının araç ipucu metnini ayarlar. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | Bir sütunu salt okunur olarak ayarlar, böylece kullanıcı istemci tarafından silemez. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Sıfır değerler gösteriliyorsa doğru. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Bir hücre aralığını düzenlenebilir yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells SetAllCellsReadonly yöntemini çağırarak tüm hücreleri salt okunur yapın. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | İlk görünen sütun indeksini temsil eder. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | İlk görünen satır indeksini temsil eder. |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | Çalışma sayfasındaki etkin hücreyi ayarlar. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Izgara çizgilerinin görünür olup olmadığını gösteren bir değeri ayarlar. Varsayılan true'dur. |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | Hücrenin salt okunur olup olmadığını ayarlar. bu GridWeb'in genişletilmiş bir özelliğidir, gerçek Excel dosyasında tutulmayacaktır |
| [setName(String value)](#setName-java.lang.String-) | Çalışma sayfasının adını ayarlar. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Anahat gösterilip gösterilmeyeceğini belirtir. |
| [setProtect()](#setProtect--) | Çalışma sayfasını korur. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Bir hücre aralığını salt okunur yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Önce SetAllCellsEditable yöntemini çağırarak tüm hücreleri düzenlenebilir yapın. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | Satır için başlığı ayarlar. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | Satır başlığının araç ipucu metnini ayarlar. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | Bir satırı salt okunur olarak ayarlar, böylece kullanıcı istemci tarafından silemez. |
| [setSelected(boolean value)](#setSelected-boolean-) | Bu çalışma sayfasının, çalışma kitabı açıldığında seçili olup olmadığını belirtir. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Bu çalışma sayfasında varsayılan satır yüksekliğini puan biriminde ayarlar. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Bu çalışma sayfasında varsayılan satır yüksekliğini piksel biriminde ayarlar. |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | Özet satırının anahatta detay satırlarının altında konumlandırılıp konumlandırılmayacağını gösterir. |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | Çalışma sayfası sekme rengini temsil eder. |
| [setVisible(boolean value)](#setVisible-boolean-) | Bu sayfanın adının denetimin sayfa sekmelerinde gösterilip gösterilmediğini belirtir. |
| [setZoom(int value)](#setZoom-int-) | Yüzde olarak ölçekleme faktörünü temsil eder. |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | Çalışma sayfasındaki bölmeleri dondurmayı kaldırır. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | Satırların gruplamasını kaldırır. |
| [unProtect()](#unProtect--) | Çalışma sayfasının korumasını kaldırır. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


Belirtilen AutoFilter'ın uygulandığı aralığı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endColumn | int | Son sütun indeksi. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


Belirtilen satır için özel filtre ekle.

**Remarks**

Filtre kriterleri dizesi. not: ayırıcı karakter olarak , ve ; kullanıyoruz, bu yüzden hücre değeri bu ayırıcı karakterleri içermemelidir. aşağıda kriter dizesi örnekleri bulunmaktadır //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int |  |
| critira | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Sütun genişliğini otomatik olarak ayarlar.

**Remarks**

AutoFitColumn, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Sütun genişliğini otomatik olarak ayarlar.

**Remarks**

Bu yöntem, satır içindeki hücre aralığındaki içeriğe göre satırı otomatik olarak sığdırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |
| firstRow | int | İlk satır indeksi. |
| lastRow | int | Son satır indeksi. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Satır yüksekliğini otomatik olarak ayarlar.

**Remarks**

AutoFitRow, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Satır yüksekliğini otomatik olarak ayarlar.

**Remarks**

Bu yöntem, satır içindeki hücre aralığındaki içeriğe göre satırı otomatik olarak sığdırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |
| firstColumn | int | İlk sütun indeksi. |
| lastColumn | int | Son sütun indeksi. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Dikdörtgen bir aralıktaki satır yüksekliğini otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| endRow | int | Bitiş satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| onlyAuto | boolean | Doğru, yalnızca satır yüksekliği özelleştirilmediğinde satır yüksekliğini otomatik olarak sığdırır. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| endRow | int | Bitiş satır indeksi. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Bir formülü hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object - 
### clearComments() {#clearComments--}
```
public void clearComments()
```


Tasarımcı elektronik tablosundaki tüm yorumları temizler.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


Başka bir çalışma sayfasından içerikleri ve biçimleri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Kaynak çalışma sayfası. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


Sayfada ara toplam oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnNameRowIndex | int | Sütun adı satırının satır indeksi. |
| dataRows | int | Veri satırlarının sayısı. |
| groupByColumnIndex | int | Gruplanacak sütunun sütun indeksi. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Ara toplam işlevi türü. |
| subtotalColumnIndexList | int[] | Ara toplam yapılacak sütun indeksleri. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Sayfada ara toplam oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnNameRowIndex | int | Sütun adı satırının satır indeksi. |
| dataRows | int | Veri satırlarının sayısı. |
| groupByColumnIndex | int | Gruplanacak sütunun sütun indeksi. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Ara toplam işlevi türü. |
| subtotalColumnIndexList | int[] | Ara toplam yapılacak sütun indeksleri. |
| functionLabel | java.lang.String | Ara toplam işlevinin etiketi. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Genel toplam satırının stili. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Ara toplam satırının stili. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Ara toplam sonuç hücrelerinin sayı türü. |
| customString | java.lang.String | Ara toplam sonuç hücrelerinin özel biçim dizesi. Null olabilir. |

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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


Kolon için filtreyi ayarlar. filterString'i çağırmadan önce AddAutoFilter'i çağırmamız gerekir. Filtre kriteri dizesi. Virgül -> "," karakterini ayırıcı olarak kullandığımızı unutmayın, bu yüzden filtrelemek istediğiniz hücre değeri virgül içermemelidir. filterString(10,"123,456") ifadesi, 10. sütunun 123 veya 456 içermesi anlamına gelir, filterString(10,"123") ifadesi, 10. sütunun 123 içermesi anlamına gelir. Sütun indeksi değeri virgülle ayrılır, örn. 123,456,789 veya abc

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int |  |
| kriter | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur.

**Remarks**

Satır indeksi ve sütun indeksi aynı anda sıfır olamaz. Satır sayısı ve sütun sayısı da aynı anda sıfır olamaz.

İlk iki parametre dondurulmuş konumu belirtir ve son iki parametre sol üst bölmede dondurulmuş alanı belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |
| freezedRows | int | Üst bölmede görünen satır sayısı, satır indeksinden fazla olamaz. |
| freezedColumns | int | Sol bölmede görünen sütun sayısı, sütun indeksinden fazla olamaz. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur.

**Remarks**

Satır indeksi ve sütun indeksi aynı anda sıfır olamaz. Satır sayısı ve sütun sayısı da aynı anda sıfır olamaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |
| freezedRows | int | Üst bölmede görünen satır sayısı, satır indeksinden fazla olamaz. |
| freezedColumns | int | Sol bölmede görünen sütun sayısı, sütun indeksinden fazla olamaz. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Çalışma sayfasındaki etkin hücreyi alır.

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Çalışma sayfasının arka plan resmini alır.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


[GridCell](../../com.aspose.gridweb/gridcell) koleksiyonunu alır.

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Çalışma sayfasının kod adını temsil eder.

**Remarks**

Şablon dosyası VBA/makro içeriyorken kod adını değiştiremezsiniz.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


Sütun başlığını alır. Başlık ayarlanmamışsa boş string döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Sütun başlığı. Başlık ayarlanmamışsa boş string döndürür.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


Sütun başlığının araç ipucu metnini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| colIndex | int | Sütunun indeksi. |

**Returns:**
java.lang.String - Araç ipucu metni.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


Bir sütunun yalnızca okunur olup olmadığını alır. Bu, GridWeb'e özgü genişletilmiş bir yöntemdir, gerçek Excel dosyasında tutulmaz ve etkili olmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | sütun indeksi. |

**Returns:**
boolean - Yalnızca okunur ise true döner.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


[GridComment](../../com.aspose.gridweb/gridcomment) koleksiyonunu alır.

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Sıfır değerler gösteriliyorsa doğru.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


İlk görünen sütun indeksini temsil eder.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


İlk görünen satır indeksini temsil eder.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Dondurulmuş bölmeleri alır.

**Returns:**
int[] - null döndürmek, çalışma sayfasının dondurulmadığını gösterir 0:Satır indeksi;1:sütun;2:dondurulmuşSatırlar;3:dondurulmuşSatırlar
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


Çalışma sayfasındaki etkin hücreyi alır.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection) koleksiyonunu alır.

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Çalışma sayfası koleksiyonundaki sayfanın indeksini alır.

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


Hücrenin yalnızca okunur olup olmadığını alır. Bu, GridWeb'in genişletilmiş bir özelliğidir, gerçek Excel dosyasında tutulmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int |  |
| col | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Çalışma sayfasının adını alır.

**Remarks**

Çalışma sayfası adının maksimum uzunluğu 31'dir. Aynı adı (büyük/küçük harf duyarsız) iki çalışma sayfasına atayamazsınız. Örneğin, \"SheetName1\" değerini ilk çalışma sayfasına, \"SHEETNAME1\" değerini ikinci çalışma sayfasına atayamazsınız.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


Anahat gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


[getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) koleksiyonunu alır.

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


Çalışma sayfasındaki pivot tabloları alır.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


Satır başlığını alır. Başlık ayarlanmamışsa boş string döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |

**Returns:**
java.lang.String - Satır başlığı. Başlık ayarlanmamışsa boş string döndürür.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


Satır başlığının araç ipucu metnini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satırın indeksi. |

**Returns:**
java.lang.String - Araç ipucu metni.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


Bir satırın readonly olup olmadığını alır. bu, özellikle GridWeb'in genişletilmiş yöntemidir, gerçek excel dosyasında saklanmaz ve etkili olmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | satır indeksi. |

**Returns:**
boolean - Yalnızca okunur ise true döner.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Bu çalışma sayfasının, çalışma kitabı açıldığında seçili olup olmadığını belirtir.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


[getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) koleksiyonunu alır.

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
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
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Çalışma sayfası sekme rengini temsil eder.

**Remarks**

Bu özellik yalnızca ExcelXP (Excel2002) ve sonraki sürümlerde desteklenir. Dosyayı Excel97 veya Excel2000 formatında kaydederseniz, atlanır.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Denetimde UniqueID'yi alır

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Bu sayfanın adının denetimin sayfa sekmelerinde gösterilip gösterilmediğini belirtir.

**Returns:**
boolean
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Çalışma sayfası koleksiyonunun [GridWorkbook](../../com.aspose.gridweb/gridworkbook) nesnesini alır.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Yüzde olarak ölçekleme faktörünü temsil eder. 10 ile 400 arasında olmalıdır.

**Returns:**
int
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
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Izgara çizgilerinin görünür olup olmadığını gösteren bir değeri alır. Varsayılan true'dur.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Çalışma sayfasının korumalı olup olmadığını belirtir.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


Özet satırının anahatta detay satırlarının altında konumlandırılıp konumlandırılmayacağını gösterir.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Sayfayı elektronik tabloda başka bir konuma taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Hedef sayfa indeksi. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


Satırları gizlemek veya göstermek için otomatik filtreleri yenile.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Çalışma sayfasının otomatik filtresini kaldır.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


Sayfadaki CreateSubtotal yöntemiyle oluşturulan alt toplamı kaldırır.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


Uygulamak istediğiniz alanın tam sayı ofseti, ilk filtre sütununa (listeden sola; en soldaki alan alan 0) dayanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Çalışma sayfasındaki etkin hücreyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Tüm hücreleri düzenlenebilir yapar. bu bir genişletilmiş özelliktir

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Tüm hücreleri salt okunur yapar. bu bir genişletilmiş özelliktir; bu özelliğin gerçek hücrede tutulamayacağını unutmayın, korumayı sürdürmek istiyorsanız lütfen setProtect kullanın

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Çalışma sayfasının arka plan resmini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


Sütun için başlığı ayarlar. lütfen bunun bir uzantı özelliği olduğunu ve Excel dosyasında tutulamayacağını unutmayın

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |
| başlık | java.lang.String | Sütun başlığı. Başlığı iptal etmek istiyorsanız null veya boş bir dize gönderin. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


Sütun başlığının araç ipucu metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| colIndex | int | Sütunun indeksi. |
| toolTip | java.lang.String | Araç ipucu metni. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


Bir sütunu readonly olarak ayarlar, böylece kullanıcı istemci tarafından silemez. bu, özellikle GridWeb'in genişletilmiş yöntemidir, gerçek excel dosyasında saklanmaz ve etkili olmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | sütun indeksi. |
| isReadonly | boolean | doğru veya yanlış. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Sıfır değerler gösteriliyorsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Bir hücre aralığını düzenlenebilir yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Tüm hücreleri SetAllCellsReadonly metodunu çağırarak yalnızca okunur yapın. ardından bu yöntemi, düzenlenebilir olacak hücre aralığını belirtmek için çağırın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Aralığın başlangıç satırı. |
| startColumn | int | Aralığın başlangıç sütunu. |
| satırlar | int | Satır sayısı. |
| sütunlar | int | Sütun sayısı. |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


İlk görünen sütun indeksini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


İlk görünen satır indeksini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


Çalışma sayfasındaki etkin hücreyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Izgara çizgilerinin görünür olup olmadığını gösteren bir değeri ayarlar. Varsayılan true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


Hücrenin salt okunur olup olmadığını ayarlar. bu GridWeb'in genişletilmiş bir özelliğidir, gerçek Excel dosyasında tutulmayacaktır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int |  |
| col | int |  |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Çalışma sayfasının adını ayarlar.

**Remarks**

Çalışma sayfası adının maksimum uzunluğu 31'dir. Aynı adı (büyük/küçük harf duyarsız) iki çalışma sayfasına atayamazsınız. Örneğin, \"SheetName1\" değerini ilk çalışma sayfasına, \"SHEETNAME1\" değerini ikinci çalışma sayfasına atayamazsınız.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Anahat gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


Çalışma sayfasını korur.

**Remarks**

Bu yöntem, çalışma sayfasını şifre olmadan korur. Excel dosyasının tüm sürümlerinde çalışma sayfasını koruyabilir.

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Bir hücre aralığını readonly yapar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells İlk olarak tüm hücreleri SetAllCellsEditable metodunu çağırarak düzenlenebilir yapın. ardından bu yöntemi, readonly olacak hücre aralığını belirtmek için çağırın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Aralığın başlangıç satırı. |
| startColumn | int | Aralığın başlangıç sütunu. |
| satırlar | int | Satır sayısı. |
| sütunlar | int | Sütun sayısı. |

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


Satır için başlığı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| başlık | java.lang.String | Satır başlığı. Başlığı iptal etmek istiyorsanız null veya boş bir dize gönderin. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


Satır başlığının araç ipucu metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satırın indeksi. |
| toolTip | java.lang.String | Araç ipucu metni. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


Bir satırı readonly olarak ayarlar, böylece kullanıcı istemci tarafından silemez. bu, özellikle GridWeb'in genişletilmiş yöntemidir, gerçek excel dosyasında saklanmaz ve etkili olmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | satır indeksi. |
| isReadonly | boolean | doğru veya yanlış. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Bu çalışma sayfasının, çalışma kitabı açıldığında seçili olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


Özet satırının anahatta detay satırlarının altında konumlandırılıp konumlandırılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


Çalışma sayfası sekme rengini temsil eder.

**Remarks**

Bu özellik yalnızca ExcelXP (Excel2002) ve sonraki sürümlerde desteklenir. Dosyayı Excel97 veya Excel2000 formatında kaydederseniz, atlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Bu sayfanın adının denetimin sayfa sekmelerinde gösterilip gösterilmediğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Yüzde olarak ölçekleme faktörünü temsil eder. 10 ile 400 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Çalışma sayfasındaki bölmeleri dondurmayı kaldırır.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


Satırların gruplamasını kaldırır.

**Remarks**

Yalnızca dış grup bilgilerini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | int | Gruplanması kaldırılacak ilk satır indeksi. |
| lastIndex | int | Gruplanması kaldırılacak son satır indeksi. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


Çalışma sayfasının korumasını kaldırır.

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

