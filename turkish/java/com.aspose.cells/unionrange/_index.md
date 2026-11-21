---
title: "UnionRange"
second_title: "Aspose.Cells for Java API Referansı"
description: "Birleşik aralığı temsil eder."
type: docs
url: /tr/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

Birleşik aralığı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tüm bir aralık için biçimleri uygular. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | Aralığı yapıştırma özel seçenekleriyle kopyalama. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | Aralıktaki tüm hücre sayısını alır. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Aralıktaki satır sayısını alır. |
| [getFirstColumn()](#getFirstColumn--) | Aralığın ilk sütununun indeksini alır. |
| [getFirstRow()](#getFirstRow--) | Aralığın ilk satırının indeksini alır. |
| [getHyperlinks()](#getHyperlinks--) | Aralıktaki tüm köprüleri alır. |
| [getName()](#getName--) | Aralığın adını alır. |
| [getRangeCount()](#getRangeCount--) | Aralıkların sayısını alır. |
| [getRanges()](#getRanges--) | Tüm birleşim aralıklarını alır. |
| [getRefersTo()](#getRefersTo--) | Aralığın referansını alır. |
| [getRowCount()](#getRowCount--) | Aralıktaki satır sayısını alır. |
| [getValue()](#getValue--) | Aralığın değerlerini alır. |
| [hasRange()](#hasRange--) | Bu nesnenin aralığı olup olmadığını gösterir. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | Başka bir aralıkla kesişir. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | Başka bir aralıkla kesişir. |
| [intersect(String range)](#intersect-java.lang.String-) | Başka bir aralıkla kesişir. |
| [iterator()](#iterator--) | Bu Aralıktaki hücreler için enumeratörü alır. |
| [merge()](#merge--) | Bir hücre aralığını tek bir hücreye birleştirir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Bir değeri aralığa yerleştirir, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [setName(String value)](#setName-java.lang.String-) | Aralığın adını ayarlar. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Hücre aralığının etrafına dış kenarlıkları ayarlar. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Aralığın stilini ayarlar. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Aralığın değerlerini ayarlar. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | Bu aralıktaki birleştirilmiş hücrelerin birleşimini kaldırır. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | Aralıkları birleştir. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | Başka bir aralığı birleştir. |
| [union(String range)](#union-java.lang.String-) | Başka bir aralığı birleştir. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


Aralığı yapıştırma özel seçenekleriyle kopyalama.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | Kaynak aralık. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Yapıştırma özel seçenekleri. |

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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


Aralıktaki tüm hücre sayısını alır.

**Returns:**
int
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


Aralıktaki satır sayısını alır.

**Remarks**

Yalnızca bir aralık içerdiğinde etkili olur.

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Aralığın ilk sütununun indeksini alır.

**Remarks**

Yalnızca bir aralık içerdiğinde etkili olur.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Aralığın ilk satırının indeksini alır.

**Remarks**

Yalnızca bir aralık içerdiğinde etkili olur.

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Aralıktaki tüm köprüleri alır.

**Returns:**
com.aspose.cells.Hyperlink[]
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
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Aralıkların sayısını alır.

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Tüm birleşim aralıklarını alır.

**Returns:**
com.aspose.cells.Range[]
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

**Remarks**

Yalnızca bir aralık içerdiğinde etkili olur.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Aralığın değerlerini alır.

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


Bu nesnenin aralığı olup olmadığını gösterir.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


Başka bir aralıkla kesişir.

**Remarks**

İki birleşim aralığı kesişmiyorsa, null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Aralık. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


Başka bir aralıkla kesişir.

**Remarks**

İki birleşim aralığı kesişmiyorsa, null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | Aralık. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


Başka bir aralıkla kesişir.

**Remarks**

İki birleşim aralığı kesişmiyorsa, null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | java.lang.String | Aralık. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Bu Aralıktaki hücreler için enumeratörü alır.

**Remarks**

Dönen Enumerator ile öğeler dolaşılırken, hücreler koleksiyonu değiştirilmemelidir (örneğin yeni Cell/Row oluşturulmasına veya mevcut Cell/Row silinmesine neden olacak işlemler). Aksi takdirde enumerator tüm hücreleri doğru şekilde dolaşamayabilir (bazı öğeler tekrar tekrar dolaşılabilir veya atlanabilir).

**Returns:**
java.util.Iterator - Hücre enumeratörü
### merge() {#merge--}
```
public void merge()
```


Bir hücre aralığını tek bir hücreye birleştirir.

**Remarks**

Aralıktaki sol üst hücrenin adresi üzerinden birleştirilmiş hücreye referans ver.

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

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Aralığın stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Style nesnesi. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Aralığın değerlerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge() {#unMerge--}
```
public void unMerge()
```


Bu aralıktaki birleştirilmiş hücrelerin birleşimini kaldırır.

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


Aralıkları birleştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Aralıklar. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


Başka bir aralığı birleştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | Aralık. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


Başka bir aralığı birleştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | java.lang.String | Aralık. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

