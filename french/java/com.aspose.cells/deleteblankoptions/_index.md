---
title: "DeleteBlankOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le paramètre de suppression des cellules/lignes/colonnes vides."
type: docs
url: /fr/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

Représente le paramètre de suppression des cellules/lignes/colonnes vides.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | Indique si les objets liés au dessin tels que l'image, la forme, le graphique... seront considérés comme vides. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | Indique si une cellule sera considérée comme vide lorsqu'elle contient une formule dont le résultat calculé est nul ou une chaîne vide. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. |
| [getEndIndex()](#getEndIndex--) | Spécifie l'index de fin de ligne/colonne (inclusif) de la plage à vérifier et à supprimer les lignes/colonnes vides. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | Obtient le moniteur pour suivre les modifications causées par la suppression. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | Indique comment traiter les cellules fusionnées lors de la suppression des lignes/colonnes vides. |
| [getStartIndex()](#getStartIndex--) | Spécifie l'index de début de ligne/colonne de la plage à vérifier et à supprimer les lignes/colonnes vides. |
| [getUpdateReference()](#getUpdateReference--) | Indique s'il faut mettre à jour les références dans les autres feuilles de calcul. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | Indique si les objets liés au dessin tels que l'image, la forme, le graphique... seront considérés comme vides. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | Indique si une cellule sera considérée comme vide lorsqu'elle contient une formule dont le résultat calculé est nul ou une chaîne vide. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. |
| [setEndIndex(int value)](#setEndIndex-int-) | Spécifie l'index de fin de ligne/colonne (inclusif) de la plage à vérifier et à supprimer les lignes/colonnes vides. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | Définit le moniteur pour suivre les modifications causées par la suppression. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | Indique comment traiter les cellules fusionnées lors de la suppression des lignes/colonnes vides. |
| [setStartIndex(int value)](#setStartIndex-int-) | Spécifie l'index de début de ligne/colonne de la plage à vérifier et à supprimer les lignes/colonnes vides. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indique s'il faut mettre à jour les références dans les autres feuilles de calcul. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
```


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
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


Indique si les objets liés au dessin tels que l'image, la forme, le graphique... seront considérés comme vides. La valeur par défaut est true.

**Remarks**

Lorsqu'on définit cette propriété sur false, toutes les lignes/colonnes couvertes par des objets de dessin ne seront pas considérées comme vides et ne seront pas supprimées.

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


Indique si une cellule sera considérée comme vide lorsqu'elle est une formule et que le résultat calculé est nul ou une chaîne vide. La valeur par défaut est false.

**Remarks**

En général, l'utilisateur doit s'assurer que les formules ont été calculées avant l'opération de suppression lorsque cette propriété est vraie. Sinon, toutes les nouvelles formules créées par les API normales telles que [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) seront considérées comme vides et pourront être supprimées car, avant le calcul, leurs résultats calculés sont tous nuls.

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. La valeur par défaut est true.

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


Spécifie l'index de fin de ligne/colonne (inclusif) de la plage à vérifier et à supprimer les lignes/colonnes vides. La valeur par défaut est -1 et -1 signifie la plage maximale de tous les objets (cellules, dessins, ...) qui doivent être vérifiés.

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


Obtient le moniteur pour suivre les modifications causées par la suppression.

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


Indique comment traiter les cellules fusionnées lors de la suppression des lignes/colonnes vides.

Voir [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Pour [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY), toutes les cellules qu'il contient seront considérées comme vides sauf la cellule en haut à gauche qui n'est pas vide. C'est la valeur par défaut de cette propriété.

Pour [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE), toutes les cellules qu'il contient seront considérées comme non vides.

Pour [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT), toutes les cellules situées en dehors de la zone d'affichage du contenu seront considérées comme vides.



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Spécifie l'index de début de ligne/colonne de la plage à vérifier et à supprimer les lignes/colonnes vides.

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Indique s'il faut mettre à jour les références dans les autres feuilles de calcul.

**Remarks**

À partir de la version 26.7, nous définissons la valeur par défaut de cette propriété à true.

**Returns:**
boolean
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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


Indique si les objets liés au dessin tels que l'image, la forme, le graphique... seront considérés comme vides. La valeur par défaut est true.

**Remarks**

Lorsqu'on définit cette propriété sur false, toutes les lignes/colonnes couvertes par des objets de dessin ne seront pas considérées comme vides et ne seront pas supprimées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


Indique si une cellule sera considérée comme vide lorsqu'elle est une formule et que le résultat calculé est nul ou une chaîne vide. La valeur par défaut est false.

**Remarks**

En général, l'utilisateur doit s'assurer que les formules ont été calculées avant l'opération de suppression lorsque cette propriété est vraie. Sinon, toutes les nouvelles formules créées par les API normales telles que [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) seront considérées comme vides et pourront être supprimées car, avant le calcul, leurs résultats calculés sont tous nuls.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


Spécifie l'index de fin de ligne/colonne (inclusif) de la plage à vérifier et à supprimer les lignes/colonnes vides. La valeur par défaut est -1 et -1 signifie la plage maximale de tous les objets (cellules, dessins, ...) qui doivent être vérifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


Définit le moniteur pour suivre les modifications causées par la suppression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


Indique comment traiter les cellules fusionnées lors de la suppression des lignes/colonnes vides.

Voir [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Pour [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY), toutes les cellules qu'il contient seront considérées comme vides sauf la cellule en haut à gauche qui n'est pas vide. C'est la valeur par défaut de cette propriété.

Pour [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE), toutes les cellules qu'il contient seront considérées comme non vides.

Pour [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT), toutes les cellules situées en dehors de la zone d'affichage du contenu seront considérées comme vides.



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


Spécifie l'index de début de ligne/colonne de la plage à vérifier et à supprimer les lignes/colonnes vides.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Indique s'il faut mettre à jour les références dans les autres feuilles de calcul.

**Remarks**

À partir de la version 26.7, nous définissons la valeur par défaut de cette propriété à true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

