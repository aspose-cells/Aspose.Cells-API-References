---
title: "GridCacheForStream"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bu sınıf GridJs için önbellek işlemlerini içerir."
type: docs
url: /tr/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

Bu sınıf, GridJs için önbellek işlemlerini içerir. Kullanıcı, buna dayanarak depolama için kendi iş mantığını uygulamalıdır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | Bu yöntemi, dosya URL'sini önbellekten alacak şekilde uygulayın. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | uid'ye sahip önbelleğin var olup olmadığını kontrol eder |
| [loadStream(String uid)](#loadStream-java.lang.String-) | Bu yöntemi, uid anahtarıyla önbelleği yükleyecek ve önbellekten akışı döndürecek şekilde uygulayın. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | Bu yöntemi, önbelleği kaydedecek ve akışı uid anahtarıyla önbelleğe kaydedecek şekilde uygulayın. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridCacheForStream() {#GridCacheForStream--}
```
public GridCacheForStream()
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
### getFileUrl(String uid) {#getFileUrl-java.lang.String-}
```
public abstract String getFileUrl(String uid)
```


Bu yöntemi, dosya URL'sini önbellekten alacak şekilde uygulayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.String - Dosyanın URL'si
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExisted(String uid) {#isExisted-java.lang.String-}
```
public abstract boolean isExisted(String uid)
```


uid'ye sahip önbelleğin var olup olmadığını kontrol eder

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
boolean - Boolean değeri
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


Bu yöntemi, uid anahtarıyla önbelleği yükleyecek ve önbellekten akışı döndürecek şekilde uygulayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
java.io.InputStream
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveStream(InputStream s, String uid) {#saveStream-java.io.InputStream-java.lang.String-}
```
public abstract void saveStream(InputStream s, String uid)
```


Bu yöntemi, önbelleği kaydedecek ve akışı uid anahtarıyla önbelleğe kaydedecek şekilde uygulayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| s | java.io.InputStream |  |
| uid | java.lang.String |  |

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

