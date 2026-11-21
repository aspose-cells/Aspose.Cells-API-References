---
title: "DigitalSignature"
second_title: "Aspose.Cells for Java API Referansı"
description: "Dosyadaki imza."
type: docs
url: /tr/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

Dosyadaki imza.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | digitalSignature'ın yapıcı metodu. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | Belgeyi imzalamak için kullanılan sertifika nesnesi. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | İmzalamanın amacı. |
| [getId()](#getId--) | Belge içeriğinde depolanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. |
| [getImage()](#getImage--) | Dijital imza için bir görüntü belirtir. |
| [getProviderId()](#getProviderId--) | İmza sağlayıcısının sınıf kimliğini (class ID) belirtir. |
| [getSignTime()](#getSignTime--) | Belgenin imzalandığı zaman. |
| [getText()](#getText--) | Dijital imzada gerçek imzanın metnini belirtir. |
| [getXAdESType()](#getXAdESType--) | XAdES türü. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | Bu dijital imza geçerli ve belge değiştirilmemişse, bu değer true olacaktır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | Belgeyi imzalamak için kullanılan sertifika nesnesi. |
| [setComments(String value)](#setComments-java.lang.String-) | İmzalamanın amacı. |
| [setId(UUID value)](#setId-java.util.UUID-) | Belge içeriğinde depolanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. |
| [setImage(byte[] value)](#setImage-byte---) | Dijital imza için bir görüntü belirtir. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | İmza sağlayıcısının sınıf kimliğini (class ID) belirtir. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | Belgenin imzalandığı zaman. |
| [setText(String value)](#setText-java.lang.String-) | Dijital imzada gerçek imzanın metnini belirtir. |
| [setXAdESType(int value)](#setXAdESType-int-) | XAdES türü. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


digitalSignature'ın yapıcı metodu.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| certificate | java.security.KeyStore | Belgeyi imzalamak için kullanılan sertifika nesnesi. |
| privateKeyPassword | java.lang.String | Özel anahtarın şifresi. |
| yorumlar | java.lang.String | İmzalamanın amacı. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | Belgenin imzalandığı utc zamanı. |

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
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


Belgeyi imzalamak için kullanılan sertifika nesnesi.

**Returns:**
java.security.KeyStore
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


İmzalamanın amacı.

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Belge içeriğinde depolanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir.

**Remarks**

Ayarlandığında, [SignatureLine](../../com.aspose.cells/signatureline) öğesini ilgili [DigitalSignature](../../com.aspose.cells/digitalsignature) ile ilişkilendirir.

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


Dijital imza için bir görüntü belirtir. Varsayılan değer null'dur.

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


İmza sağlayıcısının sınıf kimliğini (class ID) belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir.

**Remarks**

Kriptografik hizmet sağlayıcı (CSP), kimlik doğrulama, kodlama ve şifreleme için kriptografi algoritmalarını gerçekte yürüten bağımsız bir yazılım modülüdür. Microsoft Office, varsayılan imza sağlayıcısı için \{00000000-0000-0000-0000-000000000000\} değerini ve Doğu Asya imza sağlayıcısı için \{000CD6A4-0000-0000-C000-000000000046\} değerini ayırır. Ek olarak kurulan sağlayıcının GUID'i, sağlayıcıyla birlikte gelen belgelerden elde edilmelidir.

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


Belgenin imzalandığı zaman.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


Dijital imzada gerçek imzanın metnini belirtir. Varsayılan değer Boş'tur.

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


XAdES türü. Varsayılan değer Yok (XAdES kapalı).

Bkz. [XAdESType](../../com.aspose.cells/xadestype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isValid() {#isValid--}
```
public boolean isValid()
```


Bu dijital imza geçerli ve belge değiştirilmemişse, bu değer true olacaktır.

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




### setCertificate(KeyStore value) {#setCertificate-java.security.KeyStore-}
```
public void setCertificate(KeyStore value)
```


Belgeyi imzalamak için kullanılan sertifika nesnesi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


İmzalamanın amacı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Belge içeriğinde depolanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir.

**Remarks**

Ayarlandığında, [SignatureLine](../../com.aspose.cells/signatureline) öğesini ilgili [DigitalSignature](../../com.aspose.cells/digitalsignature) ile ilişkilendirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


Dijital imza için bir görüntü belirtir. Varsayılan değer null'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


İmza sağlayıcısının sınıf kimliğini (class ID) belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir.

**Remarks**

Kriptografik hizmet sağlayıcı (CSP), kimlik doğrulama, kodlama ve şifreleme için kriptografi algoritmalarını gerçekte yürüten bağımsız bir yazılım modülüdür. Microsoft Office, varsayılan imza sağlayıcısı için \{00000000-0000-0000-0000-000000000000\} değerini ve Doğu Asya imza sağlayıcısı için \{000CD6A4-0000-0000-C000-000000000046\} değerini ayırır. Ek olarak kurulan sağlayıcının GUID'i, sağlayıcıyla birlikte gelen belgelerden elde edilmelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


Belgenin imzalandığı zaman.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Dijital imzada gerçek imzanın metnini belirtir. Varsayılan değer Boş'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


XAdES türü. Varsayılan değer Yok (XAdES kapalı).

Bkz. [XAdESType](../../com.aspose.cells/xadestype).

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

