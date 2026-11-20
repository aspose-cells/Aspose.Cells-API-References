---
title: "DigitalSignature"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Firma nel file."
type: docs
url: /it/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

Firma nel file.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | Costruttore di digitalSignature. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | Oggetto certificato utilizzato per firmare il documento. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Lo scopo della firma. |
| [getId()](#getId--) | Specifica un GUID che può essere incrociato con il GUID della linea di firma memorizzata nel contenuto del documento. |
| [getImage()](#getImage--) | Specifica un'immagine per la firma digitale. |
| [getProviderId()](#getProviderId--) | Specifica l'ID della classe del provider di firma. |
| [getSignTime()](#getSignTime--) | Il momento in cui il documento è stato firmato. |
| [getText()](#getText--) | Specifica il testo della firma effettiva nella firma digitale. |
| [getXAdESType()](#getXAdESType--) | Tipo XAdES. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | Se questa firma digitale è valida e il documento non è stato manomesso, questo valore sarà true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | Oggetto certificato utilizzato per firmare il documento. |
| [setComments(String value)](#setComments-java.lang.String-) | Lo scopo della firma. |
| [setId(UUID value)](#setId-java.util.UUID-) | Specifica un GUID che può essere incrociato con il GUID della linea di firma memorizzata nel contenuto del documento. |
| [setImage(byte[] value)](#setImage-byte---) | Specifica un'immagine per la firma digitale. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Specifica l'ID della classe del provider di firma. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | Il momento in cui il documento è stato firmato. |
| [setText(String value)](#setText-java.lang.String-) | Specifica il testo della firma effettiva nella firma digitale. |
| [setXAdESType(int value)](#setXAdESType-int-) | Tipo XAdES. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


Costruttore di digitalSignature.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| certificate | java.security.KeyStore | Oggetto certificato utilizzato per firmare il documento. |
| privateKeyPassword | java.lang.String | La password per la chiave privata. |
| commenti | java.lang.String | Lo scopo della firma. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | L'ora UTC in cui il documento è stato firmato. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


Oggetto certificato utilizzato per firmare il documento.

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


Lo scopo della firma.

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Specifica un GUID che può essere incrociato con il GUID della linea di firma memorizzata nel contenuto del documento. Il valore predefinito è Empty (tutti zero) Guid.

**Remarks**

Quando impostato, associa [SignatureLine](../../com.aspose.cells/signatureline) alla corrispondente [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


Specifica un'immagine per la firma digitale. Il valore predefinito è null.

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


Specifica l'ID classe del provider di firma. Il valore predefinito è Empty (tutti zero) Guid.

**Remarks**

Il provider di servizi crittografici (CSP) è un modulo software indipendente che esegue effettivamente gli algoritmi di crittografia per l'autenticazione, la codifica e la cifratura. Microsoft Office riserva il valore \{00000000-0000-0000-0000-000000000000\} per il suo provider di firma predefinito, e \{000CD6A4-0000-0000-C000-000000000046\} per il suo provider di firma per lingue dell'Est asiatico. Il GUID del provider aggiuntivamente installato deve essere ottenuto dalla documentazione fornita con il provider.

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


Il momento in cui il documento è stato firmato.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


Specifica il testo della firma reale nella firma digitale. Il valore predefinito è Empty.

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


Tipo XAdES. Il valore predefinito è None (XAdES è disattivato).

Vedi [XAdESType](../../com.aspose.cells/xadestype).

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


Se questa firma digitale è valida e il documento non è stato manomesso, questo valore sarà true.

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


Oggetto certificato utilizzato per firmare il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Lo scopo della firma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Specifica un GUID che può essere incrociato con il GUID della linea di firma memorizzata nel contenuto del documento. Il valore predefinito è Empty (tutti zero) Guid.

**Remarks**

Quando impostato, associa [SignatureLine](../../com.aspose.cells/signatureline) alla corrispondente [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


Specifica un'immagine per la firma digitale. Il valore predefinito è null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Specifica l'ID classe del provider di firma. Il valore predefinito è Empty (tutti zero) Guid.

**Remarks**

Il provider di servizi crittografici (CSP) è un modulo software indipendente che esegue effettivamente gli algoritmi di crittografia per l'autenticazione, la codifica e la cifratura. Microsoft Office riserva il valore \{00000000-0000-0000-0000-000000000000\} per il suo provider di firma predefinito, e \{000CD6A4-0000-0000-C000-000000000046\} per il suo provider di firma per lingue dell'Est asiatico. Il GUID del provider aggiuntivamente installato deve essere ottenuto dalla documentazione fornita con il provider.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


Il momento in cui il documento è stato firmato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Specifica il testo della firma reale nella firma digitale. Il valore predefinito è Empty.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


Tipo XAdES. Il valore predefinito è None (XAdES è disattivato).

Vedi [XAdESType](../../com.aspose.cells/xadestype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

