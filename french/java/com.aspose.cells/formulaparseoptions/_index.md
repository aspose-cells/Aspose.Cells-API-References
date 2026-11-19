---
title: "FormulaParseOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options lors de l'analyse d'une formule."
type: docs
url: /fr/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

Représente les options lors de l'analyse d'une formule.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | Définition pour l'analyse des fonctions personnalisées. |
| [getLocaleDependent()](#getLocaleDependent--) | Indique si la formule est formatée selon la locale. |
| [getParse()](#getParse--) | Indique s'il faut analyser la formule donnée. |
| [getR1C1Style()](#getR1C1Style--) | Indique si la formule est au style de référence R1C1. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Définition pour l'analyse des fonctions personnalisées. |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | Indique si la formule est formatée selon la locale. |
| [setParse(boolean value)](#setParse-boolean-) | Indique s'il faut analyser la formule donnée. |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | Indique si la formule est au style de référence R1C1. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
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
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. La valeur par défaut est true (si la fonction définie par l'utilisateur correspond à un complément dans les liens externes existants, elle est alors considérée comme le complément).

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


Définition pour l'analyse des fonctions personnalisées.

**Remarks**

Pour certaines exigences spéciales, comme lors du calcul d'une fonction personnalisée dans le moteur personnalisé de l'utilisateur, certains paramètres doivent être calculés en mode tableau ; l'utilisation de cette propriété permet de marquer ces paramètres en mode tableau lors de l'analyse de la formule. Sinon, l'utilisateur doit mettre à jour ces fonctions personnalisées ultérieurement via [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) pour obtenir le même résultat.

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


Indique si la formule est formatée selon la locale. La valeur par défaut est false.

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


Indique s'il faut analyser la formule donnée. La valeur par défaut est true. Si elle est false, la chaîne de formule donnée restera telle quelle pour la cellule jusqu'à ce que l'utilisateur appelle d'autres méthodes pour les analyser ou que les données de formule analysées soient requises par d'autres opérations, comme le calcul des formules.

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


Indique si la formule est au style de référence R1C1. La valeur par défaut est false.

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




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. La valeur par défaut est true (si la fonction définie par l'utilisateur correspond à un complément dans les liens externes existants, elle est alors considérée comme le complément).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


Définition pour l'analyse des fonctions personnalisées.

**Remarks**

Pour certaines exigences spéciales, comme lors du calcul d'une fonction personnalisée dans le moteur personnalisé de l'utilisateur, certains paramètres doivent être calculés en mode tableau ; l'utilisation de cette propriété permet de marquer ces paramètres en mode tableau lors de l'analyse de la formule. Sinon, l'utilisateur doit mettre à jour ces fonctions personnalisées ultérieurement via [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) pour obtenir le même résultat.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


Indique si la formule est formatée selon la locale. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


Indique s'il faut analyser la formule donnée. La valeur par défaut est true. Si elle est false, la chaîne de formule donnée restera telle quelle pour la cellule jusqu'à ce que l'utilisateur appelle d'autres méthodes pour les analyser ou que les données de formule analysées soient requises par d'autres opérations, comme le calcul des formules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


Indique si la formule est au style de référence R1C1. La valeur par défaut est false.

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

