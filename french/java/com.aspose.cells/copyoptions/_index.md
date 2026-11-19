---
title: "CopyOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de copie."
type: docs
url: /fr/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

Représente les options de copie.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | Constructeur CopyOptions. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Indique si la largeur des colonnes est copiée en unités de caractères. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | Si la formule n'est pas valide pour la destination dest, seules les valeurs sont copiées. |
| [getCopyNames()](#getCopyNames--) | Indique si les noms sont copiés. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Indique s'il faut étendre les plages lors de la copie de la plage vers la plage adjacente. |
| [getKeepMacros()](#getKeepMacros--) | Indique si les macros sont conservées ; |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul tout en copiant une feuille vers une autre, les formules copiées doivent faire référence au classeur source. |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | Indique s'il faut se référer à la feuille cible si la feuille référencée n'est pas copiée. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | Indique si la largeur des colonnes est copiée en unités de caractères. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | Si la formule n'est pas valide pour la destination dest, seules les valeurs sont copiées. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | Indique si les noms sont copiés. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | Indique s'il faut étendre les plages lors de la copie de la plage vers la plage adjacente. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | Indique si les macros sont conservées ; |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul tout en copiant une feuille vers une autre, les formules copiées doivent faire référence au classeur source. |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | Indique s'il faut se référer à la feuille cible si la feuille référencée n'est pas copiée. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


Constructeur CopyOptions.

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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


Indique si la largeur des colonnes est copiée en unités de caractères.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


Si la formule n'est pas valide pour la destination dest, seules les valeurs sont copiées.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


Indique si les noms sont copiés.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


Indique s'il faut étendre les plages lors de la copie de la plage vers la plage adjacente.

**Remarks**

Si c'est vrai, cela étend uniquement la plage du lien hypertexte, sans ajouter de nouveau lien hypertexte lors de la copie des liens hypertexte vers des lignes adjacentes.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


Indique si les macros sont conservées ;

**Remarks**

Uniquement pour la copie du classeur.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. True signifie que la source de données du graphique copié fait référence à la feuille de destination.

**Remarks**

La valeur par défaut est false, cela fonctionne comme MS Excel. Par exemple : si vous copiez un graphique avec la source de données "sheet1!A1:B10" depuis la feuille de calcul "sheet1 to other worksheet "sheet2", la source de données sera modifiée en "sheet2!A1:B10"

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul tout en copiant une feuille vers une autre, les formules copiées doivent faire référence au classeur source. Cependant, dans certaines situations, l'utilisateur peut avoir besoin que les formules copiées fassent référence à des feuilles portant le même nom dans le même classeur, par exemple lorsque ces feuilles ont été copiées avant cette opération de copie, auquel cas cette propriété doit être conservée à true.

**Remarks**

La valeur par défaut est true.

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


Indique s'il faut se référer à la feuille cible si la feuille référencée n'est pas copiée.

**Remarks**

Fonctionne uniquement lors de la copie d'une plage ou d'une feuille depuis un autre classeur.

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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


Indique si la largeur des colonnes est copiée en unités de caractères.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


Si la formule n'est pas valide pour la destination dest, seules les valeurs sont copiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


Indique si les noms sont copiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


Indique s'il faut étendre les plages lors de la copie de la plage vers la plage adjacente.

**Remarks**

Si c'est vrai, cela étend uniquement la plage du lien hypertexte, sans ajouter de nouveau lien hypertexte lors de la copie des liens hypertexte vers des lignes adjacentes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


Indique si les macros sont conservées ;

**Remarks**

Uniquement pour la copie du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. True signifie que la source de données du graphique copié fait référence à la feuille de destination.

**Remarks**

La valeur par défaut est false, cela fonctionne comme MS Excel. Par exemple : si vous copiez un graphique avec la source de données "sheet1!A1:B10" depuis la feuille de calcul "sheet1 to other worksheet "sheet2", la source de données sera modifiée en "sheet2!A1:B10"

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul tout en copiant une feuille vers une autre, les formules copiées doivent faire référence au classeur source. Cependant, dans certaines situations, l'utilisateur peut avoir besoin que les formules copiées fassent référence à des feuilles portant le même nom dans le même classeur, par exemple lorsque ces feuilles ont été copiées avant cette opération de copie, auquel cas cette propriété doit être conservée à true.

**Remarks**

La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


Indique s'il faut se référer à la feuille cible si la feuille référencée n'est pas copiée.

**Remarks**

Fonctionne uniquement lors de la copie d'une plage ou d'une feuille depuis un autre classeur.

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

