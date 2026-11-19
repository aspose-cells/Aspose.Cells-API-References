---
title: "SplitPartInfo"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les informations d'une entrée/sortie pour plusieurs entrées/sorties, comme la page actuelle à rendre lors de la conversion d'une feuille de calcul en image."
type: docs
url: /fr/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

Représente les informations d'une entrée/sortie pour plusieurs entrées/sorties, comme la page actuelle à rendre lors de la conversion d'une feuille de calcul en image.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | Index de la partie actuelle dans la séquence (à partir de 0) |
| [getSheetIndex()](#getSheetIndex--) | Index de la feuille contenant la partie actuelle. -1 indique qu'il n'y a qu'une seule feuille. |
| [getSheetName()](#getSheetName--) | Nom de la feuille contenant la partie actuelle. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


Index de la partie actuelle dans la séquence (à partir de 0). -1 signifie qu'il n'y a pas de parties multiples, donc le résultat est unique.

**Remarks**

Si plusieurs feuilles doivent être traitées et que chaque feuille est traitée (séparée) en plusieurs parties, l'index de partie commence toujours à 0 pour chaque feuille. Par exemple, lors de la conversion du classeur en images, il représente l'index de page de sortie de la feuille actuellement traitée. Et -1 indique qu'il n'y a qu'une seule page pour la feuille actuelle.

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Index de la feuille contenant la partie actuelle. -1 indique qu'il n'y a qu'une seule feuille.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Nom de la feuille contenant la partie actuelle.

**Remarks**

Peut être nul dans certaines situations, comme lors du rendu du classeur complet en image TIFF.

**Returns:**
java.lang.String
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

