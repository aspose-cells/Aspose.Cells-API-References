---
title: "AutoFitterOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente toutes les options d'ajustement automatique."
type: docs
url: /fr/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

Représente toutes les options d'ajustement automatique.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Indique si la hauteur de ligne doit être ajustée automatiquement lorsque les cellules sont fusionnées dans une ligne. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | Obtient le type d'ajustement automatique de la hauteur de ligne des cellules fusionnées. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | Obtient le type d'ajustement automatique du texte renvoyé à la ligne. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Obtient la langue d’édition par défaut. |
| [getForRendering()](#getForRendering--) | Indique si l'ajustement est destiné à des fins de rendu. |
| [getFormatStrategy()](#getFormatStrategy--) | Obtient la stratégie de formatage. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Ignore les lignes/colonnes masquées. |
| [getMaxRowHeight()](#getMaxRowHeight--) | Obtient la hauteur maximale de ligne (en unité de point) lors de l'ajustement automatique des lignes. |
| [getOnlyAuto()](#getOnlyAuto--) | Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | Indique si la hauteur de ligne doit être ajustée automatiquement lorsque les cellules sont fusionnées dans une ligne. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | Définit le type d'ajustement automatique de la hauteur des lignes des cellules fusionnées. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | Définit le type d'ajustement automatique du texte renvoyé à la ligne. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Définit la langue d'édition par défaut. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | Indique si l'ajustement est destiné à des fins de rendu. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Définit la stratégie de formatage. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | Ignore les lignes/colonnes masquées. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | Définit la hauteur maximale des lignes (en points) lors de l'ajustement automatique des lignes. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


Indique si la hauteur des lignes doit être ajustée automatiquement lorsque les cellules sont fusionnées dans une ligne. La valeur par défaut est false.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété AutoFitterOptions.AutoFitMergedCellsType. Cette propriété sera supprimée 12 mois après décembre 2018. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


Obtient le type d'ajustement automatique de la hauteur de ligne des cellules fusionnées.

Voir [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel ignore par défaut les cellules fusionnées lors de l'ajustement de la hauteur des lignes, ainsi Aspose.Cells fonctionne comme le réglage par défaut de MS Excel. Veuillez définir ce type pour modifier la façon dont la hauteur des lignes des cellules fusionnées est ajustée automatiquement.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


Obtient le type d'ajustement automatique du texte renvoyé à la ligne.

Voir [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Obtient la langue d’édition par défaut.

Voir [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Il peut afficher/rendre différentes mises en page pour le paragraphe de texte lorsque différentes langues d'édition sont définies. La valeur par défaut est [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\\#AUTO).

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


Indique si l'ajustement est destiné à des fins de rendu.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Obtient la stratégie de formatage.

Voir [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

La valeur par défaut est CellStyle pour les performances.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


Ignore les lignes/colonnes masquées.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


Obtient la hauteur maximale de ligne (en unité de point) lors de l'ajustement automatique des lignes.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


Indique si la hauteur des lignes doit être ajustée automatiquement lorsque les cellules sont fusionnées dans une ligne. La valeur par défaut est false.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété AutoFitterOptions.AutoFitMergedCellsType. Cette propriété sera supprimée 12 mois après décembre 2018. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


Définit le type d'ajustement automatique de la hauteur des lignes des cellules fusionnées.

Voir [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel ignore par défaut les cellules fusionnées lors de l'ajustement de la hauteur des lignes, ainsi Aspose.Cells fonctionne comme le réglage par défaut de MS Excel. Veuillez définir ce type pour modifier la façon dont la hauteur des lignes des cellules fusionnées est ajustée automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


Définit le type d'ajustement automatique du texte renvoyé à la ligne.

Voir [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Définit la langue d'édition par défaut.

Voir [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Il peut afficher/rendre différentes mises en page pour le paragraphe de texte lorsque différentes langues d'édition sont définies. La valeur par défaut est [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\\#AUTO).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


Indique si l'ajustement est destiné à des fins de rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Définit la stratégie de formatage.

Voir [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

La valeur par défaut est CellStyle pour les performances.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


Ignore les lignes/colonnes masquées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


Définit la hauteur maximale des lignes (en points) lors de l'ajustement automatique des lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées.

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

