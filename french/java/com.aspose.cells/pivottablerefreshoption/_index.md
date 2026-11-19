---
title: "PivotTableRefreshOption"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'actualisation de la source de données du tableau croisé dynamique."
type: docs
url: /fr/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

Représente les options d'actualisation de la source de données du tableau croisé dynamique.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | Représente les options d'actualisation de la source de données du tableau croisé dynamique. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | Indique s’il faut conserver les données de groupe locales en cache si les valeurs maximale et minimale restent inchangées. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Représente la façon de réserver les éléments de tableau croisé manquants. |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | Indique s’il faut conserver l’ordre original des éléments du tableau croisé tel que dans l’ancienne source de données. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | Indique s’il faut conserver les données de groupe locales en cache si les valeurs maximale et minimale restent inchangées. |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | Indique s’il faut conserver l’ordre original des éléments du tableau croisé tel que dans l’ancienne source de données. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Représente la façon de réserver les éléments de tableau croisé manquants. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


Représente les options d'actualisation de la source de données du tableau croisé dynamique.

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


Indique s’il faut conserver les données de groupe locales en cache si les valeurs maximale et minimale restent inchangées. La valeur par défaut est false, ce qui signifie que le groupe est rafraîchi avec le paramètre local.

**Remarks**

Ceci est une solution temporaire, veuillez localiser les tableaux croisés en implémentant [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Représente la façon de réserver les éléments de tableau croisé manquants.

Voir [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isKeepOriginalOrder() {#isKeepOriginalOrder--}
```
public boolean isKeepOriginalOrder()
```


Indique s’il faut conserver l’ordre original des éléments du tableau croisé tel que dans l’ancienne source de données.

**Remarks**

Applicable uniquement aux champs de tableau croisé qui ne sont pas triés. Lors du rafraîchissement d’un tel champ, Ms Excel conserve l’ordre original de l’ancienne source de données. La valeur par défaut de cette propriété est true, ce qui représente le même comportement que Ms Excel. Si l’utilisateur souhaite que le champ de tableau croisé soit entièrement rafraîchi comme les données de la nouvelle source, cette propriété doit être définie sur false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setKeepCachedLocalGroupData(boolean value) {#setKeepCachedLocalGroupData-boolean-}
```
public void setKeepCachedLocalGroupData(boolean value)
```


Indique s’il faut conserver les données de groupe locales en cache si les valeurs maximale et minimale restent inchangées. La valeur par défaut est false, ce qui signifie que le groupe est rafraîchi avec le paramètre local.

**Remarks**

Ceci est une solution temporaire, veuillez localiser les tableaux croisés en implémentant [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


Indique s’il faut conserver l’ordre original des éléments du tableau croisé tel que dans l’ancienne source de données.

**Remarks**

Applicable uniquement aux champs de tableau croisé qui ne sont pas triés. Lors du rafraîchissement d’un tel champ, Ms Excel conserve l’ordre original de l’ancienne source de données. La valeur par défaut de cette propriété est true, ce qui représente le même comportement que Ms Excel. Si l’utilisateur souhaite que le champ de tableau croisé soit entièrement rafraîchi comme les données de la nouvelle source, cette propriété doit être définie sur false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Représente la façon de réserver les éléments de tableau croisé manquants.

Voir [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

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

