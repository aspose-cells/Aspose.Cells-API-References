---
title: "AbstractCalculationMonitor"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Surveille pour que l'utilisateur suive la progression du calcul de la formule."
type: docs
url: /fr/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

Surveille pour que l'utilisateur suive la progression du calcul de la formule.

**Example**

```
         class MyCalculationMonitor extends AbstractCalculationMonitor
         {
             public /*override*/ void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
             {
                 if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
                 {
                     return;
                 }
                 System.out.println("Cell A1 will be calculated.");
             }
         }
         Workbook wb = new Workbook("calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCalculationMonitor(new MyCalculationMonitor());
         wb.calculateFormula(opts);
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | Implémentez cette méthode pour effectuer des opérations après le calcul d'une cellule. |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | Implémentez cette méthode pour effectuer des opérations avant le calcul d'une cellule. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Obtient la nouvelle valeur calculée de la cellule. |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | Obtient l'ancienne valeur de la cellule calculée. |
| [getValueChanged()](#getValueChanged--) | Indique si la valeur de la cellule a été modifiée après le calcul. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | Implémentez cette méthode pour effectuer des opérations lors du calcul de formules avec des références circulaires. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationMonitor() {#AbstractCalculationMonitor--}
```
public AbstractCalculationMonitor()
```


### afterCalculate(int sheetIndex, int rowIndex, int colIndex) {#afterCalculate-int-int-int-}
```
public void afterCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implémentez cette méthode pour effectuer des opérations après le calcul d'une cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Index de la feuille à laquelle la cellule appartient. |
| rowIndex | int | Index de ligne de la cellule |
| colIndex | int | Indice de colonne de la cellule |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implémentez cette méthode pour effectuer des opérations avant le calcul d'une cellule.

**Remarks**

Pour les cellules dans les formules de tableau, cette méthode peut ne pas être exécutée car ces cellules sont généralement calculées ensemble.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Index de la feuille à laquelle la cellule appartient. |
| rowIndex | int | Index de ligne de la cellule |
| colIndex | int | Indice de colonne de la cellule |

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


Obtient la nouvelle valeur calculée de la cellule. Ne doit être utilisé que dans [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOriginalValue() {#getOriginalValue--}
```
public Object getOriginalValue()
```


Obtient l'ancienne valeur de la cellule calculée. Ne doit être utilisé que dans [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) et [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


Indique si la valeur de la cellule a été modifiée après le calcul. Ne doit être utilisé que dans [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

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




### onCircular(Iterator circularCellsData) {#onCircular-java.util.Iterator-}
```
public boolean onCircular(Iterator circularCellsData)
```


Implémentez cette méthode pour effectuer des opérations lors du calcul de formules avec des références circulaires.

**Remarks**

Dans l'implémentation, l'utilisateur peut également définir la valeur attendue comme résultat calculé pour une partie ou la totalité de ces cellules afin que le moteur de formules ne les calcule pas de manière récursive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | IEnumerator avec des éléments [CalculationCell](../../com.aspose.cells/calculationcell) représentant les cellules dépendant de références circulaires. |

**Returns:**
booléen - Indique si le moteur de formules doit calculer ces cellules en boucle après cet appel. True pour laisser le moteur de formules poursuivre le calcul pour elles. False pour que le moteur de formules se contente de marquer ces cellules comme Calculated.
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

