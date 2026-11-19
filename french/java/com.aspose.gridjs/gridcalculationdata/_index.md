---
title: "GridCalculationData"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les données requises lors du calcul d'une fonction, telles que les paramètres du nom de fonction ...etc."
type: docs
url: /fr/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Représente les données requises lors du calcul d'une fonction, telles que le nom de la fonction, les paramètres, …etc.

**Remarks**

Tous les objets fournis par cette classe sont uniquement destinés à la "lecture". L'utilisateur ne doit pas modifier les données du classeur pendant le processus de calcul de formule, sinon un résultat inattendu ou une exception peut survenir.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Obtient la valeur calculée pour cette fonction. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient l'index de la colonne Cell Column où la fonction se trouve. |
| [getFormula()](#getFormula--) | Obtient la formule Cell où la fonction se trouve. |
| [getFunctionName()](#getFunctionName--) | Obtient le nom de la fonction à calculer. |
| [getParamCount()](#getParamCount--) | Obtient le nombre de paramètres. |
| [getParamText(int index)](#getParamText-int-) | Obtient le texte littéral du paramètre à l'index donné. |
| [getParamValue(int index)](#getParamValue-int-) | Obtient l'objet valeur représentée du paramètre à l'index donné. |
| [getRow()](#getRow--) | Obtient l'index de la ligne Cell Row où la fonction se trouve. |
| [getSheetName()](#getSheetName--) | Obtient le nom de la feuille de calcul où la fonction se trouve. |
| [getStringValue()](#getStringValue--) | Obtient la valeur d'affichage Cell DisplayStringValue où la fonction se trouve. |
| [getValue()](#getValue--) | Obtient la valeur Cell où la fonction se trouve. |
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

L'utilisateur doit définir cette propriété dans son moteur de calcul personnalisé pour les fonctions prises en charge par le moteur, et la valeur définie sera renvoyée lors de la lecture de cette propriété. Lire cette propriété avant de la définir fera calculer la fonction par le moteur de calcul par défaut d'Aspose.Cells et la valeur calculée sera renvoyée.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtient l'index de la colonne Cell Column où la fonction se trouve.

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtient la formule Cell où la fonction se trouve.

**Returns:**
java.lang.String
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


Obtient le nombre de paramètres.

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
| index | int | L'index du paramètre (base 0). |

**Returns:**
java.lang.String - Le texte littéral du paramètre.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Obtient l'objet valeur représentée du paramètre à l'index donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index du paramètre (base 0). |

**Returns:**
java.lang.Object - Si le paramètre est une valeur simple, alors renvoie la valeur simple. Si le paramètre est une référence, alors renvoie l'objet ReferredArea.
### getRow() {#getRow--}
```
public int getRow()
```


Obtient l'index de la ligne Cell Row où la fonction se trouve.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Obtient le nom de la feuille de calcul où la fonction se trouve.

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Obtient la valeur d'affichage Cell DisplayStringValue où la fonction se trouve.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Obtient la valeur Cell où la fonction se trouve.

**Returns:**
java.lang.Object
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

L'utilisateur doit définir cette propriété dans son moteur de calcul personnalisé pour les fonctions prises en charge par le moteur, et la valeur définie sera renvoyée lors de la lecture de cette propriété. Lire cette propriété avant de la définir fera calculer la fonction par le moteur de calcul par défaut d'Aspose.Cells et la valeur calculée sera renvoyée.

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

