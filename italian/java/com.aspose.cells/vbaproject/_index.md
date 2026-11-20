---
title: "VbaProject"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il progetto VBA."
type: docs
url: /it/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

Rappresenta il progetto VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | Copia il progetto VBA da un altro file. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | Ottiene i dati grezzi del certificato se questo progetto VBA è firmato. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | Ottiene la codifica del progetto VBA. |
| [getIslockedForViewing()](#getIslockedForViewing--) | Indica se questo progetto VBA è bloccato per la visualizzazione. |
| [getModules()](#getModules--) | Ottiene tutti gli oggetti [VbaModule](../../com.aspose.cells/vbamodule). |
| [getName()](#getName--) | Ottiene il nome del progetto VBA. |
| [getReferences()](#getReferences--) | Ottiene tutti i riferimenti del progetto VBA. |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | Indica se questo progetto VBA è bloccato per la visualizzazione. |
| [isProtected()](#isProtected--) | Indica se questo progetto VBA è protetto. |
| [isSigned()](#isSigned--) | Indica se il codice VBA è firmato o meno. |
| [isValidSigned()](#isValidSigned--) | Indica se la firma del progetto VBA è valida o meno. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | Protegge o rimuove la protezione di questo progetto VBA. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Imposta la codifica del progetto VBA. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome del progetto VBA. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | Firma questo progetto VBA con una DigitalSignature |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Convalida la password di protezione. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


Copia il progetto VBA da un altro file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


Ottiene i dati grezzi del certificato se questo progetto VBA è firmato.

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


Ottiene la codifica del progetto VBA.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


Indica se questo progetto VBA è bloccato per la visualizzazione.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà VbaProject.IsLockedForView. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


Ottiene tutti gli oggetti [VbaModule](../../com.aspose.cells/vbamodule).

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome del progetto VBA.

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


Ottiene tutti i riferimenti del progetto VBA.

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


Indica se questo progetto VBA è bloccato per la visualizzazione. Se vero, il codice non può essere visibile.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indica se questo progetto VBA è protetto.

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


Indica se il codice VBA è firmato o meno.

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


Indica se la firma del progetto VBA è valida o meno.

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


Protegge o rimuove la protezione di questo progetto VBA.

**Remarks**

Se islockedForViewing è vero, la password non può essere nulla.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| islockedForViewing | boolean | indica se il progetto è bloccato per la visualizzazione. |
| password | java.lang.String | Se il valore è nullo, rimuove la protezione di questo progetto VBA, altrimenti protegge questo progetto VBA. |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Imposta la codifica del progetto VBA.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome del progetto VBA.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


Firma questo progetto VBA con una DigitalSignature

**Parameters:**
| Parametro | Tipo | Descrizione |
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


Convalida la password di protezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | java.lang.String | la password |

**Returns:**
boolean - Indica se la password è la password di protezione di questo progetto VBA
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

