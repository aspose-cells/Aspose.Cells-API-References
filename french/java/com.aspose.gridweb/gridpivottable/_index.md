---
title: "GridPivotTable"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un rapport PivotTable sur une feuille de calcul."
type: docs
url: /fr/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

Représente un rapport PivotTable sur une feuille de calcul. L'objet PivotTable est un membre de la collection [GridPivotTable](../../com.aspose.gridweb/gridpivottable). La collection PivotTables contient tous les objets PivotTable d'un contrôle.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Ajoute le champ à la zone spécifique. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Ajoute le champ à la zone spécifique. |
| [calculateData()](#calculateData--) | Calcule les données du pivottable dans les cellules. |
| [clearAllFields()](#clearAllFields--) | efface tous les champs pivot. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Obtient les champs spécifiques par type de champ. |
| [fields(String fieldName)](#fields-java.lang.String-) | Obtient le champ spécifique par son nom. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | Actualise les données et les paramètres du pivottable à partir de sa source de données. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Ajoute le champ à la zone spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Le type de zone des champs. |
| baseFieldIndex | int | L'index du champ dans les champs de base. |

**Returns:**
int - La position du champ dans les champs spécifiques.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Ajoute le champ à la zone spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Le type de zone des champs. |
| fieldName | java.lang.String | Le nom dans les champs de base. |

**Returns:**
int - La position du champ dans les champs spécifiques. Si aucun champ ne porte ce nom, retourner -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Calcule les données du pivottable dans les cellules.

**Remarks**

Cell.Value dans la plage pivot ne peut pas renvoyer le résultat correct si la méthode n'a pas été appelée. Cette méthode calcule les données avec un cache pivot interne, pas la source de données originale. Ainsi, si la source de données est modifiée, veuillez appeler la méthode RefreshData() en premier.

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


efface tous les champs pivot.

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


Obtient les champs spécifiques par type de champ.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). le type de champ. |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


Obtient le champ spécifique par son nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | le nom du champ. |

**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
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




### refreshData() {#refreshData--}
```
public void refreshData()
```


Actualise les données et les paramètres du pivottable à partir de sa source de données.

**Remarks**

Nous collecterons les données de la source de données dans un cache pivot, puis calculerons les données du cache dans les cellules. Cette méthode est uniquement utilisée pour rassembler toutes les données dans un cache pivot.

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

