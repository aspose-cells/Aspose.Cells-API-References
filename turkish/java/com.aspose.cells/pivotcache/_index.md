---
title: "PivotCache"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bazı PivotTable raporları için bellek önbelleğini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

Bazı PivotTable raporları için bellek önbelleğini temsil eder.

**Remarks**

Tüm veriler bu önbellekte toplanacak ve pivot tablo yalnızca bu önbellekten veri alacak, veri kaynağına doğrudan erişmeyecek. Eğer bazı [PivotTable](../../com.aspose.cells/pivottable)s veri kaynağı aynıysa, bir pivot önbelleği kullanacaklar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [dispose()](#dispose--) | Tüm kaynakları serbest bırak. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Kullanılmayan öğelerin atılmadan önce izin verilecek sayısını alır. |
| [getPivotTables()](#getPivotTables--) | Bu pivot önbelleğine sahip tüm pivot tabloları alır. |
| [getSourceType()](#getSourceType--) | [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype) öğesini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Veri kaynağından verileri yeniler ve veri kaynağı bu pivot önbelleği olan tüm pivot tablolarının görünümü için verileri hesaplar. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Veri kaynağından verileri yeniler ve veri kaynağı bu pivot önbelleği olan tüm pivot tablolarının görünümü için verileri hesaplar. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Kullanılmayan öğelerin atılmadan önce izin verilecek sayısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotCache() {#PivotCache--}
```
public PivotCache()
```


### dispose() {#dispose--}
```
public abstract void dispose()
```


Tüm kaynakları serbest bırak.

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
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Kullanılmayan öğelerin atılmadan önce izin verilecek sayısını alır. Bu değer -2'den büyük ve 1048577'den küçük olmalıdır. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


Bu pivot önbelleğine sahip tüm pivot tabloları alır.

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


[PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype) öğesini alır.

[PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype) öğesine bakın.

**Returns:**
byte
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




### refresh() {#refresh--}
```
public int refresh()
```


Veri kaynağından verileri yeniler ve veri kaynağı bu pivot önbelleği olan tüm pivot tablolarının görünümü için verileri hesaplar.

**Remarks**

Eğer table1 ve table2 bu önbelleği kullanıyorsa, iki tablo hesaplanacaktır. Dosyadaki tüm pivot tabloları ve grafikleri yenilemek için sadece [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) metodunu çağırmanız yeterlidir.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Veri kaynağından verileri yeniler ve veri kaynağı bu pivot önbelleği olan tüm pivot tablolarının görünümü için verileri hesaplar.

**Remarks**

Dosyadaki tüm pivot tabloları ve grafikleri yenilemek için sadece [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) metodunu çağırmanız yeterlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Pivot tablonun veri kaynağını yenileme seçenekleri. |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Kullanılmayan öğelerin atılmadan önce izin verilecek sayısını ayarlar. Bu değer -2'den büyük ve 1048577'den küçük olmalıdır. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

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

