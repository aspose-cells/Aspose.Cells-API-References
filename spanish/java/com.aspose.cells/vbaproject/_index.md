---
title: "VbaProject"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el proyecto VBA."
type: docs
url: /es/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

Representa el proyecto VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | Copiar proyecto VBA de otro archivo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | Obtiene los datos sin procesar del certificado si este proyecto VBA está firmado. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | Obtiene la codificación del proyecto VBA. |
| [getIslockedForViewing()](#getIslockedForViewing--) | Indica si este proyecto VBA está bloqueado para visualización. |
| [getModules()](#getModules--) | Obtiene todos los objetos [VbaModule](../../com.aspose.cells/vbamodule). |
| [getName()](#getName--) | Obtiene el nombre del proyecto VBA. |
| [getReferences()](#getReferences--) | Obtiene todas las referencias del proyecto VBA. |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | Indica si este proyecto VBA está bloqueado para visualización. |
| [isProtected()](#isProtected--) | Indica si este proyecto VBA está protegido. |
| [isSigned()](#isSigned--) | Indica si el código VBA está firmado o no. |
| [isValidSigned()](#isValidSigned--) | Indica si la firma del proyecto VBA es válida o no. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | Protege o desprotege este proyecto VBA. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Establece la codificación del proyecto VBA. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre del proyecto VBA. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | Firma este proyecto VBA con una DigitalSignature |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Valida la contraseña de protección. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


Copiar proyecto VBA de otro archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


Obtiene los datos sin procesar del certificado si este proyecto VBA está firmado.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Obtiene la codificación del proyecto VBA.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


Indica si este proyecto VBA está bloqueado para visualización.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad VbaProject.IsLockedForView. Esta propiedad será eliminada 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


Obtiene todos los objetos [VbaModule](../../com.aspose.cells/vbamodule).

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del proyecto VBA.

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


Obtiene todas las referencias del proyecto VBA.

**Returns:**
[VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLockedForView() {#isLockedForView--}
```
public boolean isLockedForView()
```


Indica si este proyecto VBA está bloqueado para visualización. Si es verdadero, los códigos no podrían ser visibles.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indica si este proyecto VBA está protegido.

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


Indica si el código VBA está firmado o no.

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


Indica si la firma del proyecto VBA es válida o no.

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




### protect(boolean islockedForViewing, String password) {#protect-boolean-java.lang.String-}
```
public void protect(boolean islockedForViewing, String password)
```


Protege o desprotege este proyecto VBA.

**Remarks**

Si islockedForViewing es verdadero, la contraseña no puede ser nula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| islockedForViewing | boolean | indica si bloquea el proyecto para visualización. |
| password | java.lang.String | Si el valor es nulo, desprotege este proyecto VBA, de lo contrario protege este proyecto VBA. |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Establece la codificación del proyecto VBA.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre del proyecto VBA.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


Firma este proyecto VBA con una DigitalSignature

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | DigitalSignature |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### validatePassword(String password) {#validatePassword-java.lang.String-}
```
public boolean validatePassword(String password)
```


Valida la contraseña de protección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| password | java.lang.String | la contraseña |

**Returns:**
booleano - Indica si la contraseña es la contraseña de protección de este proyecto VBA
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

