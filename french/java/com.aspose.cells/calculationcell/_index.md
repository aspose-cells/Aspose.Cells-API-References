---
title: "CalculationCell"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les données pertinentes du calcul concernant une cellule en cours de calcul."
type: docs
url: /fr/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

Représente les données pertinentes du calcul concernant une cellule en cours de calcul.

**Remarks**

L'utilisateur ne doit pas modifier les données du classeur pendant le processus de calcul des formules, sinon un résultat inattendu ou une exception peut survenir. Ainsi, tous les objets fournis par cette classe (comme l'objet Cell de [getCell()](../../com.aspose.cells/calculationcell\#getCell--)) sont destinés uniquement à la lecture.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Obtient l'objet Cell qui est en cours de calcul. |
| [getCellColumn()](#getCellColumn--) | Obtient l'index de colonne de la cellule. |
| [getCellRow()](#getCellRow--) | Obtient l'index de ligne de la cellule. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | Obtient l'objet Workbook. |
| [getWorksheet()](#getWorksheet--) | Obtient l'objet Worksheet où se trouve la cellule. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | Définit la valeur calculée pour la cellule. |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


Obtient l'objet Cell qui est en cours de calcul.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Obtient l'index de colonne de la cellule.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Obtient l'index de ligne de la cellule.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtient l'objet Workbook.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtient l'objet Worksheet où se trouve la cellule.

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




### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```


Définit la valeur calculée pour la cellule.

**Remarks**

L'utilisateur peut définir le résultat calculé avec cette méthode pour ignorer le calcul automatique de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| v | java.lang.Object |  |

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

