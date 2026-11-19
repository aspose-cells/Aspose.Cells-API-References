---
title: "GridWorkbookSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les paramètres du classeur."
type: docs
url: /fr/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

Représente les paramètres du classeur.

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | constructeur par défaut |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Obtient l'auteur du fichier. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Obtient si la vérification du format numérique personnalisé est activée lors du réglage de Style.Custom. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Obtient si la création d'une chaîne de formules calculées est activée. |
| [getDate1904()](#getDate1904--) | Obtient la valeur qui indique si le classeur utilise le système de date 1904. |
| [getEnableMacros()](#getEnableMacros--) | Obtient si les macros sont activées ; actuellement cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Obtient si le calcul est effectué complètement à chaque fois qu'un calcul est déclenché. |
| [getIteration()](#getIteration--) | Obtient si l'itération est utilisée pour résoudre les références circulaires. |
| [getMaxIteration()](#getMaxIteration--) | Obtient le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Vrai si les calculs dans ce classeur seront effectués en utilisant uniquement la précision des nombres tels qu'ils sont affichés |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Obtient si toutes les formules sont recalculées à l'ouverture du fichier. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Définit l'auteur du fichier. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Définit si la vérification du format numérique personnalisé est effectuée lors du réglage de Style.Custom. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Définit si la chaîne de formules calculées est créée. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Définit la valeur qui indique si le classeur utilise le système de date 1904. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Définit si les macros sont activées ; maintenant cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Définit si le calcul est effectué complètement à chaque fois qu'un calcul est déclenché. |
| [setIteration(boolean value)](#setIteration-boolean-) | Définit si l'itération est utilisée pour résoudre les références circulaires. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Définit le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Vrai si les calculs dans ce classeur seront effectués en utilisant uniquement la précision des nombres tels qu'ils sont affichés |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Définit si toutes les formules sont recalculées à l'ouverture du fichier. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


constructeur par défaut

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


Obtient si la vérification du format numérique personnalisé est activée lors du réglage de Style.Custom.

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


Obtient si la chaîne de formules calculées est créée. La valeur par défaut est false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Obtient la valeur qui indique si le classeur utilise le système de date 1904.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Obtient si les macros sont activées ; actuellement cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Obtient si le calcul est effectué complètement à chaque fois qu'un calcul est déclenché.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Obtient si l'itération est utilisée pour résoudre les références circulaires.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Obtient le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Vrai si les calculs dans ce classeur seront effectués en utilisant uniquement la précision des nombres tels qu'ils sont affichés

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Indique s'il faut conserver les espaces et les sauts de ligne qui sont remplis entre les jetons de formule lors de la lecture et de l'écriture des formules. La valeur par défaut est false.

**Remarks**

En général, ces espaces et sauts de ligne ne servent qu'à des fins visuelles. Les conserver ou non n'affecte pas le résultat calculé. Pour des considérations de performance, s'il n'y a aucune exigence particulière, il vaut mieux ne pas les conserver lors du traitement des formules.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Obtient si toutes les formules sont recalculées à l'ouverture du fichier.

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


Définit si la vérification du format numérique personnalisé est effectuée lors du réglage de Style.Custom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Définit si la chaîne de formules calculées est créée. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Définit la valeur qui indique si le classeur utilise le système de date 1904.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Définit si les macros sont activées ; maintenant cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Définit si le calcul est effectué complètement à chaque fois qu'un calcul est déclenché.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Définit si l'itération est utilisée pour résoudre les références circulaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Définit le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100.

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

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Indique s'il faut conserver les espaces et les sauts de ligne qui sont remplis entre les jetons de formule lors de la lecture et de l'écriture des formules. La valeur par défaut est false.

**Remarks**

En général, ces espaces et sauts de ligne ne servent qu'à des fins visuelles. Les conserver ou non n'affecte pas le résultat calculé. Pour des considérations de performance, s'il n'y a aucune exigence particulière, il vaut mieux ne pas les conserver lors du traitement des formules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Définit si toutes les formules sont recalculées à l'ouverture du fichier.

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

