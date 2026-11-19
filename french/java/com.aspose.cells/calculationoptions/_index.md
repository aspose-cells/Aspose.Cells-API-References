---
title: "CalculationOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de calcul."
type: docs
url: /fr/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Représente les options de calcul.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | La taille de la pile pour le calcul récursif des cellules. |
| [getCalculationMonitor()](#getCalculationMonitor--) | Le moniteur permettant à l'utilisateur de suivre la progression du calcul des formules. |
| [getCharacterEncoding()](#getCharacterEncoding--) | Spécifie l'encodage utilisé pour l'encodage/décodage des caractères lors du calcul des formules. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [getIgnoreError()](#getIgnoreError--) | Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Spécifie les sources de données pour les liens externes utilisés dans les formules. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Spécifie la stratégie de traitement de la précision du calcul. |
| [getRecursive()](#getRecursive--) | Indique s'il faut calculer les cellules dépendantes de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | Indique si les formules de tableau dynamique doivent être actualisées avant le calcul des formules. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | Indique si l'utilisateur a explicitement spécifié le comportement d'actualisation des formules de tableau dynamique avant le calcul des formules spécifiées. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | La taille de la pile pour le calcul récursif des cellules. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | Le moniteur permettant à l'utilisateur de suivre la progression du calcul des formules. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | Spécifie l'encodage utilisé pour l'encodage/décodage des caractères lors du calcul des formules. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Spécifie les sources de données pour les liens externes utilisés dans les formules. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Spécifie la stratégie de traitement de la précision du calcul. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Indique s'il faut calculer les cellules dépendantes de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | Indique si les formules de tableau dynamique doivent être actualisées avant le calcul des formules. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CalculationOptions() {#CalculationOptions--}
```
public CalculationOptions()
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
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


La taille de la pile pour le calcul récursif des cellules. La valeur par défaut est 200.

**Remarks**

Lorsque un grand nombre de cellules doivent être calculées de manière récursive dans l'arbre de dépendances, une StackOverflowException peut être déclenchée pendant le processus de calcul. Dans ce cas, l'utilisateur doit spécifier une valeur plus petite pour cette propriété. Pour une telle situation, l'utilisateur doit déterminer la valeur appropriée pour cette propriété en fonction des formules et des données réelles. Cependant, une valeur trop petite peut entraîner une dégradation des performances du calcul des formules et une valeur inférieure à 2 rendra impossible le calcul d'une formule qui dépend d'une autre. Ainsi, si la valeur spécifiée est inférieure à 2, elle sera réinitialisée à 2.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


Le moniteur permettant à l'utilisateur de suivre la progression du calcul des formules.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


Spécifie l'encodage utilisé pour l'encodage/décodage des caractères lors du calcul des formules. Pour des fonctions telles que CHAR, CODE, le résultat calculé dépend des paramètres régionaux et du jeu de caractères par défaut de l'environnement. Avec cette propriété, l'utilisateur peut spécifier l'encodage approprié utilisé pour ces fonctions afin d'obtenir le résultat attendu.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomEngine() {#getCustomEngine--}
```
public AbstractCalculationEngine getCustomEngine()
```


Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées. L'erreur peut être une fonction non prise en charge, des liens externes, etc. La valeur par défaut est true.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


Spécifie les sources de données pour les liens externes utilisés dans les formules.

**Remarks**

Comme [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), vous pouvez spécifier ici les sources de données pour les liens externes utilisés dans les formules à calculer, en particulier ceux utilisés dans la fonction INDIRECT. Pour ces liens externes utilisés dans la fonction INDIRECT, ils ne sont pas considérés comme faisant partie des liens externes du classeur et ne peuvent pas être mis à jour par [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). La correspondance de ces classeurs avec les liens externes est déterminée par [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) et [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Veuillez donc vous assurer que [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) a été spécifié avec la valeur appropriée (généralement elle doit être identique à la [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) correspondante) pour chaque classeur afin qu'ils puissent être liés comme prévu.

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


Spécifie la stratégie de traitement de la précision du calcul.

Voir [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Indique s'il faut calculer les cellules dépendantes de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules. La valeur par défaut est true.

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


Indique si les formules de tableau dynamique doivent être actualisées avant le calcul des formules.

**Remarks**

Si cette propriété a été spécifiée explicitement, la valeur spécifiée sera utilisée pour déterminer s'il faut rafraîchir les formules de tableau dynamique. Sinon ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) est false), la valeur par défaut dépend du type de formules à calculer : pour le calcul des formules du classeur, comme [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), cette propriété sera considérée comme true. Dans les autres cas, comme [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) ou [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), cette propriété sera considérée comme false.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


Indique si l'utilisateur a explicitement spécifié le comportement d'actualisation des formules de tableau dynamique avant le calcul des formules spécifiées.

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




### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


La taille de la pile pour le calcul récursif des cellules. La valeur par défaut est 200.

**Remarks**

Lorsque un grand nombre de cellules doivent être calculées de manière récursive dans l'arbre de dépendances, une StackOverflowException peut être déclenchée pendant le processus de calcul. Dans ce cas, l'utilisateur doit spécifier une valeur plus petite pour cette propriété. Pour une telle situation, l'utilisateur doit déterminer la valeur appropriée pour cette propriété en fonction des formules et des données réelles. Cependant, une valeur trop petite peut entraîner une dégradation des performances du calcul des formules et une valeur inférieure à 2 rendra impossible le calcul d'une formule qui dépend d'une autre. Ainsi, si la valeur spécifiée est inférieure à 2, elle sera réinitialisée à 2.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


Le moniteur permettant à l'utilisateur de suivre la progression du calcul des formules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


Spécifie l'encodage utilisé pour l'encodage/décodage des caractères lors du calcul des formules. Pour des fonctions telles que CHAR, CODE, le résultat calculé dépend des paramètres régionaux et du jeu de caractères par défaut de l'environnement. Avec cette propriété, l'utilisateur peut spécifier l'encodage approprié utilisé pour ces fonctions afin d'obtenir le résultat attendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


Le moteur de calcul de formules personnalisé pour étendre le moteur de calcul par défaut d'Aspose.Cells.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées. L'erreur peut être une fonction non prise en charge, des liens externes, etc. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


Spécifie les sources de données pour les liens externes utilisés dans les formules.

**Remarks**

Comme [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), vous pouvez spécifier ici les sources de données pour les liens externes utilisés dans les formules à calculer, en particulier ceux utilisés dans la fonction INDIRECT. Pour ces liens externes utilisés dans la fonction INDIRECT, ils ne sont pas considérés comme faisant partie des liens externes du classeur et ne peuvent pas être mis à jour par [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). La correspondance de ces classeurs avec les liens externes est déterminée par [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) et [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Veuillez donc vous assurer que [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) a été spécifié avec la valeur appropriée (généralement elle doit être identique à la [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) correspondante) pour chaque classeur afin qu'ils puissent être liés comme prévu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Spécifie la stratégie de traitement de la précision du calcul.

Voir [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Indique s'il faut calculer les cellules dépendantes de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


Indique si les formules de tableau dynamique doivent être actualisées avant le calcul des formules.

**Remarks**

Si cette propriété a été spécifiée explicitement, la valeur spécifiée sera utilisée pour déterminer s'il faut rafraîchir les formules de tableau dynamique. Sinon ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) est false), la valeur par défaut dépend du type de formules à calculer : pour le calcul des formules du classeur, comme [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), cette propriété sera considérée comme true. Dans les autres cas, comme [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) ou [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), cette propriété sera considérée comme false.

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

