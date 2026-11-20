---
title: "VbaProject"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt das VBA‑Projekt dar."
type: docs
url: /de/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

Stellt das VBA‑Projekt dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | Kopiere VBA-Projekt aus einer anderen Datei. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | Liefert die rohen Zertifikatsdaten, wenn dieses VBA-Projekt signiert ist. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | Liefert die Kodierung des VBA-Projekts. |
| [getIslockedForViewing()](#getIslockedForViewing--) | Gibt an, ob dieses VBA-Projekt für die Ansicht gesperrt ist. |
| [getModules()](#getModules--) | Liefert alle [VbaModule](../../com.aspose.cells/vbamodule)-Objekte. |
| [getName()](#getName--) | Liefert den Namen des VBA-Projekts. |
| [getReferences()](#getReferences--) | Liefert alle Verweise des VBA-Projekts. |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | Gibt an, ob dieses VBA-Projekt für die Ansicht gesperrt ist. |
| [isProtected()](#isProtected--) | Gibt an, ob dieses VBA-Projekt geschützt ist. |
| [isSigned()](#isSigned--) | Gibt an, ob VBA-Code signiert ist oder nicht. |
| [isValidSigned()](#isValidSigned--) | Gibt an, ob die Signatur des VBA-Projekts gültig ist oder nicht. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | Schützt oder hebt den Schutz dieses VBA-Projekts auf. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Setzt die Kodierung des VBA-Projekts. |
| [setName(String value)](#setName-java.lang.String-) | Setzt den Namen des VBA-Projekts. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | Signiere dieses VBA-Projekt mit einer DigitalSignature |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Validiert das Schutzkennwort. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


Kopiere VBA-Projekt aus einer anderen Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


Liefert die rohen Zertifikatsdaten, wenn dieses VBA-Projekt signiert ist.

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


Liefert die Kodierung des VBA-Projekts.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


Gibt an, ob dieses VBA-Projekt für die Ansicht gesperrt ist.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft VbaProject.IsLockedForView. Diese Eigenschaft wird 12 Monate nach Juli 2026 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


Liefert alle [VbaModule](../../com.aspose.cells/vbamodule)-Objekte.

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


Liefert den Namen des VBA-Projekts.

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


Liefert alle Verweise des VBA-Projekts.

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


Gibt an, ob dieses VBA-Projekt für die Ansicht gesperrt ist. Wenn true, können die Codes nicht sichtbar sein.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Gibt an, ob dieses VBA-Projekt geschützt ist.

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


Gibt an, ob VBA-Code signiert ist oder nicht.

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


Gibt an, ob die Signatur des VBA-Projekts gültig ist oder nicht.

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


Schützt oder hebt den Schutz dieses VBA-Projekts auf.

**Remarks**

Wenn islockedForViewing true ist, darf das Passwort nicht null sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| islockedForViewing | boolean | gibt an, ob das Projekt für die Anzeige gesperrt ist. |
| Passwort | java.lang.String | Wenn der Wert null ist, wird dieses VBA-Projekt ungeschützt, andernfalls wird das VBA-Projekt geschützt. |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Setzt die Kodierung des VBA-Projekts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Setzt den Namen des VBA-Projekts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


Signiere dieses VBA-Projekt mit einer DigitalSignature

**Parameters:**
| Parameter | Typ | Beschreibung |
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


Validiert das Schutzkennwort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | java.lang.String | das Passwort |

**Returns:**
boolesch – Ob das Passwort das Schutzpasswort dieses VBA-Projekts ist
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

