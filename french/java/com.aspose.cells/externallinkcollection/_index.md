---
title: "ExternalLinkCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la collection de liens externes dans un classeur."
type: docs
url: /fr/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

Représente la collection de liens externes dans un classeur.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | Ajouter un lien externe. |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | Ajoute un lien externe. |
| [clear()](#clear--) | Supprime tous les liens externes. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | Supprime tous les liens externes. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [ExternalLink](../../com.aspose.cells/externallink) à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments réellement contenus dans la collection. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Obtenez un énumérateur qui parcourt cette collection. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime le lien externe spécifié du classeur. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | Supprime le lien externe spécifié du classeur. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


Ajouter un lien externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). Le type de répertoire du nom de fichier. |
| fileName | java.lang.String | le nom de fichier. |
| sheetNames | java.lang.String[] | Tous les noms de feuilles du fichier externe. |

**Returns:**
int - La position du nom externe dans cette liste.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


Ajoute un lien externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier externe. |
| sheetNames | java.lang.String[] | Tous les noms de feuilles du fichier externe. |

**Returns:**
int - La position du nom externe dans cette liste.
### clear() {#clear--}
```
public void clear()
```


Supprime tous les liens externes.

**Remarks**

Lors de la suppression des liens externes, toutes les formules qui y font référence seront également supprimées car les références deviennent invalides.

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


Supprime tous les liens externes.

**Remarks**

Si les références doivent être mises à jour, ces références de liens externes dans les formules seront remplacées par le classeur actuel lorsque cela est possible. Par exemple, la formule originale d’une cellule est "='externalsource.xlam'!customfunction()", après la suppression des liens externes, la formule deviendra "=customfunction()" ; lorsque la formule originale est "='[externalsource.xlam]Sheet1'!$A$1", selon qu’il existe une feuille nommée "Sheet1" dans le classeur actuel : si vrai, la formule deviendra "=Sheet1!$A$1" ; si faux, la formule deviendra "=\#REF!$A$1".

Si les références ne doivent pas être mises à jour, toutes les formules contenant des références à des liens externes seront également supprimées car ces références deviennent invalides.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Indique si toutes les références des liens externes dans les formules doivent être mises à jour vers les références du classeur actuel lui‑même. |

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
### get(int index) {#get-int-}
```
public ExternalLink get(int index)
```


Obtient l'élément [ExternalLink](../../com.aspose.cells/externallink) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre d'éléments réellement contenus dans la collection.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtenez un énumérateur qui parcourt cette collection.

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime le lien externe spécifié du classeur.

**Remarks**

Lors de la suppression du lien externe, toutes les formules qui y font référence seront également supprimées car les références deviennent invalides.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l’index du lien externe à supprimer. |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


Supprime le lien externe spécifié du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l’index du lien externe à supprimer. |
| updateReferencesAsLocal | boolean | Indique si toutes les références du lien externe donné doivent être mises à jour vers la référence du classeur actuel lui‑même. Consultez [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) pour obtenir plus de détails sur ce paramètre. |

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

