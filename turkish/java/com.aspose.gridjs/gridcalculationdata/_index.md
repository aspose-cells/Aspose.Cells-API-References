---
title: "GridCalculationData"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir fonksiyonun (örneğin fonksiyon adı parametreleri ... vb.) hesaplanması sırasında gereken verileri temsil eder."
type: docs
url: /tr/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Bir fonksiyonun hesaplanması sırasında gerekli verileri temsil eder; örneğin fonksiyon adı, parametreler, vb.

**Remarks**

Bu sınıf tarafından sağlanan tüm nesneler yalnızca "okuma" amacıyla kullanılabilir. Kullanıcı, formül hesaplama sürecinde Workbook'taki herhangi bir veriyi değiştirmemelidir, aksi takdirde beklenmeyen sonuçlar veya istisna oluşabilir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Bu fonksiyon için hesaplanan değeri alır. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Fonksiyonun bulunduğu Hücre Sütun indeksini alır. |
| [getFormula()](#getFormula--) | Fonksiyonun bulunduğu Hücre formülünü alır. |
| [getFunctionName()](#getFunctionName--) | Hesaplanacak fonksiyon adını alır. |
| [getParamCount()](#getParamCount--) | Parametre sayısını alır. |
| [getParamText(int index)](#getParamText-int-) | Verilen indeksdeki parametrenin gerçek metnini alır. |
| [getParamValue(int index)](#getParamValue-int-) | Verilen indeksdeki parametrenin temsil edilen değer nesnesini alır. |
| [getRow()](#getRow--) | Fonksiyonun bulunduğu Hücre Satır indeksini alır. |
| [getSheetName()](#getSheetName--) | Fonksiyonun bulunduğu çalışma sayfası adını alır. |
| [getStringValue()](#getStringValue--) | Fonksiyonun bulunduğu Hücre DisplayStringValue değerini alır. |
| [getValue()](#getValue--) | Fonksiyonun bulunduğu Hücre değerini alır. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Fonksiyonun bulunduğu Hücre Sütun indeksini alır.

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


Fonksiyonun bulunduğu Hücre formülünü alır.

**Returns:**
java.lang.String
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


Parametre sayısını alır.

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
| dizin | int | Parametrenin indeksi (0 tabanlı). |

**Returns:**
java.lang.String - Parametrenin gerçek metni.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Verilen indeksdeki parametrenin temsil edilen değer nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Parametrenin indeksi (0 tabanlı). |

**Returns:**
java.lang.Object - Parametre düz bir değer ise, düz değeri döndürür. Parametre bir referans ise, ReferredArea nesnesini döndürür.
### getRow() {#getRow--}
```
public int getRow()
```


Fonksiyonun bulunduğu Hücre Satır indeksini alır.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Fonksiyonun bulunduğu çalışma sayfası adını alır.

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Fonksiyonun bulunduğu Hücre DisplayStringValue değerini alır.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Fonksiyonun bulunduğu Hücre değerini alır.

**Returns:**
java.lang.Object
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

