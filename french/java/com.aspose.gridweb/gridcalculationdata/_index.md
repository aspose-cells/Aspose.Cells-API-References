---
title: "GridCalculationData"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les données requises lors du calcul d'une fonction, telles que les paramètres du nom de fonction ...etc."
type: docs
url: /fr/java/com.aspose.gridweb/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Représente les données requises lors du calcul d'une fonction, telles que le nom de la fonction, les paramètres, …etc.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Obtient la valeur calculée pour cette fonction. |
| [getCell()](#getCell--) | Obtient l'objet Cell où se trouve la fonction. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Obtient le nom de la fonction à calculer. |
| [getParamCount()](#getParamCount--) | Obtient le nombre de paramètres |
| [getParamText(int index)](#getParamText-int-) | Obtient le texte littéral du paramètre à l'index donné. |
| [getParamValue(int index)](#getParamValue-int-) | Obtient l'objet valeur représentée du paramètre à l'index donné. |
| [getWorkbook()](#getWorkbook--) | Obtient l'objet Workbook où se trouve la fonction. |
| [getWorksheet()](#getWorksheet--) | Obtient l'objet Workbook où se trouve la fonction. |
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
### getCell() {#getCell--}
```
public GridCell getCell()
```


Obtient l'objet Cell où se trouve la fonction.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
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


Obtient l'objet valeur représentée du paramètre à l'index donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | index du paramètre (base 0) |

**Returns:**
java.lang.Object - Si le paramètre est une valeur simple, alors renvoie la valeur simple. Si le paramètre est une référence, alors renvoie l'objet ReferredArea.
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Obtient l'objet Workbook où se trouve la fonction.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getWorksheet() {#getWorksheet--}
```
public GridWorksheet getWorksheet()
```


Obtient l'objet Workbook où se trouve la fonction.

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
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

