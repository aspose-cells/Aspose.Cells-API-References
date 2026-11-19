---
title: "FormulaSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Paramètres des formules et du calcul."
type: docs
url: /fr/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

Paramètres des formules et du calcul.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | Indique si l'application doit effectuer un calcul complet lorsque le classeur est ouvert. |
| [getCalculateOnSave()](#getCalculateOnSave--) | Indique s'il faut recalculer le classeur avant d'enregistrer le document, lorsqu'il est en mode de calcul manuel. |
| [getCalculationId()](#getCalculationId--) | Spécifie la version du moteur de calcul utilisé pour calculer les valeurs dans le classeur. |
| [getCalculationMode()](#getCalculationMode--) | Obtient le mode de calcul du classeur dans MS Excel. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | Indique s'il faut activer la chaîne de calcul pour les formules. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | Indique s'il faut activer le calcul itératif pour résoudre les références circulaires. |
| [getForceFullCalculation()](#getForceFullCalculation--) | Indique s'il calcule toutes les formules à chaque déclenchement d'un calcul. |
| [getMaxChange()](#getMaxChange--) | Le changement maximal pour résoudre une référence circulaire. |
| [getMaxIteration()](#getMaxIteration--) | Le nombre maximal d'itérations pour résoudre une référence circulaire. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Indique s'il faut conserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de la récupération et de la définition des formules. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | Indique si l'application doit effectuer un calcul complet lorsque le classeur est ouvert. |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | Indique s'il faut recalculer le classeur avant d'enregistrer le document, lorsqu'il est en mode de calcul manuel. |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | Spécifie la version du moteur de calcul utilisé pour calculer les valeurs dans le classeur. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Définit le mode de calcul du classeur dans MS Excel. |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | Indique s'il faut activer la chaîne de calcul pour les formules. |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | Indique s'il faut activer le calcul itératif pour résoudre les références circulaires. |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | Indique s'il calcule toutes les formules à chaque déclenchement d'un calcul. |
| [setMaxChange(double value)](#setMaxChange-double-) | Le changement maximal pour résoudre une référence circulaire. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Le nombre maximal d'itérations pour résoudre une référence circulaire. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Indique s'il faut conserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de la récupération et de la définition des formules. |
| [toString()](#toString--) |  |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


Indique si l'application doit effectuer un calcul complet lorsque le classeur est ouvert.

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement du fichier résultant. Pour des considérations de performances pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quelle que soit la valeur définie pour cette propriété.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


Indique s'il faut recalculer le classeur avant d'enregistrer le document, lorsqu'il est en mode de calcul manuel.

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des considérations de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit la valeur définie pour cette propriété.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Spécifie la version du moteur de calcul utilisé pour calculer les valeurs dans le classeur.

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Dans le cas de MS Excel, si la valeur de cette propriété est inférieure à l'identifiant du moteur de recalcul associé à l'application qui ouvre le fichier résultant, l'application recalculera les résultats de toutes les formules de ce classeur immédiatement après le chargement du fichier. Pour des considérations de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit la valeur définie pour cette propriété.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


Obtient le mode de calcul du classeur dans MS Excel.

Voir [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des considérations de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit le mode défini pour cette propriété. Si l'utilisateur a besoin de calculer des formules, veuillez toujours appeler les méthodes sur les différents objets selon les besoins : [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableCalculationChain() {#getEnableCalculationChain--}
```
public boolean getEnableCalculationChain()
```


Indique si la chaîne de calcul pour les formules doit être activée. La valeur par défaut est false.

**Remarks**

Lorsque le classeur contient de nombreuses formules et que l'utilisateur doit les recalculer de façon répétée en ne modifiant qu'une petite partie d'entre elles, activer la chaîne de calcul peut être bénéfique pour les performances. En revanche, si la chaîne est activée, le maintien du modèle de chaîne nécessite plus de mémoire et requiert également un peu plus de temps CPU pour certaines autres opérations, comme la modification de la valeur ou des formules d'une cellule. Après avoir changé cette propriété de false à true, la chaîne de calcul sera analysée et construite lors du premier calcul du classeur, de sorte que le temps requis pour le premier calcul peut être supérieur à un calcul normal sans chaîne.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


Indique s'il faut activer le calcul itératif pour résoudre les références circulaires.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


Indique s'il calcule toutes les formules à chaque déclenchement d'un calcul.

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des considérations de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit la valeur définie pour cette propriété.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


Le changement maximal pour résoudre une référence circulaire.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Le nombre maximal d'itérations pour résoudre une référence circulaire.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Indique si les espaces et sauts de ligne insérés entre les jetons de formule lors de la récupération et de la définition des formules doivent être conservés. La valeur par défaut est false.

**Remarks**

En général, ces espaces et sauts de ligne ne servent qu'à des fins visuelles. Les conserver ou non n'affecte pas le résultat calculé. Pour des considérations de performance, s'il n'y a aucune exigence particulière, il vaut mieux ne pas les conserver lors du traitement des formules.

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




### setCalculateOnOpen(boolean value) {#setCalculateOnOpen-boolean-}
```
public void setCalculateOnOpen(boolean value)
```


Indique si l'application doit effectuer un calcul complet lorsque le classeur est ouvert.

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement du fichier résultant. Pour des considérations de performances pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quelle que soit la valeur définie pour cette propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


Indique s'il faut recalculer le classeur avant d'enregistrer le document, lorsqu'il est en mode de calcul manuel.

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des considérations de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit la valeur définie pour cette propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


Spécifie la version du moteur de calcul utilisé pour calculer les valeurs dans le classeur.

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Dans le cas de MS Excel, si la valeur de cette propriété est inférieure à l'identifiant du moteur de recalcul associé à l'application qui ouvre le fichier résultant, l'application recalculera les résultats de toutes les formules de ce classeur immédiatement après le chargement du fichier. Pour des considérations de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit la valeur définie pour cette propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


Définit le mode de calcul du classeur dans MS Excel.

Voir [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des considérations de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit le mode défini pour cette propriété. Si l'utilisateur a besoin de calculer des formules, veuillez toujours appeler les méthodes sur les différents objets selon les besoins : [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


Indique si la chaîne de calcul pour les formules doit être activée. La valeur par défaut est false.

**Remarks**

Lorsque le classeur contient de nombreuses formules et que l'utilisateur doit les recalculer de façon répétée en ne modifiant qu'une petite partie d'entre elles, activer la chaîne de calcul peut être bénéfique pour les performances. En revanche, si la chaîne est activée, le maintien du modèle de chaîne nécessite plus de mémoire et requiert également un peu plus de temps CPU pour certaines autres opérations, comme la modification de la valeur ou des formules d'une cellule. Après avoir changé cette propriété de false à true, la chaîne de calcul sera analysée et construite lors du premier calcul du classeur, de sorte que le temps requis pour le premier calcul peut être supérieur à un calcul normal sans chaîne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


Indique s'il faut activer le calcul itératif pour résoudre les références circulaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


Indique s'il calcule toutes les formules à chaque déclenchement d'un calcul.

**Remarks**

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des considérations de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit la valeur définie pour cette propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


Le changement maximal pour résoudre une référence circulaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Le nombre maximal d'itérations pour résoudre une référence circulaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Indique si les espaces et sauts de ligne insérés entre les jetons de formule lors de la récupération et de la définition des formules doivent être conservés. La valeur par défaut est false.

**Remarks**

En général, ces espaces et sauts de ligne ne servent qu'à des fins visuelles. Les conserver ou non n'affecte pas le résultat calculé. Pour des considérations de performance, s'il n'y a aucune exigence particulière, il vaut mieux ne pas les conserver lors du traitement des formules.

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

