---
title: "YenidenBağlantıYöntemiTürü"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir."
type: docs
url: /tr/java/com.aspose.cells/reconnectionmethodtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReConnectionMethodType
```

Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [ALWAYS](#ALWAYS) | Her yenilemede, mevcutsa dış bağlantı dosyasından güncellenmiş bağlantı bilgilerini al ve mevcut bağlantı bilgileri yerine kullan. |
| [NEVER](#NEVER) | Dış bağlantı dosyası mevcut olsa ve mevcut bağlantı bilgileri geçersiz olsa bile asla güncellenmiş bağlantı bilgilerini alma. |
| [REQUIRED](#REQUIRED) | Yenilemede mevcut bağlantı bilgilerini kullan ve eğer geçersiz olursa, dış bağlantı dosyasından mevcutsa güncellenmiş bağlantı bilgilerini al. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Her yenilemede, mevcutsa dış bağlantı dosyasından güncellenmiş bağlantı bilgilerini al ve mevcut bağlantı bilgileri yerine kullan. Bu durumda dış bağlantı dosyası mevcut değilse veri yenilemesi başarısız olur.

### NEVER {#NEVER}
```
public static final int NEVER
```


Dış bağlantı dosyası mevcut olsa ve mevcut bağlantı bilgileri geçersiz olsa bile asla güncellenmiş bağlantı bilgilerini alma.

### REQUIRED {#REQUIRED}
```
public static final int REQUIRED
```


Yenilemede mevcut bağlantı bilgilerini kullan ve eğer geçersiz olursa, dış bağlantı dosyasından mevcutsa güncellenmiş bağlantı bilgilerini al.

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

