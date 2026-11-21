---
title: "JsonCacheOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "GridJs içinde JSON önbellekleme için yapılandırma seçenekleri."
type: docs
url: /tr/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

GridJs'de JSON önbellekleme için yapılandırma seçenekleri. Hem bellek (L1) hem de disk (L2) önbellek davranışını kontrol eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | Disk önbelleğinin Gzip kullanarak sıkıştırılıp sıkıştırılmayacağını alır (varsayılan: true). |
| [getDiskPath()](#getDiskPath--) | Disk önbellek dizin yolunu alır. |
| [getDiskTtl()](#getDiskTtl--) | Disk önbellek için dakikalar cinsinden TTL'yi alır (varsayılan: 1440). |
| [getEnable()](#getEnable--) | Daha hızlı yanıt için JSON önbelleklemenin etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnableDisk()](#getEnableDisk--) | Disk önbelleğin etkinleştirilip etkinleştirilmeyeceğini alır (varsayılan: true). |
| [getImplementation()](#getImplementation--) | Özel JSON önbellek uygulamasını alır. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | Maksimum disk önbellek boyutunu MB cinsinden alır (varsayılan: 500 MB). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | Bellek önbelleğindeki maksimum giriş sayısını alır (varsayılan: 1000). |
| [getMemoryTtl()](#getMemoryTtl--) | Bellek önbellek için dakikalar cinsinden TTL'yi alır (varsayılan: 60). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | Disk önbelleğin Gzip kullanarak sıkıştırılıp sıkıştırılmayacağını ayarlar (varsayılan: true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | Disk önbellek dizin yolunu ayarlar. |
| [setDiskTtl(long value)](#setDiskTtl-long-) | Disk önbellek için dakikalar cinsinden TTL'yi ayarlar (varsayılan: 1440). |
| [setEnable(boolean value)](#setEnable-boolean-) | Daha hızlı yanıt için JSON önbelleklemenin etkinleştirilip etkinleştirilmeyeceğini ayarlar. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | Disk önbelleğin etkinleştirilip etkinleştirilmeyeceğini ayarlar (varsayılan: true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | Özel JSON önbellek uygulamasını ayarlar. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | Maksimum disk önbellek boyutunu MB cinsinden ayarlar (varsayılan: 500 MB). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | Bellek önbelleğindeki maksimum giriş sayısını ayarlar (varsayılan: 1000). |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | Bellek önbelleği için TTL'yi dakika cinsinden ayarlar (varsayılan: 60). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonCacheOptions() {#JsonCacheOptions--}
```
public JsonCacheOptions()
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
### getCompressDisk() {#getCompressDisk--}
```
public boolean getCompressDisk()
```


Disk önbelleğinin Gzip kullanılarak sıkıştırılıp sıkıştırılmayacağını alır (varsayılan: true). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


Disk önbellek dizini yolunu alır. Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. Varsayılan: [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


Disk önbelleği için TTL'yi dakika cinsinden alır (varsayılan: 1440). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


Daha hızlı yanıt için JSON önbelleklemenin etkinleştirilip etkinleştirilmeyeceğini alır. Etkinleştirildiğinde, GridJs oluşturulan JSON'ı önbelleğe alır ve sonraki isteklerde yeniden kullanır. Varsayılan değer false'tur. Not: Özel önbellek depolama kullanmak için Implementation'ı ayarlamanız gerekir.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


Disk önbelleğin etkinleştirilip etkinleştirilmeyeceğini alır (varsayılan: true). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


Özel JSON önbellek uygulamasını alır. Ayarlanmamışsa, GridJs varsayılan bellek + disk önbelleğini kullanır.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


Maksimum disk önbellek boyutunu MB cinsinden alır (varsayılan: 500 MB). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


Bellek önbelleğindeki maksimum giriş sayısını alır (varsayılan: 1000). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


Bellek önbelleği için TTL'yi dakika cinsinden alır (varsayılan: 60). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Returns:**
long
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




### setCompressDisk(boolean value) {#setCompressDisk-boolean-}
```
public void setCompressDisk(boolean value)
```


Disk önbelleğinin Gzip kullanılarak sıkıştırılıp sıkıştırılmayacağını ayarlar (varsayılan: true). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


Disk önbellek dizini yolunu ayarlar. Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. Varsayılan: [FileCacheDirectory]/json\_cache

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


Disk önbelleği için TTL'yi dakika cinsinden ayarlar (varsayılan: 1440). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


Daha hızlı yanıt için JSON önbelleklemenin etkinleştirilip etkinleştirilmeyeceğini ayarlar. Etkinleştirildiğinde, GridJs oluşturulan JSON'ı önbelleğe alır ve sonraki isteklerde yeniden kullanır. Varsayılan değer false'tur. Not: Özel önbellek depolama kullanmak için Implementation'ı ayarlamanız gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


Disk önbelleğin etkinleştirilip etkinleştirilmeyeceğini ayarlar (varsayılan: true). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


Özel JSON önbellek uygulamasını ayarlar. Ayarlanmamışsa, GridJs varsayılan bellek + disk önbelleğini kullanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


Maksimum disk önbellek boyutunu MB cinsinden ayarlar (varsayılan: 500 MB). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


Bellek önbelleğindeki maksimum giriş sayısını ayarlar (varsayılan: 1000). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


Bellek önbelleği için TTL'yi dakika cinsinden ayarlar (varsayılan: 60). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | long |  |

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

