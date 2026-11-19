---
title: "GridAbstractCalculationEngine"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells."
type: docs
url: /fr/java/com.aspose.gridweb/gridabstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```

Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells.

**Example**

```
          class MyEngine extends GridAbstractCalculationEngine
         {
             public /*override*/ void calculate(GridCalculationData data)
             {
                 String funcName = data.getFunctionName().toUpperCase();
                 if ("MYFUNC".equals(funcName))
                 {
                     //do calculation for MYFUNC here
                     int count = data.getParamCount();
                     Object res = null;
                     for (int i = 0; i <count; i++)
                     {
                         Object pv = data.getParamValue(i);
                         if (pv instanceof GridReferredArea)
                         {
                             GridReferredArea ra = (GridReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridweb.GridCalculationData-) | Calcule une fonction avec les données fournies. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridAbstractCalculationEngine() {#GridAbstractCalculationEngine--}
```
public GridAbstractCalculationEngine()
```


### calculate(GridCalculationData data) {#calculate-com.aspose.gridweb.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```


Calcule une fonction avec les données fournies.

**Remarks**

L'utilisateur doit définir la valeur calculée pour les données données pour toutes les fonctions (y compris les fonctions natives d'Excel) qu'il souhaite calculer lui‑même dans cette implémentation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridweb/gridcalculationdata) | les données requises pour calculer la fonction telles que le nom de la fonction, les paramètres, ...etc. |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

