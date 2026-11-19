---
title: "VbaProject"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le projet VBA."
type: docs
url: /fr/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

Représente le projet VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | Copier le projet VBA depuis un autre fichier. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | Obtient les données brutes du certificat si ce projet VBA est signé. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | Obtient l'encodage du projet VBA. |
| [getIslockedForViewing()](#getIslockedForViewing--) | Indique si ce projet VBA est verrouillé pour la visualisation. |
| [getModules()](#getModules--) | Obtient tous les objets [VbaModule](../../com.aspose.cells/vbamodule). |
| [getName()](#getName--) | Obtient le nom du projet VBA. |
| [getReferences()](#getReferences--) | Obtient toutes les références du projet VBA. |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | Indique si ce projet VBA est verrouillé pour la visualisation. |
| [isProtected()](#isProtected--) | Indique si ce projet VBA est protégé. |
| [isSigned()](#isSigned--) | Indique si le code VBA est signé ou non. |
| [isValidSigned()](#isValidSigned--) | Indique si la signature du projet VBA est valide ou non. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | Protège ou déprotège ce projet VBA. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Définit l'encodage du projet VBA. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom du projet VBA. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | Signer ce projet VBA avec une DigitalSignature |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Valide le mot de passe de protection. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


Copier le projet VBA depuis un autre fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


Obtient les données brutes du certificat si ce projet VBA est signé.

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


Obtient l'encodage du projet VBA.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


Indique si ce projet VBA est verrouillé pour la visualisation.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété VbaProject.IsLockedForView. Cette propriété sera supprimée 12 mois plus tard à partir de juillet 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


Obtient tous les objets [VbaModule](../../com.aspose.cells/vbamodule).

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


Obtient le nom du projet VBA.

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


Obtient toutes les références du projet VBA.

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


Indique si ce projet VBA est verrouillé pour la visualisation. Si vrai, le code ne peut pas être visible.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indique si ce projet VBA est protégé.

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


Indique si le code VBA est signé ou non.

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


Indique si la signature du projet VBA est valide ou non.

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


Protège ou déprotège ce projet VBA.

**Remarks**

Si islockedForViewing est vrai, le mot de passe ne peut pas être nul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| islockedForViewing | boolean | indique si le projet est verrouillé pour la visualisation. |
| password | java.lang.String | Si la valeur est nulle, déprotège ce projet VBA, sinon le protège. |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Définit l'encodage du projet VBA.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom du projet VBA.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


Signer ce projet VBA avec une DigitalSignature

**Parameters:**
| Paramètre | Type | Description |
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


Valide le mot de passe de protection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| password | java.lang.String | le mot de passe |

**Returns:**
booléen - Indique si le mot de passe est le mot de passe de protection de ce projet VBA
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

