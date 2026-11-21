---
title: "Range"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir elektronik tablo içinde hücre aralığını temsil eden nesneyi kapsar."
type: docs
url: /tr/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

Bir elektronik tablo içinde hücre aralığını temsil eden nesneyi kapsar.

**Remarks**

Range sınıfı, bir Excel elektronik tablosundaki bir bölgeyi temsil eder. Bununla, bölgenin biçimini ayarlayabilir ve değerini belirleyebilirsiniz. Ayrıca Excel bölgesini kolayca kopyalayabilirsiniz.

**Example**

Aşağıdaki örnek, bir Excel aralığı oluşturmayı ve aralığın değerini ayarlamayı gösterir.

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         // Create a range (A1:D3).
         Range range = cells.createRange("A1", "D3");
         // Set value to the range.
         range.setValue("Hello");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | Sınıf yapıcı. |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | Sınıf yapıcı. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tüm bir aralık için biçimleri uygular. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | Hedef aralığı otomatik olarak doldurur. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | Hedef aralığı otomatik olarak doldurur. |
| [clear()](#clear--) | Bu aralığı temizler. |
| [clearComments()](#clearComments--) | Bu aralığın yorumlarını temizler. |
| [clearContents()](#clearContents--) | Bu aralığın içeriğini temizler. |
| [clearFormats()](#clearFormats--) | Bu aralığın biçimlerini temizler. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | Yalnızca köprüleri kaldırır. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | Kaynak bir aralıktaki verileri (formüller dahil), biçimlendirmeyi, çizim nesnelerini vb. kopyalar. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | Aralığı yapıştırma özel seçenekleriyle kopyalama. |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | Kaynak bir aralıktaki hücre verilerini (formüller dahil) kopyalar. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | Bir kaynak aralıktan stil ayarlarını kopyalar. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | Bir kaynak aralıktan hücre değerini kopyalar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | Bu aralıktaki [Cell](../../com.aspose.cells/cell) nesnesini alır. |
| [getAddress()](#getAddress--) | Aralığın adresini alır. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | Bu aralıktaki [Cell](../../com.aspose.cells/cell) nesnesini veya null değerini alır. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Aralıktaki sütun sayısını alır. |
| [getColumnWidth()](#getColumnWidth--) | Bu aralığın sütun genişliğini ayarlar veya alır. |
| [getCurrentRegion()](#getCurrentRegion--) | Geçerli bölgeyi temsil eden bir Range nesnesi döndürür. |
| [getEntireColumn()](#getEntireColumn--) | Belirtilen aralığı içeren tüm sütunu (veya sütunları) temsil eden bir Range nesnesini alır. |
| [getEntireRow()](#getEntireRow--) | Belirtilen aralığı içeren tüm satırı (veya satırları) temsil eden bir Range nesnesini alır. |
| [getFirstColumn()](#getFirstColumn--) | Aralığın ilk sütununun indeksini alır. |
| [getFirstRow()](#getFirstRow--) | Aralığın ilk satırının indeksini alır. |
| [getHeight()](#getHeight--) | Bir aralığın genişliğini puan cinsinden alır. |
| [getHyperlinks()](#getHyperlinks--) | Aralıktaki tüm köprüleri alır. |
| [getLeft()](#getLeft--) | A sütununun sol kenarından aralığın sol kenarına kadar olan mesafeyi puan cinsinden alır. |
| [getName()](#getName--) | Aralığın adını alır. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | Ofset ile [Range](../../com.aspose.cells/range) aralığını alır. |
| [getRefersTo()](#getRefersTo--) | Aralığın referansını alır. |
| [getRowCount()](#getRowCount--) | Aralıktaki satır sayısını alır. |
| [getRowHeight()](#getRowHeight--) | Bu aralıktaki satırların yüksekliğini ayarlar veya alır. |
| [getTop()](#getTop--) | 1. satırın üst kenarından aralığın üst kenarına kadar olan mesafeyi puan cinsinden alır. |
| [getValue()](#getValue--) | Aralığın değerini alır. |
| [getWidth()](#getWidth--) | Bir aralığın genişliğini puan cinsinden alır. |
| [getWorksheet()](#getWorksheet--) | Bu aralığı içeren [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) nesnesini alır. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | İki aralığın dikdörtgen kesişimini temsil eden bir [Range](../../com.aspose.cells/range) nesnesi döndürür. |
| [isBlank()](#isBlank--) | Aralığın değer içerip içermediğini gösterir. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | Aralığın kesişip kesişmediğini gösterir. |
| [iterator()](#iterator--) | Bu Aralıktaki hücreler için enumeratörü alır. |
| [merge()](#merge--) | Bir hücre aralığını tek bir hücreye birleştirir. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | Geçerli aralığı hedef aralığa taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Bir değeri aralığa yerleştirir, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Bu aralığın sütun genişliğini ayarlar veya alır. |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | Aralığın iç kenarlıklarını ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Aralığın adını ayarlar. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | Hücre aralığının etrafına dış kenarlık ayarlar. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | Hücre aralığının etrafına dış kenarlık ayarlar. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Hücre aralığının etrafına dış kenarlıkları ayarlar. |
| [setRowHeight(double value)](#setRowHeight-double-) | Bu aralıktaki satırların yüksekliğini ayarlar veya alır. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Aralığın stilini ayarlar. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Hücre stilini uygula. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Aralığın değerini ayarlar. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | Aralığı html'ye dönüştür. |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | Aralığı görüntüye dönüştürür. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | Aralığı JSON değerine dönüştür. |
| [toString()](#toString--) | Geçerli Range nesnesini temsil eden bir dize döndürür. |
| [transpose()](#transpose--) | Verileri satırlardan sütunlara veya tersine (döndürerek) transpoze eder. |
| [unMerge()](#unMerge--) | Bu aralıktaki birleştirilmiş hücrelerin birleşimini kaldırır. |
| [union(Range range)](#union-com.aspose.cells.Range-) | İki aralığın birleşimini döndürür. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | İki aralığın birleşim sonucunu döndürür. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | İki aralığın birleşim sonucunu döndürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


Sınıf yapıcı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Aralık. |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


Sınıf yapıcı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | int | Bu aralığın ilk sütunu (sıfır tabanlı). |
| rowNumber | int | Satır sayısı (bir tabanlı) |
| columnNumber | int | Sütun sayısı (bir tabanlı) |
| cells | [Cells](../../com.aspose.cells/cells) | Range nesnesi bu Cells nesnesine aittir. |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adres | java.lang.String | Köprü adresi. |
| textToDisplay | java.lang.String | Belirtilen bağlantı için görüntülenecek metin. |
| screenTip | java.lang.String | Belirtilen bağlantı için ekran ipucu metni. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tüm bir aralık için biçimleri uygular.

**Remarks**

Bu aralıktaki her hücre bir [Style](../../com.aspose.cells/style) nesnesi içerir. Bu nedenle bellek yoğun bir yöntemdir. Lütfen dikkatli kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Uygulanacak stil nesnesi. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


Hedef aralığı otomatik olarak doldurur.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue(1);
         cells.get("A2").putValue(2);
         Range source = cells.createRange("A1:A2");
         Range target = cells.createRange("A3:A10");
         //fill 3,4,5....10 to the range A3:A10
         source.autoFill(target);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | hedef aralık. |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


Hedef aralığı otomatik olarak doldurur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | Hedef aralık. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). Otomatik doldurma türü. |

### clear() {#clear--}
```
public void clear()
```


Bu aralığı temizler.

### clearComments() {#clearComments--}
```
public void clearComments()
```


Bu aralığın yorumlarını temizler.

### clearContents() {#clearContents--}
```
public void clearContents()
```


Bu aralığın içeriğini temizler.

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


Bu aralığın biçimlerini temizler.

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


Yalnızca köprüleri kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| clearFormat | boolean | Köprülerin biçimini temizleyip temizlemeyeceğini gösterir. |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


Kaynak bir aralıktaki verileri (formüller dahil), biçimlendirmeyi, çizim nesnelerini vb. kopyalar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A6:A10");
         //Copy the range.
         range1.copy(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Kaynak [Range](../../com.aspose.cells/range) nesnesi. |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


Aralığı yapıştırma özel seçenekleriyle kopyalama.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Kaynak aralık. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Yapıştırma özel seçenekleri. |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


Kaynak bir aralıktaki hücre verilerini (formüller dahil) kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Kaynak [Range](../../com.aspose.cells/range) nesnesi. |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


Bir kaynak aralıktan stil ayarlarını kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Kaynak [Range](../../com.aspose.cells/range) nesnesi. |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


Bir kaynak aralıktan hücre değerini kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Kaynak [Range](../../com.aspose.cells/range) nesnesi. |

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
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


Bu aralıktaki [Cell](../../com.aspose.cells/cell) nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Bu aralıktaki satır ofseti, sıfır tabanlı. |
| columnOffset | int | Bu aralıktaki sütun ofseti, sıfır tabanlı. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


Aralığın adresini alır.

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


Bu aralıktaki [Cell](../../com.aspose.cells/cell) nesnesini veya null değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Bu aralıktaki satır ofseti, sıfır tabanlı. |
| columnOffset | int | Bu aralıktaki sütun ofseti, sıfır tabanlı. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Aralıktaki sütun sayısını alır.

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Bu aralığın sütun genişliğini ayarlar veya alır.

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


Geçerli bölgeyi temsil eden bir Range nesnesi döndürür. Geçerli bölge, boş satırların ve boş sütunların herhangi bir kombinasyonu ile sınırlanan bir aralıktır.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


Belirtilen aralığı içeren tüm sütunu (veya sütunları) temsil eden bir Range nesnesini alır.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


Belirtilen aralığı içeren tüm satırı (veya satırları) temsil eden bir Range nesnesini alır.

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Aralığın ilk sütununun indeksini alır.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Aralığın ilk satırının indeksini alır.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Bir aralığın genişliğini puan cinsinden alır.

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Aralıktaki tüm köprüleri alır.

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


A sütununun sol kenarından aralığın sol kenarına kadar olan mesafeyi puan cinsinden alır.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


Aralığın adını alır.

**Remarks**

Adlandırılmış aralık desteklenir. Örneğin,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


Ofset ile [Range](../../com.aspose.cells/range) aralığını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Bu aralıktaki satır ofseti, sıfır tabanlı. |
| columnOffset | int | Bu aralıktaki sütun ofseti, sıfır tabanlı. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Aralığın referansını alır.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Aralıktaki satır sayısını alır.

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Bu aralıktaki satırların yüksekliğini ayarlar veya alır.

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


1. satırın üst kenarından aralığın üst kenarına kadar olan mesafeyi puan cinsinden alır.

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


Aralığın değerini alır.

**Remarks**

Aralık birden fazla hücre içeriyorsa, döndürülen/uygulanan nesne Object[][]. olmalıdır.

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


Bir aralığın genişliğini puan cinsinden alır.

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Bu aralığı içeren [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) nesnesini alır.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range range) {#intersect-com.aspose.cells.Range-}
```
public Range intersect(Range range)
```


İki aralığın dikdörtgen kesişimini temsil eden bir [Range](../../com.aspose.cells/range) nesnesi döndürür.

**Remarks**

İki aralık kesişmiyorsa, null döndürür.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A3:A10");
         //Get intersected range of the two ranges.
         Range intersectRange = range1.intersect(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Kesişen aralık. |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Aralığın değer içerip içermediğini gösterir.

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


Aralığın kesişip kesişmediğini gösterir.

**Remarks**

İki aralık aynı çalışma sayfasında değilse, false döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Aralık. |

**Returns:**
boolean - Aralığın kesişip kesişmediği.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Bu Aralıktaki hücreler için enumeratörü alır.

**Remarks**

Dönen Enumerator ile öğeler dolaşılırken, hücreler koleksiyonu değiştirilmemelidir (örneğin yeni Cell/Row oluşturulmasına veya mevcut Cell/Row silinmesine neden olacak işlemler). Aksi takdirde enumerator tüm hücreleri doğru şekilde dolaşamayabilir (bazı öğeler tekrar tekrar dolaşılabilir veya atlanabilir).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.createRange("B2:C3").iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - Hücre enumeratörü
### merge() {#merge--}
```
public void merge()
```


Bir hücre aralığını tek bir hücreye birleştirir.

**Remarks**

Aralıktaki sol üst hücrenin adresi üzerinden birleştirilmiş hücreye referans ver.

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


Geçerli aralığı hedef aralığa taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destRow | int | Hedef aralığın başlangıç satırı. |
| destColumn | int | Hedef aralığın başlangıç sütunu. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Bir değeri aralığa yerleştirir, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | java.lang.String | Girdi değeri |
| isConverted | boolean | True: uygun olduğunda diğer veri tipine dönüştürülür. |
| setStyle | boolean | True: diğer veri tipine dönüştürürken sayı biçimini hücrenin stiline ayarlar |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Bu aralığın sütun genişliğini ayarlar veya alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


Aralığın iç kenarlıklarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). İç sınır türü, yalnızca [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) ve [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL) olabilir. |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlık stili. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Kenarlığın rengi. |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Aralığın adını ayarlar.

**Remarks**

Adlandırılmış aralık desteklenir. Örneğin,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


Hücre aralığının etrafına dış kenarlık ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Kenarlık kenarı. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlık stili. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Kenarlık rengi. |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


Hücre aralığının etrafına dış kenarlık ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Kenarlık kenarı. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlık stili. |
| borderColor | [Color](../../com.aspose.cells/color) | Kenarlık rengi. |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlık stili. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Kenarlık rengi. |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlık stili. |
| borderColor | [Color](../../com.aspose.cells/color) | Kenarlık rengi. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Hücre aralığının etrafına dış kenarlıkları ayarlar.

**Remarks**

borderStyles ve borderStyles uzunlukları ikisi de 4 olmalıdır. borderStyles ve borderStyles sırası üst,alt,sol,sağ olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlık stilleri. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Kenarlık renkleri. |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Bu aralıktaki satırların yüksekliğini ayarlar veya alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Aralığın stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Style nesnesi. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Hücre stilini uygula.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Hücre stili. |
| explicitFlag | boolean | True, yalnızca açıkça ayarlanmış biçimlendirmeyi üzerine yazar. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Aralığın değerini ayarlar.

**Remarks**

Aralık birden fazla hücre içeriyorsa, döndürülen/uygulanan nesne Object[][]. olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


Aralığı html'ye dönüştür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | Aralığı html'ye dönüştürme seçenekleri. |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


Aralığı görüntüye dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Bu aralığı görüntüye dönüştürme seçenekleri. |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


Aralığı JSON değerine dönüştür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Dönüştürme seçenekleri. |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Geçerli Range nesnesini temsil eden bir dize döndürür.

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


Verileri satırlardan sütunlara veya tersine (döndürerek) transpoze eder.

### unMerge() {#unMerge--}
```
public void unMerge()
```


Bu aralıktaki birleştirilmiş hücrelerin birleşimini kaldırır.

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


İki aralığın birleşimini döndürür.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen Range.UnionRanges() yöntemini kullanın. Bu yöntem Kasım 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Aralık |

**Returns:**
java.util.ArrayList - İki aralığın birleşimi.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


İki aralığın birleşim sonucunu döndürür.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen Range.UnionRanges() yöntemini kullanın. Bu yöntem Mayıs 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Aralık |

**Returns:**
com.aspose.cells.Range[] - İki aralığın birleşimi.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


İki aralığın birleşim sonucunu döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Aralık |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - The union of two ranges.
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

