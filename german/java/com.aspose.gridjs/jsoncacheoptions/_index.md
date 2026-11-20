---
title: "JsonCacheOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Konfigurationsoptionen für JSON‑Caching in GridJs."
type: docs
url: /de/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

Konfigurationsoptionen für das JSON‑Caching in GridJs. Steuert sowohl das Speicher‑ (L1) als auch das Festplatten‑ (L2) Cache‑Verhalten.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | Ermittelt, ob der Festplatten‑Cache mit Gzip komprimiert wird (Standard: true). |
| [getDiskPath()](#getDiskPath--) | Ermittelt den Pfad des Festplatten‑Cache‑Verzeichnisses. |
| [getDiskTtl()](#getDiskTtl--) | Ermittelt die TTL für den Festplatten‑Cache in Minuten (Standard: 1440). |
| [getEnable()](#getEnable--) | Ermittelt, ob JSON-Caching für schnellere Antworten aktiviert werden soll. |
| [getEnableDisk()](#getEnableDisk--) | Ermittelt, ob der Festplatten-Cache aktiviert ist (Standard: true). |
| [getImplementation()](#getImplementation--) | Ermittelt die benutzerdefinierte JSON-Cache-Implementierung. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | Ermittelt die maximale Größe des Festplatten-Caches in MB (Standard: 500 MB). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | Ermittelt die maximale Anzahl von Einträgen im Speicher-Cache (Standard: 1000). |
| [getMemoryTtl()](#getMemoryTtl--) | Ermittelt die TTL für den Speicher-Cache in Minuten (Standard: 60). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | Legt fest, ob der Festplatten-Cache mit Gzip komprimiert werden soll (Standard: true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | Legt den Pfad des Festplatten-Cache-Verzeichnisses fest. |
| [setDiskTtl(long value)](#setDiskTtl-long-) | Legt die TTL für den Festplatten-Cache in Minuten fest (Standard: 1440). |
| [setEnable(boolean value)](#setEnable-boolean-) | Legt fest, ob JSON-Caching für schnellere Antworten aktiviert werden soll. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | Legt fest, ob der Festplatten-Cache aktiviert werden soll (Standard: true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | Legt die benutzerdefinierte JSON-Cache-Implementierung fest. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | Legt die maximale Größe des Festplatten-Caches in MB fest (Standard: 500 MB). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | Legt die maximale Anzahl von Einträgen im Speicher-Cache fest (Standard: 1000). |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | Legt die TTL für den Speicher-Cache in Minuten fest (Standard: 60). |
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
| Parameter | Typ | Beschreibung |
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


Ermittelt, ob der Festplatten-Cache mit Gzip komprimiert werden soll (Standard: true). Wirkt nur, wenn Enable = true und der Standard-Cache verwendet wird.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


Ermittelt den Pfad des Festplatten-Cache-Verzeichnisses. Wirkt nur, wenn Enable = true und der Standard-Cache verwendet wird. Standard: [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


Ermittelt die TTL für den Festplatten-Cache in Minuten (Standard: 1440). Wirkt nur, wenn Enable = true und der Standard-Cache verwendet wird.

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


Ermittelt, ob JSON-Caching für schnellere Antworten aktiviert ist. Wenn aktiviert, cached GridJs das erzeugte JSON und verwendet es bei nachfolgenden Anfragen erneut. Der Standardwert ist false. Hinweis: Sie müssen Implementation setzen, um benutzerdefinierten Cache-Speicher zu verwenden.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


Ermittelt, ob der Festplatten-Cache aktiviert ist (Standard: true). Wirkt nur, wenn Enable = true und der Standard-Cache verwendet wird.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


Ermittelt die benutzerdefinierte JSON-Cache-Implementierung. Wenn nicht gesetzt, verwendet GridJs den Standard‑Speicher‑+‑Festplatten‑Cache.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


Ermittelt die maximale Größe des Festplatten-Caches in MB (Standard: 500 MB). Wirkt nur, wenn Enable = true und der Standard-Cache verwendet wird.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


Ermittelt die maximale Anzahl von Einträgen im Speicher-Cache (Standard: 1000). Wirkt nur, wenn Enable = true und der Standard-Cache verwendet wird.

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


Ermittelt die TTL für den Speicher-Cache in Minuten (Standard: 60). Wirkt nur, wenn Enable = true und der Standard-Cache verwendet wird.

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


Legt fest, ob der Festplatten-Cache mit Gzip komprimiert werden soll (Standard: true). Wirkt nur, wenn Enable = true und der Standard-Cache verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


Legt den Pfad des Festplatten-Cache-Verzeichnisses fest. Wirkt, wenn Enable = true und der Standard-Cache verwendet wird. Standard: [FileCacheDirectory]/json\_cache

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


Legt die TTL für den Festplatten-Cache in Minuten fest (Standard: 1440). Wirkt, wenn Enable = true und der Standard-Cache verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


Legt fest, ob JSON-Caching für schnellere Antworten aktiviert werden soll. Wenn aktiviert, cached GridJs das erzeugte JSON und verwendet es für nachfolgende Anfragen erneut. Der Standardwert ist false. Hinweis: Sie müssen Implementation festlegen, um benutzerdefinierten Cache-Speicher zu verwenden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


Legt fest, ob der Festplatten-Cache aktiviert werden soll (Standard: true). Wirkt, wenn Enable = true und der Standard-Cache verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


Legt die benutzerdefinierte JSON-Cache-Implementierung fest. Wenn nicht gesetzt, verwendet GridJs den Standard‑Memory‑+‑Disk‑Cache.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


Legt die maximale Größe des Festplatten-Caches in MB fest (Standard: 500 MB). Wirkt, wenn Enable = true und der Standard-Cache verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


Legt die maximale Anzahl von Einträgen im Speicher-Cache fest (Standard: 1000). Wirkt, wenn Enable = true und der Standard-Cache verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


Legt die TTL für den Speicher-Cache in Minuten fest (Standard: 60). Wirkt, wenn Enable = true und der Standard-Cache verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | long |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

