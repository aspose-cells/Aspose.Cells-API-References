---
title: "VbaProjectReference"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la référence du projet VBA."
type: docs
url: /fr/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

Représente la référence du projet VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         // Add vba project reference
         vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Obtient le Libid étendu de la référence. |
| [getLibid()](#getLibid--) | Obtient le Libid de la référence. |
| [getName()](#getName--) | Obtient le nom de la référence. |
| [getRelativeLibid()](#getRelativeLibid--) | Obtient l'identifiant du projet VBA référencé avec un chemin relatif. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Obtient le Libid modifié de la référence. |
| [getType()](#getType--) | Obtient le type de cette référence. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Définit le Libid étendu de la référence. |
| [setLibid(String value)](#setLibid-java.lang.String-) | Définit le Libid de la référence. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la référence. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Définit l'identifiant du projet VBA référencé avec un chemin relatif. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Définit le Libid modifié de la référence. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExtendedLibid() {#getExtendedLibid--}
```
public String getExtendedLibid()
```


Obtient le Libid étendu de la référence.

**Remarks**

Uniquement pour la référence de contrôle.

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


Obtient le Libid de la référence.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la référence.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


Obtient l'identifiant du projet VBA référencé avec un chemin relatif.

**Remarks**

Uniquement pour la référence du projet.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


Obtient le Libid modifié de la référence.

**Remarks**

Uniquement pour la référence de contrôle.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Obtient le type de cette référence.

Voir [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setExtendedLibid(String value) {#setExtendedLibid-java.lang.String-}
```
public void setExtendedLibid(String value)
```


Définit le Libid étendu de la référence.

**Remarks**

Uniquement pour la référence de contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


Définit le Libid de la référence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la référence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


Définit l'identifiant du projet VBA référencé avec un chemin relatif.

**Remarks**

Uniquement pour la référence du projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


Définit le Libid modifié de la référence.

**Remarks**

Uniquement pour la référence de contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

