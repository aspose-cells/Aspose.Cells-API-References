---
title: "DigitalSignature"
second_title: "Aspose.Cells för Java API-referens"
description: "Signatur i fil."
type: docs
url: /sv/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

Signatur i fil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | Konstruktor för digitalSignature. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | Certifikatobjekt som användes för att signera dokumentet. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Syftet med signaturen. |
| [getId()](#getId--) | Anger en GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. |
| [getImage()](#getImage--) | Anger en bild för den digitala signaturen. |
| [getProviderId()](#getProviderId--) | Anger klass-ID för signaturleverantören. |
| [getSignTime()](#getSignTime--) | Tidpunkten då dokumentet signerades. |
| [getText()](#getText--) | Anger texten för den faktiska signaturen i den digitala signaturen. |
| [getXAdESType()](#getXAdESType--) | XAdES-typ. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | Om denna digitala signatur är giltig och dokumentet inte har manipulerats, kommer detta värde att vara true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | Certifikatobjekt som användes för att signera dokumentet. |
| [setComments(String value)](#setComments-java.lang.String-) | Syftet med signaturen. |
| [setId(UUID value)](#setId-java.util.UUID-) | Anger en GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. |
| [setImage(byte[] value)](#setImage-byte---) | Anger en bild för den digitala signaturen. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Anger klass-ID för signaturleverantören. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | Tidpunkten då dokumentet signerades. |
| [setText(String value)](#setText-java.lang.String-) | Anger texten för den faktiska signaturen i den digitala signaturen. |
| [setXAdESType(int value)](#setXAdESType-int-) | XAdES-typ. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


Konstruktor för digitalSignature.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| certifikat | java.security.KeyStore | Certifikatobjekt som användes för att signera dokumentet. |
| privateKeyPassword | java.lang.String | Lösenordet för den privata nyckeln. |
| kommentarer | java.lang.String | Syftet med signaturen. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | UTC-tiden då dokumentet signerades. |

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
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


Certifikatobjekt som användes för att signera dokumentet.

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


Syftet med signaturen.

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Anger en GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. Standardvärdet är Empty (alla nollor) Guid.

**Remarks**

När den är inställd associerar den [SignatureLine](../../com.aspose.cells/signatureline) med motsvarande [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


Anger en bild för den digitala signaturen. Standardvärdet är null.

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


Anger klass-ID för signaturleverantören. Standardvärdet är Empty (alla nollor) Guid.

**Remarks**

Den kryptografiska tjänsteleverantören (CSP) är en oberoende programmodul som faktiskt utför kryptografialgoritmer för autentisering, kodning och kryptering. Microsoft Office reserverar värdet \{00000000-0000-0000-0000-000000000000\} för sin standardsignaturleverantör, och \{000CD6A4-0000-0000-C000-000000000046\} för sin östasiatiska signaturleverantör. GUID för den ytterligare installerade leverantören bör hämtas från dokumentationen som levereras med leverantören.

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


Tidpunkten då dokumentet signerades.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


Anger texten för den faktiska signaturen i den digitala signaturen. Standardvärdet är Empty.

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


XAdES-typ. Standardvärdet är None (XAdES är avstängt).

Se [XAdESType](../../com.aspose.cells/xadestype).

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


Om denna digitala signatur är giltig och dokumentet inte har manipulerats, kommer detta värde att vara true.

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


Certifikatobjekt som användes för att signera dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Syftet med signaturen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Anger en GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. Standardvärdet är Empty (alla nollor) Guid.

**Remarks**

När den är inställd associerar den [SignatureLine](../../com.aspose.cells/signatureline) med motsvarande [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


Anger en bild för den digitala signaturen. Standardvärdet är null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Anger klass-ID för signaturleverantören. Standardvärdet är Empty (alla nollor) Guid.

**Remarks**

Den kryptografiska tjänsteleverantören (CSP) är en oberoende programmodul som faktiskt utför kryptografialgoritmer för autentisering, kodning och kryptering. Microsoft Office reserverar värdet \{00000000-0000-0000-0000-000000000000\} för sin standardsignaturleverantör, och \{000CD6A4-0000-0000-C000-000000000046\} för sin östasiatiska signaturleverantör. GUID för den ytterligare installerade leverantören bör hämtas från dokumentationen som levereras med leverantören.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


Tidpunkten då dokumentet signerades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Anger texten för den faktiska signaturen i den digitala signaturen. Standardvärdet är Empty.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


XAdES-typ. Standardvärdet är None (XAdES är avstängt).

Se [XAdESType](../../com.aspose.cells/xadestype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

