---
title: "PivotTableCalculateOption"
second_title: "Aspose.Cells for Java API Referansı"
description: "PivotTable verilerini hesaplama seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivottablecalculateoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableCalculateOption
```

PivotTable verilerini hesaplama seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PivotTableCalculateOption()](#PivotTableCalculateOption--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRefreshCharts()](#getRefreshCharts--) | Bu pivot tabloya dayalı grafiklerin yenilenip yenilenmediğini gösterir. |
| [getRefreshData()](#getRefreshData--) | Pivot tablonun veri kaynağının yenilenip yenilenmeyeceğini gösterir. |
| [getRefreshOption()](#getRefreshOption--) | Veri kaynağını pivot önbelleğe yenilemek için seçenekleri alır. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Eksik pivot öğelerinin nasıl ayrılacağını temsil eder. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRefreshCharts(boolean value)](#setRefreshCharts-boolean-) | Bu pivot tabloya dayalı grafiklerin yenilenip yenilenmediğini gösterir. |
| [setRefreshData(boolean value)](#setRefreshData-boolean-) | Pivot tablonun veri kaynağının yenilenip yenilenmeyeceğini gösterir. |
| [setRefreshOption(PivotTableRefreshOption value)](#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-) | Veri kaynağını pivot önbelleğe yenilemek için seçenekleri ayarlar. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Eksik pivot öğelerinin nasıl ayrılacağını temsil eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableCalculateOption() {#PivotTableCalculateOption--}
```
public PivotTableCalculateOption()
```


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
### getRefreshCharts() {#getRefreshCharts--}
```
public boolean getRefreshCharts()
```


Bu pivot tabloya dayalı grafiklerin yenilenip yenilenmediğini gösterir.

**Returns:**
boolean
### getRefreshData() {#getRefreshData--}
```
public boolean getRefreshData()
```


Pivot tablonun veri kaynağının yenilenip yenilenmeyeceğini gösterir.

**Remarks**

Doğru ise, pivot önbelleği veri kaynağından yeniler, ardından aynı pivot önbelleğine dayalı tüm pivot tabloları hesaplar.

**Returns:**
boolean
### getRefreshOption() {#getRefreshOption--}
```
public PivotTableRefreshOption getRefreshOption()
```


Veri kaynağını pivot önbelleğe yenilemek için seçenekleri alır.

**Returns:**
[PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption)
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Eksik pivot öğelerinin nasıl ayrılacağını temsil eder.

Bakınız [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Yalnızca [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) doğru olduğunda çalışır.

**Returns:**
int
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




### setRefreshCharts(boolean value) {#setRefreshCharts-boolean-}
```
public void setRefreshCharts(boolean value)
```


Bu pivot tabloya dayalı grafiklerin yenilenip yenilenmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRefreshData(boolean value) {#setRefreshData-boolean-}
```
public void setRefreshData(boolean value)
```


Pivot tablonun veri kaynağının yenilenip yenilenmeyeceğini gösterir.

**Remarks**

Doğru ise, pivot önbelleği veri kaynağından yeniler, ardından aynı pivot önbelleğine dayalı tüm pivot tabloları hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRefreshOption(PivotTableRefreshOption value) {#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-}
```
public void setRefreshOption(PivotTableRefreshOption value)
```


Veri kaynağını pivot önbelleğe yenilemek için seçenekleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Eksik pivot öğelerinin nasıl ayrılacağını temsil eder.

Bakınız [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Yalnızca [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) doğru olduğunda çalışır.

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

