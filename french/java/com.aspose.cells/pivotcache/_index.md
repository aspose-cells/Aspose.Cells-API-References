---
title: "PivotCache"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le cache mémoire pour certains rapports de tableau croisé dynamique."
type: docs
url: /fr/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

Représente le cache mémoire pour certains rapports de tableau croisé dynamique.

**Remarks**

Toutes les données seront rassemblées dans ce cache, et le tableau croisé dynamique ne récupère les données que depuis ce cache, sans accéder directement à la source de données. Si la source de données de certains [PivotTable](../../com.aspose.cells/pivottable)s est la même, ils utiliseront un cache de tableau croisé dynamique.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [dispose()](#dispose--) | Libérer toutes les ressources. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Obtient le nombre d'éléments inutilisés à autoriser avant de supprimer les éléments inutilisés. |
| [getPivotTables()](#getPivotTables--) | Obtient tous les tableaux croisés dynamiques avec ce cache de tableau croisé dynamique. |
| [getSourceType()](#getSourceType--) | Obtient le [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Actualise les données depuis la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de tableau croisé dynamique. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Actualise les données depuis la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de tableau croisé dynamique. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Définit le nombre d'éléments inutilisés à autoriser avant de supprimer les éléments inutilisés. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotCache() {#PivotCache--}
```
public PivotCache()
```


### dispose() {#dispose--}
```
public abstract void dispose()
```


Libérer toutes les ressources.

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
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Obtient le nombre d'éléments inutilisés à autoriser avant de supprimer les éléments inutilisés. Cette valeur DOIT être supérieure à -2 et inférieure à 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


Obtient tous les tableaux croisés dynamiques avec ce cache de tableau croisé dynamique.

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


Obtient le [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

Voir [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
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




### refresh() {#refresh--}
```
public int refresh()
```


Actualise les données depuis la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de tableau croisé dynamique.

**Remarks**

Si table1 et table2 utilisent tous deux ce cache, les deux tableaux seront calculés. Il est préférable d'appeler simplement [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) pour actualiser tous les tableaux croisés dynamiques et graphiques du fichier.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Actualise les données depuis la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de tableau croisé dynamique.

**Remarks**

Il est préférable que vous puissiez simplement appeler [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) pour actualiser tous les tableaux croisés dynamiques et graphiques du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Les options pour actualiser la source de données du tableau croisé dynamique. |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Définit le nombre d'éléments inutilisés à autoriser avant de supprimer les éléments inutilisés. Cette valeur DOIT être supérieure à -2 et inférieure à 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

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

