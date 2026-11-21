---
title: "SignatureLine"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la línea de firma."
type: docs
url: /es/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

Representa la línea de firma.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         // Create signature line object
         SignatureLine s = new SignatureLine();
         s.setSigner("Simon");
         s.setTitle("Development");
         s.setEmail("simon@aspose.com");
         s.setInstructions("Sign to confirm the excel content.");
 
         // Adds a Signature Line to the worksheet.
         Picture signatureLine = worksheet.getShapes().addSignatureLine(0, 0, s);
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | Indica si se pueden adjuntar comentarios. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | Obtiene el correo electrónico del cantante. |
| [getId()](#getId--) | Obtiene el identificador de esta línea de firma. |
| [getInstructions()](#getInstructions--) | Obtiene el texto mostrado al usuario al firmar. |
| [getProviderId()](#getProviderId--) | Obtiene el id del proveedor de firma. |
| [getShowSignedDate()](#getShowSignedDate--) | Indica si se muestra la fecha de firma. |
| [getSignatureLineType()](#getSignatureLineType--) | Obtiene el tipo de firma. |
| [getSigner()](#getSigner--) | Obtiene el firmante. |
| [getTitle()](#getTitle--) | Obtiene el título del cantante. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | Indica si es una línea de firma. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | Indica si se pueden adjuntar comentarios. |
| [setEmail(String value)](#setEmail-java.lang.String-) | Establece el correo electrónico del cantante. |
| [setId(UUID value)](#setId-java.util.UUID-) | Establece el identificador de esta línea de firma. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | Establece el texto mostrado al usuario al firmar. |
| [setLine(boolean value)](#setLine-boolean-) | Indica si es una línea de firma. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Establece el id del proveedor de firma. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | Indica si se muestra la fecha de firma. |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | Establece el tipo de firma. |
| [setSigner(String value)](#setSigner-java.lang.String-) | Establece el firmante. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Establece el título del cantante. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SignatureLine() {#SignatureLine--}
```
public SignatureLine()
```


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
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


Indica si se pueden adjuntar comentarios.

**Example**

```
         if(s.getAllowComments())
         {
             // Comments could be attached.
         }
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmail() {#getEmail--}
```
public String getEmail()
```


Obtiene el correo electrónico del cantante.

**Example**

```
         // Create signature line object
         SignatureLine s5 = new SignatureLine();
         s5.setEmail("Simon.Zhao@aspose.com");
```

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Obtiene el identificador de esta línea de firma.

**Example**

```
         // Create signature line object
         SignatureLine s1 = new SignatureLine();
         s1.setId(java.util.UUID.randomUUID());
```

**Returns:**
java.util.UUID
### getInstructions() {#getInstructions--}
```
public String getInstructions()
```


Obtiene el texto mostrado al usuario al firmar.

**Example**

```
         // Create signature line object
         SignatureLine s6 = new SignatureLine();
         s6.setInstructions("Just do it.");
```

**Returns:**
java.lang.String
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


Obtiene el id del proveedor de firma.

**Remarks**

Normalmente es el CLSID del complemento COM del proveedor.

**Example**

```
         // Create signature line object
         SignatureLine s2 = new SignatureLine();
         s2.setProviderId(java.util.UUID.fromString("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"));//The GUID should be obtained from the documentation shipped with the provider.
```

**Returns:**
java.util.UUID
### getShowSignedDate() {#getShowSignedDate--}
```
public boolean getShowSignedDate()
```


Indica si se muestra la fecha de firma.

**Example**

```
         if(s.getShowSignedDate())
         {
             //Show signed date.
         }
```

**Returns:**
boolean
### getSignatureLineType() {#getSignatureLineType--}
```
public int getSignatureLineType()
```


Obtiene el tipo de firma. Default - Cuando se establece el valor predeterminado, el valor correspondiente de ProviderId se fija a \{0000000000-0000-0000-0000-0000000000\}. Stamp - Cuando el valor es Stamp, el valor correspondiente de ProviderId suele ser \{000CD6A4-0000-0000-C000-000000000046\}. Custom - Cuando el valor es Custom, el valor correspondiente de ProviderId normalmente debe ser establecido por el usuario. debe obtenerse de la documentación suministrada con el proveedor.

Ver [SignatureType](../../com.aspose.cells/signaturetype).

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


Obtiene el firmante.

**Example**

```
         // Create signature line object
         SignatureLine s3 = new SignatureLine();
         s3.setSigner("Mr xxx");
```

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Obtiene el título del cantante.

**Example**

```
         // Create signature line object
         SignatureLine s4 = new SignatureLine();
         s4.setTitle("Development Lead");
```

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLine() {#isLine--}
```
public boolean isLine()
```


Indica si es una línea de firma.

**Example**

```
         if(s.isLine())
         {
             //Is line.
         }
```

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




### setAllowComments(boolean value) {#setAllowComments-boolean-}
```
public void setAllowComments(boolean value)
```


Indica si se pueden adjuntar comentarios.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


Establece el correo electrónico del cantante.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Establece el identificador de esta línea de firma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


Establece el texto mostrado al usuario al firmar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


Indica si es una línea de firma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Establece el id del proveedor de firma.

**Remarks**

Normalmente es el CLSID del complemento COM del proveedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


Indica si se muestra la fecha de firma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


Establece el tipo de firma. Default - Cuando se establece el valor predeterminado, el valor correspondiente de ProviderId se fija a \{0000000000-0000-0000-0000-0000000000\}. Stamp - Cuando el valor es Stamp, el valor correspondiente de ProviderId suele ser \{000CD6A4-0000-0000-C000-000000000046\}. Custom - Cuando el valor es Custom, el valor correspondiente de ProviderId normalmente debe ser establecido por el usuario. debe obtenerse de la documentación suministrada con el proveedor.

Ver [SignatureType](../../com.aspose.cells/signaturetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


Establece el firmante.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Establece el título del cantante.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

