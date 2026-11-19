---
title: "FormatConditionType"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Type de règle de mise en forme conditionnelle."
type: docs
url: /fr/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

Type de règle de mise en forme conditionnelle.
## Champs

| Champ | Description |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont au-dessus ou en dessous de la moyenne de toutes les valeurs de la plage. |
| [BEGINS_WITH](#BEGINS-WITH) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules de la plage qui commencent par le texte donné. |
| [CELL_VALUE](#CELL-VALUE) | Cette règle de mise en forme conditionnelle compare la valeur d’une cellule à un résultat calculé par une formule, en utilisant un opérateur. |
| [COLOR_SCALE](#COLOR-SCALE) | Cette règle de mise en forme conditionnelle crée une échelle de couleur graduée sur les cellules. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont complètement vides. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des erreurs de formule. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant le texte donné. |
| [DATA_BAR](#DATA-BAR) | Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | Cette règle de mise en forme conditionnelle met en surbrillance les valeurs dupliquées. |
| [ENDS_WITH](#ENDS-WITH) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules se terminant par le texte donné. |
| [EXPRESSION](#EXPRESSION) | Cette règle de mise en forme conditionnelle contient une formule à évaluer. |
| [ICON_SET](#ICON-SET) | Cette règle de mise en forme conditionnelle applique des icônes aux cellules en fonction de leurs valeurs. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne sont pas vides. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules sans erreurs de formule. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne contiennent pas le texte donné. |
| [TIME_PERIOD](#TIME-PERIOD) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des dates dans la période spécifiée. |
| [TOP_10](#TOP-10) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans le premier N ou le dernier N, selon la spécification. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | Cette règle de mise en forme conditionnelle met en surbrillance les valeurs uniques de la plage. |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont au-dessus ou en dessous de la moyenne de toutes les valeurs de la plage.

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules de la plage qui commencent par le texte donné. Équivalent à l’utilisation de la fonction feuille LEFT() et à la comparaison des valeurs.

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Cette règle de mise en forme conditionnelle compare la valeur d’une cellule à un résultat calculé par une formule, en utilisant un opérateur.

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


Cette règle de mise en forme conditionnelle crée une échelle de couleur graduée sur les cellules.

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont complètement vides. Équivalent à l’utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide.

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des erreurs de formule. Équivalent à l’utilisation de la fonction feuille ISERROR() pour déterminer s’il y a une erreur de formule.

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant le texte donné. Équivalent à l’utilisation de la fonction feuille SEARCH() pour déterminer si la cellule contient le texte.

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules.

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


Cette règle de mise en forme conditionnelle met en surbrillance les valeurs dupliquées.

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules se terminant par le texte donné. Équivalent à l’utilisation de la fonction feuille RIGHT() et à la comparaison des valeurs.

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


Cette règle de mise en forme conditionnelle contient une formule à évaluer. Lorsque le résultat de la formule est vrai, la cellule est mise en surbrillance.

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


Cette règle de mise en forme conditionnelle applique des icônes aux cellules en fonction de leurs valeurs.

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne sont pas vides. Équivalent à l'utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide.

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules sans erreurs de formule. Équivalent à l'utilisation de la fonction de feuille ISERROR() pour déterminer s'il y a une erreur de formule.

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne contiennent pas le texte donné. Équivalent à l'utilisation de la fonction de feuille SEARCH() pour déterminer si la cellule contient le texte ou non.

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des dates dans la période spécifiée. La valeur sous‑jacent de la cellule est évaluée, ainsi la cellule n’a pas besoin d’être formatée en date pour être évaluée. Par exemple, avec une cellule contenant la valeur 38913, le format conditionnel sera appliqué si la règle nécessite une valeur du 14/07/2006.

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans le premier N ou le dernier N, selon la spécification.

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


Cette règle de mise en forme conditionnelle met en surbrillance les valeurs uniques de la plage.

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

