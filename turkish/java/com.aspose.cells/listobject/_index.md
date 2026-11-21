---
title: "ListObject"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma sayfasındaki tabloyu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Bir çalışma sayfasındaki tabloyu temsil eder.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | Tablo stilini aralığa uygula. |
| [convertToRange()](#convertToRange--) | Tabloyu aralığa dönüştür. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | Tabloyu aralığa dönüştür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | Tabloyu filtrele. |
| [getAlternativeDescription()](#getAlternativeDescription--) | Alternatif açıklamayı alır. |
| [getAlternativeText()](#getAlternativeText--) | Alternatif metni alır. |
| [getAutoFilter()](#getAutoFilter--) | Bu tablonun otomatik filtresini alır. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Tablonun yorumunu alır. |
| [getDataRange()](#getDataRange--) | Tablonun veri aralığını alır. |
| [getDataSourceType()](#getDataSourceType--) | Tablonun veri kaynağı türünü alır. |
| [getDisplayName()](#getDisplayName--) | Tablonun görüntüleme adını alır. |
| [getEndColumn()](#getEndColumn--) | Aralığın son sütununu alır. |
| [getEndRow()](#getEndRow--) | Aralığın son satırını alır. |
| [getListColumns()](#getListColumns--) | Bu tablonun [ListColumn](../../com.aspose.cells/listcolumn) listesini alır. |
| [getQueryTable()](#getQueryTable--) | Bağlantılı QueryTable'ı alır. |
| [getShowHeaderRow()](#getShowHeaderRow--) | Bu Tablonun başlık satırını gösterip göstermediğini alır. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Tablodaki ilk sütunun uygulanan stil olup olmadığını gösterir. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Tablodaki son sütunun uygulanan stil olup olmadığını gösterir. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [getShowTotals()](#getShowTotals--) | Bu Tablonun toplam satırını gösterip göstermediğini alır. |
| [getStartColumn()](#getStartColumn--) | Aralığın başlangıç sütununu alır. |
| [getStartRow()](#getStartRow--) | Aralığın başlangıç satırını alır. |
| [getTableStyleName()](#getTableStyleName--) | Tablo stil adını alır. |
| [getTableStyleType()](#getTableStyleType--) | Yerleşik tablo stilini alır. |
| [getXmlMap()](#getXmlMap--) | Bu liste için kullanılan bir [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) alır. |
| [hasAutoFilter()](#hasAutoFilter--) | Bu tabloya otomatik filtre uygulanıp uygulanmadığını gösterir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | Formülü tablodaki hücreye koyar. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | Formülü tablodaki hücreye koyar. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Değeri hücreye koyar. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | Değeri hücreye koyar. |
| [removeAutoFilter()](#removeAutoFilter--) | Bu tabloya uygulanan otomatik filtreyi kaldırır. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Liste nesnesinin aralığını yeniden boyutlandırır. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | Alternatif açıklamayı ayarlar. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Alternatif metni ayarlar. |
| [setComment(String value)](#setComment-java.lang.String-) | Tablonun yorumunu ayarlar. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Tablonun görüntülenen adını ayarlar. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | Bu tabloya otomatik filtre uygulanıp uygulanmadığını gösterir. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | Bu Tablonun başlık satırını gösterip göstermeyeceğini ayarlar. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | Tablodaki ilk sütunun uygulanan stil olup olmadığını gösterir. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | Tablodaki son sütunun uygulanan stil olup olmadığını gösterir. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | Bu TAble'in toplam satırını gösterip göstermeyeceğini ayarlar. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | Tablo stil adını ayarlar. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | Yerleşik tablo stilini alır. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Tüm liste sütunlarının adını tablodaki hücrelere günceller. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


Tablo stilini aralığa uygula.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


Tabloyu aralığa dönüştür.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


Tabloyu aralığa dönüştür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | Tabloyu aralığa dönüştürürken seçenekler. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


Tabloyu filtrele.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, lütfen ListObject.HasAutoFilter özelliğini ayarlayın./// Bu özellik, Ekim 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


Alternatif açıklamayı alır.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Alternatif metni alır.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Bu tablonun otomatik filtresini alır.

**Remarks**

Yalnızca [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) false olduğunda çalışır.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


Tablonun yorumunu alır.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Tablonun veri aralığını alır.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Tablonun veri kaynağı türünü alır.

Bakınız [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Tablonun görüntüleme adını alır.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Aralığın son sütununu alır.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Aralığın son satırını alır.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


Bu tablonun [ListColumn](../../com.aspose.cells/listcolumn) listesini alır.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


Bağlantılı QueryTable'ı alır.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


Bu Tablonun başlık satırını gösterip göstermediğini alır.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Tablodaki ilk sütunun uygulanan stil olup olmadığını gösterir.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Tablodaki son sütunun uygulanan stil olup olmadığını gösterir.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


Bu Tablonun toplam satırını gösterip göstermediğini alır.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Aralığın başlangıç sütununu alır.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Aralığın başlangıç satırını alır.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


Tablo stil adını alır.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Yerleşik tablo stilini alır.

Bakınız [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


Bu liste için kullanılan bir [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) alır.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


Bu tabloya otomatik filtre uygulanıp uygulanmadığını gösterir.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


Formülü tablodaki hücreye koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Tablodaki satır ofseti. |
| columnOffset | int | Tablodaki sütun ofseti. |
| formula | java.lang.String | Hücrenin formülü. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


Formülü tablodaki hücreye koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Tablodaki satır ofseti. |
| columnOffset | int | Tablodaki sütun ofseti. |
| formula | java.lang.String | Hücrenin formülü. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Değeri hücreye koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Tablodaki satır ofseti. |
| columnOffset | int | Tablodaki sütun ofseti. |
| değer | java.lang.Object | Hücre değeri. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


Değeri hücreye koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Tablodaki satır ofseti. |
| columnOffset | int | Tablodaki sütun ofseti. |
| değer | java.lang.Object | Hücre değeri. |
| isTotalsRowLabel | boolean | Toplam satırı için bir etiket olup olmadığını gösterir, yalnızca toplam satırda çalışır. False ise ve bu satır toplam satırsa, yeni bir satır eklenecektir. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Bu tabloya uygulanan otomatik filtreyi kaldırır.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Liste nesnesinin aralığını yeniden boyutlandırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Yeni aralığın başlangıç satır indeksi. |
| startColumn | int | Yeni aralığın başlangıç sütun indeksi. |
| endRow | int | Yeni aralığın bitiş satır indeksi. |
| endColumn | int | Yeni aralığın bitiş sütun indeksi. |
| hasHeaders | boolean | Bu tablonun başlıkları olup olmadığı. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


Alternatif açıklamayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Alternatif metni ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Tablonun yorumunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Tablonun görüntülenen adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


Bu tabloya otomatik filtre uygulanıp uygulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


Bu Tablonun başlık satırını gösterip göstermeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


Tablodaki ilk sütunun uygulanan stil olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


Tablodaki son sütunun uygulanan stil olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


Bu TAble'in toplam satırını gösterip göstermeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


Tablo stil adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


Yerleşik tablo stilini alır.

Bakınız [TableStyleType](../../com.aspose.cells/tablestyletype).

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
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Tüm liste sütunlarının adını tablodaki hücrelere günceller.

**Remarks**

Tablonun başlık satırındaki hücrelerin değeri, ListColumn adının aynı olması gerekir; Cell.PutValue, performans için ListColumn adını otomatik olarak değiştirmez.

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

