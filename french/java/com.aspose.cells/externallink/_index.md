---
title: "ExternalLink"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un lien externe dans un classeur."
type: docs
url: /fr/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

Représente un lien externe dans un classeur.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | Ajoute un nom externe. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | Représente la source de données du lien externe. |
| [getOriginalDataSource()](#getOriginalDataSource--) | Représente la source de données stockée du lien externe. |
| [getPathType()](#getPathType--) | Obtenir le type de chemin de ce lien externe |
| [getType()](#getType--) | Obtient le type du lien externe. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indique si ce lien externe est référencé par d'autres. |
| [isVisible()](#isVisible--) | Indique si ce lien externe est visible dans MS Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | Représente la source de données du lien externe. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | Représente la source de données stockée du lien externe. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


Ajoute un nom externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| texte | java.lang.String | Le texte du nom externe. Si le nom externe appartient à une feuille de calcul, le texte doit être sous la forme Sheet1!Text. |
| referTo | java.lang.String | Le referTo du nom externe. Il doit s'agir d'une cellule ou de la plage. |

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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```


Représente la source de données du lien externe.

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


Représente la source de données stockée du lien externe.

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


Obtenir le type de chemin de ce lien externe

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Obtient le type du lien externe.

Voir [ExternalLinkType](../../com.aspose.cells/externallinktype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Indique si ce lien externe est référencé par d'autres.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indique si ce lien externe est visible dans MS Excel.

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




### setDataSource(String value) {#setDataSource-java.lang.String-}
```
public void setDataSource(String value)
```


Représente la source de données du lien externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


Représente la source de données stockée du lien externe.

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

