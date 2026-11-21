---
title: "PivotTableRefreshOption"
second_title: "Aspose.Cells for Java API Referansı"
description: "PivotTable veri kaynağını yenileme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

PivotTable veri kaynağını yenileme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | PivotTable veri kaynağını yenileme seçeneklerini temsil eder. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | Maksimum ve minimum değerler değişmediğinde önbelleğe alınmış yerel grup verilerinin korunup korunmayacağını gösterir. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Eksik pivot öğelerinin nasıl ayrılacağını temsil eder. |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | Pivot öğelerinin orijinal sırasının eski veri kaynağı olarak korunup korunmayacağını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | Maksimum ve minimum değerler değişmediğinde önbelleğe alınmış yerel grup verilerinin korunup korunmayacağını gösterir. |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | Pivot öğelerinin orijinal sırasının eski veri kaynağı olarak korunup korunmayacağını gösterir. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Eksik pivot öğelerinin nasıl ayrılacağını temsil eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


PivotTable veri kaynağını yenileme seçeneklerini temsil eder.

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


Maksimum ve minimum değerler değişmediğinde önbelleğe alınmış yerel grup verilerinin korunup korunmayacağını gösterir. Varsayılan değer false'tur, bu da grubun yerel ayarlarla yenileneceği anlamına gelir.

**Remarks**

Bu geçici bir çözümdür, lütfen pivot tablolarını [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) uygulayarak yerelleştirin.

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Eksik pivot öğelerinin nasıl ayrılacağını temsil eder.

Bakınız [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isKeepOriginalOrder() {#isKeepOriginalOrder--}
```
public boolean isKeepOriginalOrder()
```


Pivot öğelerinin orijinal sırasının eski veri kaynağı olarak korunup korunmayacağını gösterir.

**Remarks**

Sıralanmamış pivot alanı için yalnızca geçerlidir. Böyle bir pivot alanı yenilendiğinde, Ms Excel eski veri kaynağının orijinal sırasını korur. Bu özelliğin varsayılan değeri true'dır ve Ms Excel ile aynı davranışı temsil eder. Kullanıcı, pivot alanının yeni veri kaynağındaki veriler gibi tamamen yenilenmesini istiyorsa, bu özellik false olarak ayarlanmalıdır.

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




### setKeepCachedLocalGroupData(boolean value) {#setKeepCachedLocalGroupData-boolean-}
```
public void setKeepCachedLocalGroupData(boolean value)
```


Maksimum ve minimum değerler değişmediğinde önbelleğe alınmış yerel grup verilerinin korunup korunmayacağını gösterir. Varsayılan değer false'tur, bu da grubun yerel ayarlarla yenileneceği anlamına gelir.

**Remarks**

Bu geçici bir çözümdür, lütfen pivot tablolarını [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) uygulayarak yerelleştirin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


Pivot öğelerinin orijinal sırasının eski veri kaynağı olarak korunup korunmayacağını gösterir.

**Remarks**

Sıralanmamış pivot alanı için yalnızca geçerlidir. Böyle bir pivot alanı yenilendiğinde, Ms Excel eski veri kaynağının orijinal sırasını korur. Bu özelliğin varsayılan değeri true'dır ve Ms Excel ile aynı davranışı temsil eder. Kullanıcı, pivot alanının yeni veri kaynağındaki veriler gibi tamamen yenilenmesini istiyorsa, bu özellik false olarak ayarlanmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Eksik pivot öğelerinin nasıl ayrılacağını temsil eder.

Bakınız [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

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

