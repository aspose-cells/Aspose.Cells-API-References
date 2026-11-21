---
title: "MultipleFilterCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çoklu filtre koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

Çoklu filtre koleksiyonunu temsil eder.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) kullanın. Bu özellik Haziran 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | Yeni bir örnek oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Bir tarih filtre kriteri değeri ekler. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Bir tarih saat filtresi kriteri değeri ekler. |
| [add(String filter)](#add-java.lang.String-) | Bir etiket filtre kriteri ekler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) veya bir dize değeri alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Filtre değerlerinin sayısını alır. |
| [getMatchBlank()](#getMatchBlank--) | Boş değerle filtreleme yapılıp yapılmayacağını gösterir. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Filtre değeri için yineleyiciyi al, |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Boş değerle filtreleme yapılıp yapılmayacağını gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


Yeni bir örnek oluşturur.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FilterColumn.FilterType'ı FilterType.MultipleFilters olarak ayarlayın, ardından FilterColumn.MultipleFilters'ı alın. Bu özellik Haziran 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


Bir tarih filtre kriteri değeri ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Tarih filtresinin türü. |
| yıl | int | Yıl. |
| ay | int | Ay. |
| gün | int | Gün. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


Bir tarih saat filtresi kriteri değeri ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Tarih filtresinin türü. |
| yıl | int | Yıl. |
| ay | int | Ay. |
| gün | int | Gün. |
| saat | int | Saat. |
| dakika | int | Dakika. |
| saniye | int | Saniye. |

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Bir etiket filtre kriteri ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filtre | java.lang.String | Filtre verileri. |

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
### get(int index) {#get-int-}
```
public Object get(int index)
```


[DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) veya bir dize değeri alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
java.lang.Object - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Filtre değerlerinin sayısını alır.

**Returns:**
int
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


Boş değerle filtreleme yapılıp yapılmayacağını gösterir.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Filtre değeri için yineleyiciyi al,

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


Boş değerle filtreleme yapılıp yapılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

