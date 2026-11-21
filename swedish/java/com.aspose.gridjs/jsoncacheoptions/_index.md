---
title: "JsonCacheOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Konfigurationsalternativ för JSON-cachning i GridJs."
type: docs
url: /sv/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

Konfigurationsalternativ för JSON‑caching i GridJs. Kontrollerar både minnes‑ (L1) och disk‑ (L2) cachebeteende.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | Hämtar om diskcachen ska komprimeras med Gzip (standard: true). |
| [getDiskPath()](#getDiskPath--) | Hämtar sökvägen till diskcache‑katalogen. |
| [getDiskTtl()](#getDiskTtl--) | Hämtar TTL för diskcachen, i minuter (standard: 1440). |
| [getEnable()](#getEnable--) | Hämtar om JSON‑caching ska aktiveras för snabbare svar. |
| [getEnableDisk()](#getEnableDisk--) | Hämtar om diskcache ska aktiveras (standard: true). |
| [getImplementation()](#getImplementation--) | Hämtar den anpassade JSON‑cache‑implementeringen. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | Hämtar maximal storlek för diskcache i MB (standard: 500 MB). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | Hämtar maximalt antal poster i minnescachen (standard: 1000). |
| [getMemoryTtl()](#getMemoryTtl--) | Hämtar TTL för minnescachen, i minuter (standard: 60). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | Ställer in om diskcachen ska komprimeras med Gzip (standard: true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | Ställer in sökvägen för diskcachekatalogen. |
| [setDiskTtl(long value)](#setDiskTtl-long-) | Ställer in TTL för diskcachen, i minuter (standard: 1440). |
| [setEnable(boolean value)](#setEnable-boolean-) | Ställer in om JSON-cachning ska aktiveras för snabbare svar. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | Ställer in om diskcache ska aktiveras (standard: true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | Ställer in den anpassade JSON-cacheimplementeringen. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | Ställer in den maximala storleken för diskcachen i MB (standard: 500 MB). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | Ställer in det maximala antalet poster i minnescachen (standard: 1000). |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | Ställer in TTL för minnescachen, i minuter (standard: 60). |
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
| Parameter | Typ | Beskrivning |
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


Hämtar om diskcachen ska komprimeras med Gzip (standard: true). Påverkar när Enable = true och standardcachen används.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


Hämtar sökvägen för diskcachekatalogen. Påverkar när Enable = true och standardcachen används. Standard: [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


Hämtar TTL för diskcachen, i minuter (standard: 1440). Påverkar när Enable = true och standardcachen används.

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


Hämtar om JSON-cachning ska aktiveras för snabbare svar. När den är aktiverad kommer GridJs att cacha den genererade JSONen och återanvända den för efterföljande förfrågningar. Standardvärdet är false. Obs: Du måste ange Implementation för att använda anpassad cachelagring.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


Hämtar om diskcache ska aktiveras (standard: true). Påverkar när Enable = true och standardcachen används.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


Hämtar den anpassade JSON-cacheimplementeringen. Om den inte är angiven kommer GridJs att använda standardminne + diskcache.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


Hämtar den maximala storleken för diskcachen i MB (standard: 500 MB). Påverkar när Enable = true och standardcachen används.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


Hämtar det maximala antalet poster i minnescachen (standard: 1000). Påverkar när Enable = true och standardcachen används.

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


Hämtar TTL för minnescachen, i minuter (standard: 60). Påverkar när Enable = true och standardcachen används.

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


Ställer in om diskcachen ska komprimeras med Gzip (standard: true). Påverkar när Enable = true och standardcachen används.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


Ställer in sökvägen för diskcachekatalogen. Påverkar när Enable = true och standardcachen används. Standard: [FileCacheDirectory]/json\_cache

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


Ställer in TTL för diskcachen, i minuter (standard: 1440). Påverkar när Enable = true och standardcachen används.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


Ställer in om JSON-cachning ska aktiveras för snabbare svar. När den är aktiverad kommer GridJs att cacha den genererade JSONen och återanvända den för efterföljande förfrågningar. Standardvärdet är false. Obs: Du måste ange Implementation för att använda anpassad cachelagring.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


Ställer in om diskcache ska aktiveras (standard: true). Påverkar när Enable = true och standardcachen används.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


Ställer in den anpassade JSON-cacheimplementeringen. Om den inte är angiven kommer GridJs att använda standardminne + diskcache.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


Ställer in den maximala storleken för diskcachen i MB (standard: 500 MB). Påverkar när Enable = true och standardcachen används.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


Ställer in det maximala antalet poster i minnescachen (standard: 1000). Påverkar när Enable = true och standardcachen används.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


Ställer in TTL för minnescache, i minuter (standard: 60). Träder i kraft när Enable = true och standardcachen används.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | long |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

