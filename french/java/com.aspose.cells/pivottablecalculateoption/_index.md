---
title: "PivotTableCalculateOption"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de calcul des données du tableau croisé dynamique."
type: docs
url: /fr/java/com.aspose.cells/pivottablecalculateoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableCalculateOption
```

Représente les options de calcul des données du tableau croisé dynamique.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PivotTableCalculateOption()](#PivotTableCalculateOption--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRefreshCharts()](#getRefreshCharts--) | Indique si le rafraîchissement des graphiques est basé sur ce tableau croisé dynamique. |
| [getRefreshData()](#getRefreshData--) | Indique si le rafraîchissement de la source de données du tableau croisé dynamique. |
| [getRefreshOption()](#getRefreshOption--) | Obtient les options de rafraîchissement de la source de données vers le cache du tableau croisé dynamique. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Représente la façon de réserver les éléments de tableau croisé manquants. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRefreshCharts(boolean value)](#setRefreshCharts-boolean-) | Indique si le rafraîchissement des graphiques est basé sur ce tableau croisé dynamique. |
| [setRefreshData(boolean value)](#setRefreshData-boolean-) | Indique si le rafraîchissement de la source de données du tableau croisé dynamique. |
| [setRefreshOption(PivotTableRefreshOption value)](#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-) | Définit les options de rafraîchissement de la source de données vers le cache du tableau croisé dynamique. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Représente la façon de réserver les éléments de tableau croisé manquants. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableCalculateOption() {#PivotTableCalculateOption--}
```
public PivotTableCalculateOption()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRefreshCharts() {#getRefreshCharts--}
```
public boolean getRefreshCharts()
```


Indique si le rafraîchissement des graphiques est basé sur ce tableau croisé dynamique.

**Returns:**
boolean
### getRefreshData() {#getRefreshData--}
```
public boolean getRefreshData()
```


Indique si le rafraîchissement de la source de données du tableau croisé dynamique.

**Remarks**

Si c'est vrai, rafraîchit le cache du tableau croisé dynamique à partir de la source de données, puis calcule tous les tableaux croisés dynamiques basés sur le même cache.

**Returns:**
boolean
### getRefreshOption() {#getRefreshOption--}
```
public PivotTableRefreshOption getRefreshOption()
```


Obtient les options de rafraîchissement de la source de données vers le cache du tableau croisé dynamique.

**Returns:**
[PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption)
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Représente la façon de réserver les éléments de tableau croisé manquants.

Voir [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Fonctionne uniquement lorsque [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\\#getRefreshData--) est vrai.

**Returns:**
int
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




### setRefreshCharts(boolean value) {#setRefreshCharts-boolean-}
```
public void setRefreshCharts(boolean value)
```


Indique si le rafraîchissement des graphiques est basé sur ce tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRefreshData(boolean value) {#setRefreshData-boolean-}
```
public void setRefreshData(boolean value)
```


Indique si le rafraîchissement de la source de données du tableau croisé dynamique.

**Remarks**

Si c'est vrai, rafraîchit le cache du tableau croisé dynamique à partir de la source de données, puis calcule tous les tableaux croisés dynamiques basés sur le même cache.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRefreshOption(PivotTableRefreshOption value) {#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-}
```
public void setRefreshOption(PivotTableRefreshOption value)
```


Définit les options de rafraîchissement de la source de données vers le cache du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Représente la façon de réserver les éléments de tableau croisé manquants.

Voir [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Fonctionne uniquement lorsque [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\\#getRefreshData--) est vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

