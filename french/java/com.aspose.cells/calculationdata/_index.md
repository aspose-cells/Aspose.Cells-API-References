---
title: "CalculationData"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les données requises lors du calcul d'une fonction, telles que les paramètres du nom de fonction ...etc."
type: docs
url: /fr/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

Représente les données requises lors du calcul d'une fonction, telles que le nom de la fonction, les paramètres, …etc.

**Remarks**

Tous les objets fournis par cette classe sont uniquement destinés à la "lecture". L'utilisateur ne doit pas modifier les données du classeur pendant le processus de calcul de formule, sinon un résultat inattendu ou une exception peut survenir.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Obtient la valeur calculée pour cette fonction. |
| [getCell()](#getCell--) | Obtient l'objet Cell où se trouve la fonction. |
| [getCellColumn()](#getCellColumn--) | Obtient l'index de colonne de la cellule où se trouve la fonction. |
| [getCellRow()](#getCellRow--) | Obtient l'index de ligne de la cellule où se trouve la fonction. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Obtient le nom de la fonction à calculer. |
| [getParamCount()](#getParamCount--) | Obtient le nombre de paramètres |
| [getParamText(int index)](#getParamText-int-) | Obtient le texte littéral du paramètre à l'index donné. |
| [getParamValue(int index)](#getParamValue-int-) | Obtient l'objet valeur représenté du paramètre à un index donné. |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | Obtient la/les valeur(s) du paramètre à un index donné. |
| [getWorkbook()](#getWorkbook--) | Obtient l'objet Workbook où se trouve la fonction. |
| [getWorksheet()](#getWorksheet--) | Obtient l'objet Worksheet où se trouve la fonction. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Définit la valeur calculée pour cette fonction. |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Obtient la valeur calculée pour cette fonction.

**Remarks**

L'utilisateur doit définir cette propriété dans son moteur de calcul personnalisé pour les fonctions que le moteur prend en charge, et la valeur définie sera renvoyée lors de la lecture de cette propriété ultérieurement. La valeur définie peut être de types possibles de [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), ou un tableau de ce type de valeurs, ou un Range, Name, ReferredArea. Lire cette propriété avant d'y affecter une valeur entraînera le calcul de la fonction par le moteur de calcul par défaut d'Aspose.Cells, puis la valeur calculée sera renvoyée (généralement cela devrait être \#NAME? pour les fonctions définies par l'utilisateur).

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


Obtient l'objet Cell où se trouve la fonction.

**Remarks**

Lors du calcul d'une formule sans l'affecter à une cellule, par exemple via [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-), la formule sera calculée comme si elle avait été placée dans la cellule A1, de sorte que [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) et [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) sont tous deux à 0. Cependant, la cellule A1 de la feuille de calcul peut ne pas avoir été instanciée. Ainsi, dans ce type de situation, cette propriété sera nulle.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Obtient l'index de colonne de la cellule où se trouve la fonction.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Obtient l'index de ligne de la cellule où se trouve la fonction.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


Obtient le nom de la fonction à calculer.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


Obtient le nombre de paramètres

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Obtient le texte littéral du paramètre à l'index donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | index du paramètre (base 0) |

**Returns:**
java.lang.String - texte littéral du paramètre
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Obtient l'objet valeur représenté du paramètre à un index donné.

**Remarks**

Pour un paramètre :

Si c'est une valeur simple, alors renvoie la valeur simple elle-même ;

Si c'est une référence, alors renvoie l'objet ReferredArea ;

Si elle fait référence à un ou plusieurs jeux de données contenant plusieurs valeurs, alors renvoie un tableau d'objets ;

Si c'est une sorte d'expression qui doit être calculée, elle sera calculée en mode valeur et, généralement, une seule valeur sera renvoyée en fonction de la cellule de base actuelle. Par exemple, si un paramètre de la formule de D2 est A:A+B:B, alors A2+B2 sera calculé et renvoyé. Cependant, si ce paramètre a été spécifié en mode tableau (par  ou ), alors un tableau (object[][]) sera renvoyé dont les éléments sont A1+B1, A2+B2, ….

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index du paramètre (base 0) |

**Returns:**
java.lang.Object - La valeur calculée du paramètre.
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


Obtient la/les valeur(s) du paramètre à un index donné. Si le paramètre est une sorte d'expression qui doit être calculée, alors il sera calculé en mode tableau.

**Remarks**

Pour une expression qui doit être calculée, en prenant A:A+B:B comme exemple : en mode valeur, elle sera calculée en une seule valeur selon la cellule de base actuelle. Mais en mode tableau, toutes les valeurs de A1+B1, A2+B2, A3+B3, … seront calculées et utilisées pour construire le tableau renvoyé. Dans ce type de situation, il est préférable de spécifier la limite du nombre de lignes/colonnes (par exemple selon [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) et [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--)), sinon le grand tableau renvoyé peut augmenter la consommation de mémoire avec une grande quantité de données inutiles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index du paramètre (base 0) |
| maxRowCount | int | La limite du nombre de lignes pour le tableau renvoyé. Si elle est non positive ou supérieure au nombre réel de lignes, alors le nombre réel de lignes sera utilisé. |
| maxColumnCount | int | La limite du nombre de colonnes pour le tableau renvoyé. Si elle est non positive ou supérieure au nombre réel de lignes, alors le nombre réel de colonnes sera utilisé. |

**Returns:**
java.lang.Object[][] - Un tableau qui contient tous les éléments représentés par le paramètre spécifié.
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtient l'objet Workbook où se trouve la fonction.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtient l'objet Worksheet où se trouve la fonction.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


Définit la valeur calculée pour cette fonction.

**Remarks**

L'utilisateur doit définir cette propriété dans son moteur de calcul personnalisé pour les fonctions que le moteur prend en charge, et la valeur définie sera renvoyée lors de la lecture de cette propriété ultérieurement. La valeur définie peut être de types possibles de [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), ou un tableau de ce type de valeurs, ou un Range, Name, ReferredArea. Lire cette propriété avant d'y affecter une valeur entraînera le calcul de la fonction par le moteur de calcul par défaut d'Aspose.Cells, puis la valeur calculée sera renvoyée (généralement cela devrait être \#NAME? pour les fonctions définies par l'utilisateur).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

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

