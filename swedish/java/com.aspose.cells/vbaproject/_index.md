---
title: "VbaProject"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar VBA-projektet."
type: docs
url: /sv/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

Representerar VBA-projektet.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | Kopiera VBA-projekt från en annan fil. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | Hämtar certifikatets rådata om detta VBA-projekt är signerat. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | Hämtar kodningen för VBA-projektet. |
| [getIslockedForViewing()](#getIslockedForViewing--) | Indikerar om detta VBA-projekt är låst för visning. |
| [getModules()](#getModules--) | Hämtar alla [VbaModule](../../com.aspose.cells/vbamodule) objekt. |
| [getName()](#getName--) | Hämtar namnet på VBA-projektet. |
| [getReferences()](#getReferences--) | Hämtar alla referenser till VBA-projektet. |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | Indikerar om detta VBA-projekt är låst för visning. |
| [isProtected()](#isProtected--) | Indikerar om detta VBA-projekt är skyddat. |
| [isSigned()](#isSigned--) | Indikerar om VBA-kod är signerad eller inte. |
| [isValidSigned()](#isValidSigned--) | Indikerar om signaturen för VBA-projektet är giltig eller inte. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | Skyddar eller avskyddar detta VBA-projekt. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Ställer in kodningen för VBA-projektet. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på VBA-projektet. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | Signera detta VBA-projekt med en DigitalSignature |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Validerar skyddslösenordet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


Kopiera VBA-projekt från en annan fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


Hämtar certifikatets rådata om detta VBA-projekt är signerat.

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


Hämtar kodningen för VBA-projektet.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


Indikerar om detta VBA-projekt är låst för visning.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället **VbaProject.IsLockedForView**-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2026. **Aspose** ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


Hämtar alla [VbaModule](../../com.aspose.cells/vbamodule) objekt.

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på VBA-projektet.

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


Hämtar alla referenser till VBA-projektet.

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


Indikerar om detta VBA-projekt är låst för visning. Om true, kan koderna inte vara synliga.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indikerar om detta VBA-projekt är skyddat.

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


Indikerar om VBA-kod är signerad eller inte.

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


Indikerar om signaturen för VBA-projektet är giltig eller inte.

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


Skyddar eller avskyddar detta VBA-projekt.

**Remarks**

Om islockedForViewing är true, får lösenordet inte vara null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| islockedForViewing | boolean | indikerar om projektet låses för visning. |
| lösenord | java.lang.String | Om värdet är null, avskyddar detta VBA-projekt, annars skyddar detta VBA-projekt. |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Ställer in kodningen för VBA-projektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på VBA-projektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


Signera detta VBA-projekt med en DigitalSignature

**Parameters:**
| Parameter | Typ | Beskrivning |
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


Validerar skyddslösenordet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | java.lang.String | lösenordet |

**Returns:**
boolean - Huruvida lösenordet är skyddslösenordet för detta VBA-projekt
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

