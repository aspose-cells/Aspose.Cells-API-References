---
title: "ProtectedRange"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Une plage spécifiée autorisée à être modifiée lorsque la protection de la feuille est ACTIVÉE."
type: docs
url: /fr/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

Une plage spécifiée autorisée à être modifiée lorsque la protection de la feuille est ACTIVÉE.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | Ajoute une zone référencée à cet objet. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Obtient toutes les zones référencées. |
| [getCellArea()](#getCellArea--) | Obtient le [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) objet qui représente la zone de cellules à protéger. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Obtient le titre de la plage. |
| [getPassword()](#getPassword--) | Représente le mot de passe pour protéger la plage. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | Le descripteur de sécurité définit les comptes d'utilisateur qui peuvent modifier cette plage sans fournir de mot de passe pour y accéder. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indique si la feuille de calcul est protégée par un mot de passe. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | Obtient le titre de la plage. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Représente le mot de passe pour protéger la plage. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | Le descripteur de sécurité définit les comptes d'utilisateur qui peuvent modifier cette plage sans fournir de mot de passe pour y accéder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


Ajoute une zone référencée à cet objet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ. |
| startColumn | int | La colonne de départ. |
| endRow | int | La ligne de fin. |
| endColumn | int | La colonne de fin. |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Obtient toutes les zones référencées.

**Returns:**
com.aspose.cells.CellArea[] - Retourne toutes les zones référencées.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Obtient le [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) objet qui représente la zone de cellules à protéger.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Obtient le titre de la plage. Ceci est utilisé comme un descripteur, et non comme une définition de plage nommée.

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


Représente le mot de passe pour protéger la plage.

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


Le descripteur de sécurité définit les comptes d'utilisateur qui peuvent modifier cette plage sans fournir de mot de passe pour y accéder.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Indique si la feuille de calcul est protégée par un mot de passe.

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




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Obtient le titre de la plage. Ceci est utilisé comme un descripteur, et non comme une définition de plage nommée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Représente le mot de passe pour protéger la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


Le descripteur de sécurité définit les comptes d'utilisateur qui peuvent modifier cette plage sans fournir de mot de passe pour y accéder.

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

