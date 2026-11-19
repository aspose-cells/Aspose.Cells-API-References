---
title: "Name"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un nom défini pour une plage de cellules."
type: docs
url: /fr/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

Représente un nom défini pour une plage de cellules.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Obtient le commentaire du nom. |
| [getFullText()](#getFullText--) | Obtient le texte complet du nom de l’objet avec le paramètre de portée. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | Obtient une référence R1C1 du [Name](../../com.aspose.cells/name). |
| [getRange()](#getRange--) | Obtient la plage si ce nom fait référence à une plage. |
| [getRange(boolean recalculate)](#getRange-boolean-) | Obtient la plage si ce nom fait référence à une plage |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | Obtient la plage si ce nom fait référence à une plage. |
| [getRanges()](#getRanges--) | Obtient toutes les plages référencées par ce nom. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | Obtient toutes les plages référencées par ce nom. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | Obtient toutes les références référencées par ce nom. |
| [getRefersTo()](#getRefersTo--) | Renvoie ou définit la formule à laquelle le nom est défini pour faire référence, en commençant par un signe égal. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | Obtenez la référence de ce Nom. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | Obtenez la référence de ce Nom en fonction de la cellule spécifiée. |
| [getSheetIndex()](#getSheetIndex--) | Indique que ce nom appartient au classeur ou à la feuille de calcul. 0 = nom global, sinon indice de la feuille (basé sur 1). |
| [getText()](#getText--) | Obtient le texte du nom de l'objet. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indique si ce nom est référencé par d'autres formules. |
| [isVisible()](#isVisible--) | Indique si le nom est visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | Définit le commentaire du nom. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | Définit une référence R1C1 du [Name](../../com.aspose.cells/name). |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | Renvoie ou définit la formule à laquelle le nom est défini pour faire référence, en commençant par un signe égal. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | Définissez la référence de ce Nom. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Indique que ce nom appartient au classeur ou à la feuille de calcul. 0 = nom global, sinon indice de la feuille (basé sur 1). |
| [setText(String value)](#setText-java.lang.String-) | Obtient le texte du nom de l'objet. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indique si le nom est visible. |
| [toString()](#toString--) | Renvoie une chaîne représentant l'objet Range actuel. |
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
### getComment() {#getComment--}
```
public String getComment()
```


Obtient le commentaire du nom. S'applique uniquement aux versions Excel 2007 ou supérieures.

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


Obtient le texte complet du nom de l’objet avec le paramètre de portée.

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


Obtient une référence R1C1 du [Name](../../com.aspose.cells/name).

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Obtient la plage si ce nom fait référence à une plage.

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


Obtient la plage si ce nom fait référence à une plage

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| recalculer | boolean | si le recalculer si ce nom a déjà été calculé avant cet appel. |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


Obtient la plage si ce nom fait référence à une plage. Si la référence de ce nom n'est pas absolue, la plage peut différer selon la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | L'indice de la feuille correspondant. |
| ligne | int | L'indice de la ligne correspondant. |
| colonne | int | L'indice de la colonne correspondant |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Obtient toutes les plages référencées par ce nom.

**Returns:**
com.aspose.cells.Range[] - Toutes les plages.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


Obtient toutes les plages référencées par ce nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| recalculer | boolean | si le recalculer si ce nom a déjà été calculé avant cet appel. |

**Returns:**
com.aspose.cells.Range[] - Toutes les plages.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


Obtient toutes les références référencées par ce nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| recalculer | boolean | si le recalculer si ce nom a déjà été calculé avant cet appel. |

**Returns:**
com.aspose.cells.ReferredArea[] - Toutes les plages.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Renvoie ou définit la formule à laquelle le nom est défini pour faire référence, en commençant par un signe égal.

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


Obtenez la référence de ce Nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la référence doit être formatée en R1C1. |
| isLocal | boolean | Indique si la référence doit être formatée selon la locale. |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtenez la référence de ce Nom en fonction de la cellule spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la référence doit être formatée en R1C1. |
| isLocal | boolean | Indique si la référence doit être formatée selon la locale. |
| ligne | int | L'indice de ligne de la cellule. |
| colonne | int | L'index de colonne de la cellule. |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Indique que ce nom appartient au classeur ou à la feuille de calcul. 0 = nom global, sinon indice de la feuille (basé sur 1).

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Obtient le texte du nom de l'objet.

**Returns:**
java.lang.String
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


Indique si ce nom est référencé par d'autres formules.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indique si le nom est visible.

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




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Définit le commentaire du nom. S'applique uniquement aux versions Excel 2007 ou supérieures.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


Définit une référence R1C1 du [Name](../../com.aspose.cells/name).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


Renvoie ou définit la formule à laquelle le nom est défini pour faire référence, en commençant par un signe égal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


Définissez la référence de ce Nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| refersTo | java.lang.String | La référence. |
| isR1C1 | boolean | Indique si la référence est au format R1C1. |
| isLocal | boolean | Si la référence est formatée selon la locale. |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


Indique que ce nom appartient au classeur ou à la feuille de calcul. 0 = nom global, sinon indice de la feuille (basé sur 1).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Obtient le texte du nom de l'objet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indique si le nom est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne représentant l'objet Range actuel.

**Returns:**
java.lang.String -
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

