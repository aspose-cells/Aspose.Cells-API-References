---
title: "LookInType"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le type de recherche."
type: docs
url: /fr/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

Représente le type de recherche.
## Champs

| Champ | Description |
| --- | --- |
| [COMMENTS](#COMMENTS) | Recherche l'objet uniquement dans le commentaire de la cellule. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | Recherche l'objet uniquement à partir de la valeur formatée de la cellule([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [FORMULAS](#FORMULAS) | Recherche l'objet recherché à partir de la formule([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) si la cellule est une formule, sinon recherche à partir de la valeur originale de la cellule (identique à [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)). |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | Ignore les cellules qui ne sont pas des formules. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | Trouve l'objet à partir de la valeur d'origine de la cellule uniquement. |
| [VALUES](#VALUES) | Trouve l'objet à partir de la valeur d'origine de la cellule([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) et de la valeur formatée([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | Ignore les cellules qui sont des formules. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


Trouve l'objet à partir du commentaire de la cellule uniquement. Ignore les cellules qui n'ont pas de commentaire.

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


Recherche l'objet uniquement à partir de la valeur formatée de la cellule([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


Recherche l'objet recherché à partir de la formule([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) si la cellule est une formule, sinon recherche à partir de la valeur originale de la cellule (identique à [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)).

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


Ignore les cellules qui ne sont pas des formules. Pour les cellules qui sont des formules, trouve l'objet recherché à partir de la formule([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)).

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


Trouve l'objet à partir de la valeur d'origine de la cellule uniquement.

### VALUES {#VALUES}
```
public static final int VALUES
```


Trouve l'objet à partir de la valeur d'origine de la cellule([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) et de la valeur formatée([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


Ignore les cellules qui sont des formules. Pour les cellules qui ne sont pas des formules, c'est identique à [VALUES](../../com.aspose.cells/lookintype\#VALUES).

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

