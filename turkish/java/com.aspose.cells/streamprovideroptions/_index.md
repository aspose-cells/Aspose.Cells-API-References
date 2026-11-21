---
title: "StreamProviderOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Akış seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

Akış seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | Yeni bir [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) sınıfı örneği başlatır. |
| [StreamProviderOptions()](#StreamProviderOptions--) | Yeni bir [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | Referans alınan kaynak için oluşturulan html dosyasında kaydedilen kullanıcı özel yolu (URL). |
| [getDefaultPath()](#getDefaultPath--) | Referans alınan kaynak için oluşturulan html dosyasında kaydedilen varsayılan yol (URL). |
| [getInputStream()](#getInputStream--) | Veri almak için giriş akışını alır. |
| [getResourceLoadingType()](#getResourceLoadingType--) | Yükleme kaynağının tipini alır. |
| [getStream()](#getStream--) | Kaydedilen veriyi yazmak için çıkış akışını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | Referans alınan kaynak için oluşturulan html dosyasında kaydedilen kullanıcı özel yolu (URL). |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | Veri almak için giriş akışını ayarlar. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | Yükleme kaynağının tipini ayarlar. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Kaydedilen veriyi yazmak için çıkış akışını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


Yeni bir [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). Bağlantılı kaynağı yüklemek için tip. |
| defaultPath | java.lang.String | Varsayılan yol. |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


Yeni bir [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) sınıfı örneği başlatır.

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
### getCustomPath() {#getCustomPath--}
```
public String getCustomPath()
```


Referans alınan kaynak için oluşturulan html dosyasında kaydedilen kullanıcı özel yolu (URL). Kullanıcı tarafından tanımlanmazsa, DefaultPath kullanılacaktır. Örneğin, sayfa verileri kullanıcı tarafından d:/sheet001.htm konumuna kaydedildiğinde, ana html dosyasında kullanılan url \"d:/sheet001.htm\" olmalı veya ana html dosyası tarafından erişilebilecek başka geçerli bir göreli yol olmalıdır.

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


Referans alınan kaynak için oluşturulan html dosyasında kaydedilen varsayılan yol (URL). Örneğin, sayfa verileri xxx\\_files/sheet001.htm içinde kaydedildiğinde, ana html dosyasında kullanılan url \"src=\\\"xxx\\_files/sheet001.htm\\\"\" şeklinde olmalıdır.

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


Veri almak için giriş akışını alır.

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


Yükleme kaynağının tipini alır.

Bakınız [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


Kaydedilen veriyi yazmak için çıkış akışını alır.

**Returns:**
java.io.OutputStream
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




### setCustomPath(String value) {#setCustomPath-java.lang.String-}
```
public void setCustomPath(String value)
```


Referans alınan kaynak için oluşturulan html dosyasında kaydedilen kullanıcı özel yolu (URL). Kullanıcı tarafından tanımlanmazsa, DefaultPath kullanılacaktır. Örneğin, sayfa verileri kullanıcı tarafından d:/sheet001.htm konumuna kaydedildiğinde, ana html dosyasında kullanılan url \"d:/sheet001.htm\" olmalı veya ana html dosyası tarafından erişilebilecek başka geçerli bir göreli yol olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


Veri almak için giriş akışını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


Yükleme kaynağının tipini ayarlar.

Bakınız [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


Kaydedilen veriyi yazmak için çıkış akışını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.io.OutputStream |  |

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

