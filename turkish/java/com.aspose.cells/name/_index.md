---
title: "Name"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücre aralığı için tanımlanmış bir adı temsil eder."
type: docs
url: /tr/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

Hücre aralığı için tanımlanmış bir adı temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | İsmin yorumunu alır. |
| [getFullText()](#getFullText--) | Kapsam ayarıyla nesnenin tam ad metnini alır. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | [Name](../../com.aspose.cells/name) referansının R1C1 referansını alır. |
| [getRange()](#getRange--) | Bu isim bir aralığa işaret ediyorsa aralığı alır. |
| [getRange(boolean recalculate)](#getRange-boolean-) | Bu isim bir aralığa işaret ediyorsa aralığı alır. |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | Bu isim bir aralığa işaret ediyorsa aralığı alır. |
| [getRanges()](#getRanges--) | Bu isim tarafından referans verilen tüm aralıkları alır. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | Bu isim tarafından referans verilen tüm aralıkları alır. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | Bu isim tarafından referans verilen tüm referansları alır. |
| [getRefersTo()](#getRefersTo--) | İsmin başvurduğu formülü, eşittir işaretiyle başlayan, döndürür veya ayarlar. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | Bu Adın referansını alın. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | Belirtilen hücreye göre bu Adın referansını alın. |
| [getSheetIndex()](#getSheetIndex--) | Bu adın Çalışma Kitabı'na mı yoksa Çalışma Sayfası'na mı ait olduğunu gösterir. 0 = Genel ad, aksi takdirde sayfa indeksi (bir tabanlı). |
| [getText()](#getText--) | Nesnenin ad metnini alır. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Bu adın diğer formüller tarafından referans alınıp alınmadığını gösterir. |
| [isVisible()](#isVisible--) | Adın görünür olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | Adın yorumunu ayarlar. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | R1C1 referansını [Ad](../../com.aspose.cells/name) için ayarlar. |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | İsmin başvurduğu formülü, eşittir işaretiyle başlayan, döndürür veya ayarlar. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | Bu Adın referansını ayarla. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Bu adın Çalışma Kitabı'na mı yoksa Çalışma Sayfası'na mı ait olduğunu gösterir. 0 = Genel ad, aksi takdirde sayfa indeksi (bir tabanlı). |
| [setText(String value)](#setText-java.lang.String-) | Nesnenin ad metnini alır. |
| [setVisible(boolean value)](#setVisible-boolean-) | Adın görünür olup olmadığını gösterir. |
| [toString()](#toString--) | Geçerli Range nesnesini temsil eden bir dize döndürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


Adın yorumunu alır. Yalnızca Excel 2007 veya daha yeni sürümler için geçerlidir.

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


Kapsam ayarıyla nesnenin tam ad metnini alır.

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


[Name](../../com.aspose.cells/name) referansının R1C1 referansını alır.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Bu isim bir aralığa işaret ediyorsa aralığı alır.

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


Bu isim bir aralığa işaret ediyorsa aralığı alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yeniden hesapla | boolean | Bu ad bu çağrıdan önce hesaplandıysa yeniden hesaplayıp hesaplamayacağını. |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


Bu ad bir aralığa işaret ediyorsa aralığı alır. Bu adın referansı mutlak değilse, aralık farklı hücreler için değişebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | İlgili sayfa indeksi. |
| satır | int | İlgili satır indeksi. |
| sütun | int | İlgili sütun indeksi |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Bu isim tarafından referans verilen tüm aralıkları alır.

**Returns:**
com.aspose.cells.Range[] - Tüm aralıklar.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


Bu isim tarafından referans verilen tüm aralıkları alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yeniden hesapla | boolean | Bu ad bu çağrıdan önce hesaplandıysa yeniden hesaplayıp hesaplamayacağını. |

**Returns:**
com.aspose.cells.Range[] - Tüm aralıklar.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


Bu isim tarafından referans verilen tüm referansları alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yeniden hesapla | boolean | Bu ad bu çağrıdan önce hesaplandıysa yeniden hesaplayıp hesaplamayacağını. |

**Returns:**
com.aspose.cells.ReferredArea[] - Tüm aralıklar.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


İsmin başvurduğu formülü, eşittir işaretiyle başlayan, döndürür veya ayarlar.

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


Bu Adın referansını alın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Referansın R1C1 formatında biçimlendirilip biçimlendirilmesi gerekir. |
| isLocal | boolean | Referansın yerel ayara göre biçimlendirilip biçimlendirilmesi gerekir. |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


Belirtilen hücreye göre bu Adın referansını alın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Referansın R1C1 formatında biçimlendirilip biçimlendirilmesi gerekir. |
| isLocal | boolean | Referansın yerel ayara göre biçimlendirilip biçimlendirilmesi gerekir. |
| satır | int | Hücrenin satır indeksi. |
| sütun | int | Hücrenin sütun indeksi. |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Bu adın Çalışma Kitabı'na mı yoksa Çalışma Sayfası'na mı ait olduğunu gösterir. 0 = Genel ad, aksi takdirde sayfa indeksi (bir tabanlı).

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Nesnenin ad metnini alır.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Bu adın diğer formüller tarafından referans alınıp alınmadığını gösterir.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Adın görünür olup olmadığını gösterir.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Adın yorumunu ayarlar. Yalnızca Excel 2007 veya daha yeni sürümler için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


R1C1 referansını [Ad](../../com.aspose.cells/name) için ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


İsmin başvurduğu formülü, eşittir işaretiyle başlayan, döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


Bu Adın referansını ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| refersTo | java.lang.String | Referans. |
| isR1C1 | boolean | Referansın R1C1 formatında olup olmadığı. |
| isLocal | boolean | Referansın yerel formatta olup olmadığı. |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


Bu adın Çalışma Kitabı'na mı yoksa Çalışma Sayfası'na mı ait olduğunu gösterir. 0 = Genel ad, aksi takdirde sayfa indeksi (bir tabanlı).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Nesnenin ad metnini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Adın görünür olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### toString() {#toString--}
```
public String toString()
```


Geçerli Range nesnesini temsil eden bir dize döndürür.

**Returns:**
java.lang.String -
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

