---
title: "JsonCacheOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات التكوين لتخزين JSON المؤقت في GridJs."
type: docs
url: /ar/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

خيارات التكوين لتخزين JSON المؤقت في GridJs. يتحكم في سلوك التخزين المؤقت للذاكرة (L1) والقرص (L2).
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | يحصل على ما إذا كان سيتم ضغط التخزين المؤقت للقرص باستخدام Gzip (الافتراضي: true). |
| [getDiskPath()](#getDiskPath--) | يحصل على مسار دليل التخزين المؤقت للقرص. |
| [getDiskTtl()](#getDiskTtl--) | يحصل على قيمة TTL للتخزين المؤقت للقرص، بالدقائق (الافتراضي: 1440). |
| [getEnable()](#getEnable--) | يحصل على ما إذا كان سيتم تمكين تخزين JSON المؤقت لاستجابة أسرع. |
| [getEnableDisk()](#getEnableDisk--) | يحصل على ما إذا كان سيتم تمكين التخزين المؤقت للقرص (الافتراضي: true). |
| [getImplementation()](#getImplementation--) | يحصل على تنفيذ تخزين JSON المؤقت المخصص. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | يحصل على الحد الأقصى لحجم التخزين المؤقت للقرص بالميغابايت (الافتراضي: 500 MB). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | يحصل على الحد الأقصى لعدد الإدخالات في التخزين المؤقت للذاكرة (الافتراضي: 1000). |
| [getMemoryTtl()](#getMemoryTtl--) | يحصل على قيمة TTL للتخزين المؤقت للذاكرة، بالدقائق (الافتراضي: 60). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | يضبط ما إذا كان سيتم ضغط التخزين المؤقت للقرص باستخدام Gzip (الافتراضي: true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | يضبط مسار دليل التخزين المؤقت للقرص. |
| [setDiskTtl(long value)](#setDiskTtl-long-) | يضبط قيمة TTL للتخزين المؤقت للقرص، بالدقائق (الافتراضي: 1440). |
| [setEnable(boolean value)](#setEnable-boolean-) | يضبط ما إذا كان سيتم تمكين تخزين JSON المؤقت لاستجابة أسرع. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | يضبط ما إذا كان سيتم تمكين التخزين المؤقت للقرص (الافتراضي: true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | يضبط تنفيذ ذاكرة التخزين المؤقت JSON المخصص. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | يضبط الحد الأقصى لحجم ذاكرة التخزين المؤقت على القرص بالميغابايت (الافتراضي: 500 ميغابايت). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | يضبط الحد الأقصى لعدد الإدخالات في ذاكرة التخزين المؤقت في الذاكرة (الافتراضي: 1000). |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | يضبط زمن الحياة (TTL) لذاكرة التخزين المؤقت في الذاكرة، بالدقائق (الافتراضي: 60). |
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
| معامل | نوع | الوصف |
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


يحصل على ما إذا كان سيتم ضغط ذاكرة التخزين المؤقت على القرص باستخدام Gzip (الافتراضي: true). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


يحصل على مسار دليل ذاكرة التخزين المؤقت على القرص. يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي. الافتراضي: [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


يحصل على زمن الحياة (TTL) لذاكرة التخزين المؤقت على القرص، بالدقائق (الافتراضي: 1440). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


يحصل على ما إذا كان سيتم تمكين التخزين المؤقت لـ JSON للحصول على استجابة أسرع. عند التمكين، سيقوم GridJs بتخزين JSON المُولد وإعادة استخدامه للطلبات اللاحقة. القيمة الافتراضية هي false. ملاحظة: تحتاج إلى ضبط Implementation لاستخدام تخزين مؤقت مخصص.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


يحصل على ما إذا كان سيتم تمكين التخزين المؤقت على القرص (الافتراضي: true). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


يحصل على تنفيذ التخزين المؤقت JSON المخصص. إذا لم يتم ضبطه، سيستخدم GridJs التخزين المؤقت الافتراضي في الذاكرة + القرص.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


يحصل على الحد الأقصى لحجم التخزين المؤقت على القرص بالميغابايت (الافتراضي: 500 ميغابايت). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


يحصل على الحد الأقصى لعدد الإدخالات في ذاكرة التخزين المؤقت في الذاكرة (الافتراضي: 1000). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


يحصل على زمن الحياة (TTL) لذاكرة التخزين المؤقت في الذاكرة، بالدقائق (الافتراضي: 60). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

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


يضبط ما إذا كان سيتم ضغط التخزين المؤقت على القرص باستخدام Gzip (الافتراضي: true). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


يضبط مسار دليل التخزين المؤقت على القرص. يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي. الافتراضي: [FileCacheDirectory]/json\_cache

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


يضبط زمن الحياة (TTL) للتخزين المؤقت على القرص، بالدقائق (الافتراضي: 1440). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


يضبط ما إذا كان سيتم تمكين التخزين المؤقت لـ JSON للحصول على استجابة أسرع. عند التمكين، سيقوم GridJs بتخزين JSON المُولد وإعادة استخدامه للطلبات اللاحقة. القيمة الافتراضية هي false. ملاحظة: تحتاج إلى ضبط Implementation لاستخدام تخزين مؤقت مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


يضبط ما إذا كان سيتم تمكين التخزين المؤقت على القرص (الافتراضي: true). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


يضبط تنفيذ التخزين المؤقت JSON المخصص. إذا لم يتم ضبطه، سيستخدم GridJs التخزين المؤقت الافتراضي في الذاكرة + القرص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


يضبط الحد الأقصى لحجم التخزين المؤقت على القرص بالميغابايت (الافتراضي: 500 ميغابايت). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


يضبط الحد الأقصى لعدد الإدخالات في ذاكرة التخزين المؤقت في الذاكرة (الافتراضي: 1000). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


يضبط زمن الحياة (TTL) لذاكرة التخزين المؤقت في الذاكرة، بالدقائق (الافتراضي: 60). يصبح ساريًا عندما Enable = true ويُستخدم التخزين المؤقت الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | long |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

