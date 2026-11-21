---
title: "DigitalSignature"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Firma en el archivo."
type: docs
url: /es/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

Firma en el archivo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | Constructor de digitalSignature. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | Objeto de certificado que se utilizó para firmar el documento. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | El propósito de la firma. |
| [getId()](#getId--) | Especifica un GUID que puede cruzarse con el GUID de la línea de firma almacenada en el contenido del documento. |
| [getImage()](#getImage--) | Especifica una imagen para la firma digital. |
| [getProviderId()](#getProviderId--) | Especifica el ID de clase del proveedor de firma. |
| [getSignTime()](#getSignTime--) | El momento en que el documento fue firmado. |
| [getText()](#getText--) | Especifica el texto de la firma real en la firma digital. |
| [getXAdESType()](#getXAdESType--) | Tipo XAdES. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | Si esta firma digital es válida y el documento no ha sido manipulado, este valor será true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | Objeto de certificado que se utilizó para firmar el documento. |
| [setComments(String value)](#setComments-java.lang.String-) | El propósito de la firma. |
| [setId(UUID value)](#setId-java.util.UUID-) | Especifica un GUID que puede cruzarse con el GUID de la línea de firma almacenada en el contenido del documento. |
| [setImage(byte[] value)](#setImage-byte---) | Especifica una imagen para la firma digital. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Especifica el ID de clase del proveedor de firma. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | El momento en que el documento fue firmado. |
| [setText(String value)](#setText-java.lang.String-) | Especifica el texto de la firma real en la firma digital. |
| [setXAdESType(int value)](#setXAdESType-int-) | Tipo XAdES. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


Constructor de digitalSignature.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| certificate | java.security.KeyStore | Objeto de certificado que se utilizó para firmar el documento. |
| privateKeyPassword | java.lang.String | La contraseña de la clave privada. |
| comentarios | java.lang.String | El propósito de la firma. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | La hora UTC cuando se firmó el documento. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


Objeto de certificado que se utilizó para firmar el documento.

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


El propósito de la firma.

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Especifica un GUID que puede cruzarse con el GUID de la línea de firma almacenada en el contenido del documento. El valor predeterminado es Empty (todos ceros) Guid.

**Remarks**

Cuando se establece, asocia [SignatureLine](../../com.aspose.cells/signatureline) con la correspondiente [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


Especifica una imagen para la firma digital. El valor predeterminado es null.

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


Especifica el ID de clase del proveedor de firma. El valor predeterminado es Empty (todos ceros) Guid.

**Remarks**

El proveedor de servicios criptográficos (CSP) es un módulo de software independiente que realmente ejecuta algoritmos criptográficos para autenticación, codificación y cifrado. Microsoft Office reserva el valor de \{00000000-0000-0000-0000-000000000000\} para su proveedor de firma predeterminado, y \{000CD6A4-0000-0000-C000-000000000046\} para su proveedor de firma de Asia Oriental. El GUID del proveedor adicionalmente instalado debe obtenerse de la documentación suministrada con el proveedor.

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


El momento en que el documento fue firmado.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


Especifica el texto de la firma real en la firma digital. El valor predeterminado es Empty.

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


Tipo XAdES. El valor predeterminado es None (XAdES está desactivado).

Ver [XAdESType](../../com.aspose.cells/xadestype).

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


Si esta firma digital es válida y el documento no ha sido manipulado, este valor será true.

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


Objeto de certificado que se utilizó para firmar el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


El propósito de la firma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Especifica un GUID que puede cruzarse con el GUID de la línea de firma almacenada en el contenido del documento. El valor predeterminado es Empty (todos ceros) Guid.

**Remarks**

Cuando se establece, asocia [SignatureLine](../../com.aspose.cells/signatureline) con la correspondiente [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


Especifica una imagen para la firma digital. El valor predeterminado es null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Especifica el ID de clase del proveedor de firma. El valor predeterminado es Empty (todos ceros) Guid.

**Remarks**

El proveedor de servicios criptográficos (CSP) es un módulo de software independiente que realmente ejecuta algoritmos criptográficos para autenticación, codificación y cifrado. Microsoft Office reserva el valor de \{00000000-0000-0000-0000-000000000000\} para su proveedor de firma predeterminado, y \{000CD6A4-0000-0000-C000-000000000046\} para su proveedor de firma de Asia Oriental. El GUID del proveedor adicionalmente instalado debe obtenerse de la documentación suministrada con el proveedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


El momento en que el documento fue firmado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Especifica el texto de la firma real en la firma digital. El valor predeterminado es Empty.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


Tipo XAdES. El valor predeterminado es None (XAdES está desactivado).

Ver [XAdESType](../../com.aspose.cells/xadestype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

