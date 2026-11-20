---
title: "DigitalSignature"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Signatur in Datei."
type: docs
url: /de/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

Signatur in Datei.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | Konstruktor von digitalSignature. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Der Zweck der Signatur. |
| [getId()](#getId--) | Gibt eine GUID an, die mit der GUID der Signaturzeile, die im Dokumentinhalt gespeichert ist, abgeglichen werden kann. |
| [getImage()](#getImage--) | Gibt ein Bild für die digitale Signatur an. |
| [getProviderId()](#getProviderId--) | Gibt die Klassen-ID des Signaturanbieters an. |
| [getSignTime()](#getSignTime--) | Der Zeitpunkt, zu dem das Dokument signiert wurde. |
| [getText()](#getText--) | Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. |
| [getXAdESType()](#getXAdESType--) | XAdES‑Typ. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | Wenn diese digitale Signatur gültig ist und das Dokument nicht manipuliert wurde, ist dieser Wert true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde. |
| [setComments(String value)](#setComments-java.lang.String-) | Der Zweck der Signatur. |
| [setId(UUID value)](#setId-java.util.UUID-) | Gibt eine GUID an, die mit der GUID der Signaturzeile, die im Dokumentinhalt gespeichert ist, abgeglichen werden kann. |
| [setImage(byte[] value)](#setImage-byte---) | Gibt ein Bild für die digitale Signatur an. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Gibt die Klassen-ID des Signaturanbieters an. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | Der Zeitpunkt, zu dem das Dokument signiert wurde. |
| [setText(String value)](#setText-java.lang.String-) | Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. |
| [setXAdESType(int value)](#setXAdESType-int-) | XAdES‑Typ. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


Konstruktor von digitalSignature.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zertifikat | java.security.KeyStore | Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde. |
| privateKeyPassword | java.lang.String | Das Passwort für den privaten Schlüssel. |
| Kommentare | java.lang.String | Der Zweck der Signatur. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | Die UTC-Zeit, zu der das Dokument signiert wurde. |

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
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde.

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


Der Zweck der Signatur.

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Gibt eine GUID an, die mit der GUID der Signaturzeile, die im Dokumentinhalt gespeichert ist, abgeglichen werden kann. Standardwert ist Empty (alle Nullen) Guid.

**Remarks**

Wenn gesetzt, verknüpft es [SignatureLine](../../com.aspose.cells/signatureline) mit der entsprechenden [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


Gibt ein Bild für die digitale Signatur an. Standardwert ist null.

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


Gibt die Klassen-ID des Signaturanbieters an. Standardwert ist Empty (alle Nullen) Guid.

**Remarks**

Der kryptografische Dienstanbieter (CSP) ist ein unabhängiges Softwaremodul, das tatsächlich kryptografische Algorithmen für Authentifizierung, Codierung und Verschlüsselung ausführt. Microsoft Office reserviert den Wert \{00000000-0000-0000-0000-000000000000\} für seinen Standard‑Signaturanbieter und \{000CD6A4-0000-0000-C000-000000000046\} für seinen ostasiatischen Signaturanbieter. Die GUID des zusätzlich installierten Anbieters sollte aus der mit dem Anbieter gelieferten Dokumentation entnommen werden.

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


Der Zeitpunkt, zu dem das Dokument signiert wurde.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. Standardwert ist Empty.

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


XAdES-Typ. Standardwert ist None (XAdES ist deaktiviert).

Siehe [XAdESType](../../com.aspose.cells/xadestype).

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


Wenn diese digitale Signatur gültig ist und das Dokument nicht manipuliert wurde, ist dieser Wert true.

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


Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Der Zweck der Signatur.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Gibt eine GUID an, die mit der GUID der Signaturzeile, die im Dokumentinhalt gespeichert ist, abgeglichen werden kann. Standardwert ist Empty (alle Nullen) Guid.

**Remarks**

Wenn gesetzt, verknüpft es [SignatureLine](../../com.aspose.cells/signatureline) mit der entsprechenden [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


Gibt ein Bild für die digitale Signatur an. Standardwert ist null.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Gibt die Klassen-ID des Signaturanbieters an. Standardwert ist Empty (alle Nullen) Guid.

**Remarks**

Der kryptografische Dienstanbieter (CSP) ist ein unabhängiges Softwaremodul, das tatsächlich kryptografische Algorithmen für Authentifizierung, Codierung und Verschlüsselung ausführt. Microsoft Office reserviert den Wert \{00000000-0000-0000-0000-000000000000\} für seinen Standard‑Signaturanbieter und \{000CD6A4-0000-0000-C000-000000000046\} für seinen ostasiatischen Signaturanbieter. Die GUID des zusätzlich installierten Anbieters sollte aus der mit dem Anbieter gelieferten Dokumentation entnommen werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


Der Zeitpunkt, zu dem das Dokument signiert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. Standardwert ist Empty.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


XAdES-Typ. Standardwert ist None (XAdES ist deaktiviert).

Siehe [XAdESType](../../com.aspose.cells/xadestype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

