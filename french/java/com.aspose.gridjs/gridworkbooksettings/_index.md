---
title: "GridWorkbookSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les paramètres du classeur."
type: docs
url: /fr/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Représente les paramètres du classeur.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Obtient l'auteur du fichier. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indique s'il faut vérifier le format de nombre personnalisé lors du réglage de Style.Custom, la valeur par défaut est false. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Indique s'il faut créer une chaîne de formules calculées. |
| [getDate1904()](#getDate1904--) | Obtient une valeur qui représente si le classeur utilise le système de dates 1904. |
| [getEnableMacros()](#getEnableMacros--) | Activer les macros ; maintenant cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Indique s'il faut recalculer complètement à chaque déclenchement d'un calcul. |
| [getIteration()](#getIteration--) | Indique s'il faut utiliser l'itération pour résoudre les références circulaires. |
| [getMaxIteration()](#getMaxIteration--) | Renvoie ou définit le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Vrai si les calculs dans ce classeur seront effectués en utilisant uniquement la précision des nombres tels qu'ils sont affichés |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Indique s'il faut recalculer toutes les formules à l'ouverture du fichier. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Définit l'auteur du fichier. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Indique s'il faut vérifier le format de nombre personnalisé lors du réglage de Style.Custom, la valeur par défaut est false. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Indique s'il faut créer une chaîne de formules calculées. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Définit une valeur qui représente si le classeur utilise le système de date 1904. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Activer les macros ; maintenant cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Indique s'il faut recalculer complètement à chaque déclenchement d'un calcul. |
| [setIteration(boolean value)](#setIteration-boolean-) | Indique s'il faut utiliser l'itération pour résoudre les références circulaires. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Renvoie ou définit le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Vrai si les calculs dans ce classeur seront effectués en utilisant uniquement la précision des nombres tels qu'ils sont affichés |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Indique s'il faut recalculer toutes les formules à l'ouverture du fichier. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtient l'auteur du fichier.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Indique s'il faut vérifier le format de nombre personnalisé lors du réglage de Style.Custom, la valeur par défaut est false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple via Cell.PutValue(string), si cette propriété est true, vous obtiendrez une Exception. Si cette propriété est false, nous accepterons votre chaîne d'entrée comme valeur de la cellule, ce qui vous permettra ensuite d'exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. default is false.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Indique s'il faut créer une chaîne de formules calculées. Default is false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Obtient une valeur qui représente si le classeur utilise le système de dates 1904.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Activer les macros ; maintenant cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Indique s'il faut recalculer complètement à chaque déclenchement d'un calcul.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Indique s'il faut utiliser l'itération pour résoudre les références circulaires.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Renvoie ou définit le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Vrai si les calculs dans ce classeur seront effectués en utilisant uniquement la précision des nombres tels qu'ils sont affichés

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Indique s'il faut recalculer toutes les formules à l'ouverture du fichier. Default is true.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Définit l'auteur du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Indique s'il faut vérifier le format de nombre personnalisé lors du réglage de Style.Custom, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple via Cell.PutValue(string), si cette propriété est true, vous obtiendrez une Exception. Si cette propriété est false, nous accepterons votre chaîne d'entrée comme valeur de la cellule, ce qui vous permettra ensuite d'exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. default is false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Indique s'il faut créer une chaîne de formules calculées. Default is false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Définit une valeur qui représente si le classeur utilise le système de date 1904.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Activer les macros ; maintenant cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Indique s'il faut recalculer complètement à chaque déclenchement d'un calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Indique s'il faut utiliser l'itération pour résoudre les références circulaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Renvoie ou définit le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Vrai si les calculs dans ce classeur seront effectués en utilisant uniquement la précision des nombres tels qu'ils sont affichés

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Indique s'il faut recalculer toutes les formules à l'ouverture du fichier. Default is true.

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

