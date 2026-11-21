---
title: "GridCalculationData"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir fonksiyonun (örneğin fonksiyon adı parametreleri ... vb.) hesaplanması sırasında gereken verileri temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Bir fonksiyonun hesaplanması sırasında gerekli verileri temsil eder; örneğin fonksiyon adı, parametreler, vb.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Bu fonksiyon için hesaplanan değeri alır. |
| [getCell()](#getCell--) | Fonksiyonun bulunduğu Cell nesnesini alır. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Hesaplanacak fonksiyon adını alır. |
| [getParamCount()](#getParamCount--) | Parametre sayısını alır |
| [getParamText(int index)](#getParamText-int-) | Verilen indeksdeki parametrenin gerçek metnini alır. |
| [getParamValue(int index)](#getParamValue-int-) | Verilen indeksdeki parametrenin temsil edilen değer nesnesini alır. |
| [getWorkbook()](#getWorkbook--) | Fonksiyonun bulunduğu Workbook nesnesini alır. |
| [getWorksheet()](#getWorksheet--) | Fonksiyonun bulunduğu Workbook nesnesini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Bu fonksiyon için hesaplanmış değeri ayarlar. |
| [toString()](#toString--) |  |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Bu fonksiyon için hesaplanan değeri alır.

**Remarks**

Kullanıcı, motorun desteklediği fonksiyonlar için bu özelliği kendi özel hesaplama motorunda ayarlamalıdır ve ayarlanan değer bu özellik alındığında geri döndürülür. Bu özellik ayarlamadan önce alındığında, fonksiyon Aspose.Cells'in varsayılan hesaplama motoru tarafından hesaplanır ve hesaplanan değer geri döndürülür.

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public GridCell getCell()
```


Fonksiyonun bulunduğu Cell nesnesini alır.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


Hesaplanacak fonksiyon adını alır.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


Parametre sayısını alır

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Verilen indeksdeki parametrenin gerçek metnini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | parametrenin indeksi (0 tabanlı) |

**Returns:**
java.lang.String - parametrenin literal metni.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Verilen indeksdeki parametrenin temsil edilen değer nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | parametrenin indeksi (0 tabanlı) |

**Returns:**
java.lang.Object - Parametre düz bir değer ise, düz değeri döndürür. Parametre bir referans ise, ReferredArea nesnesini döndürür.
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Fonksiyonun bulunduğu Workbook nesnesini alır.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getWorksheet() {#getWorksheet--}
```
public GridWorksheet getWorksheet()
```


Fonksiyonun bulunduğu Workbook nesnesini alır.

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


Bu fonksiyon için hesaplanmış değeri ayarlar.

**Remarks**

Kullanıcı, motorun desteklediği fonksiyonlar için bu özelliği kendi özel hesaplama motorunda ayarlamalıdır ve ayarlanan değer bu özellik alındığında geri döndürülür. Bu özellik ayarlamadan önce alındığında, fonksiyon Aspose.Cells'in varsayılan hesaplama motoru tarafından hesaplanır ve hesaplanan değer geri döndürülür.

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

