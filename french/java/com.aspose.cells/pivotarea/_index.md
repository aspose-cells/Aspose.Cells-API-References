---
title: "PivotArea"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Présente la zone sélectionnée du tableau croisé dynamique."
type: docs
url: /fr/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

Présente la zone sélectionnée du tableau croisé dynamique.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | Présente la zone sélectionnée du tableau croisé dynamique. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | Obtient la région du tableau croisé dynamique à laquelle cette règle s'applique. |
| [getCellAreas()](#getCellAreas--) | Obtient les zones de cellules de cette zone de tableau croisé dynamique. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | Obtient tous les filtres pour cette zone de tableau croisé dynamique. |
| [getOnlyData()](#getOnlyData--) | Indique si seules les valeurs de données (dans la zone de données de la vue) pour une sélection d'élément sont sélectionnées et n'incluent pas les libellés d'élément. |
| [getOnlyLabel()](#getOnlyLabel--) | Indique si seuls les libellés de données pour une sélection d'élément sont sélectionnés. |
| [getRuleType()](#getRuleType--) | Obtient le type de règle de sélection. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | Indique si le total général de la colonne est inclus. |
| [isOutline()](#isOutline--) | Indique si la règle fait référence à une zone en mode plan. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | Indique si le total général de la ligne est inclus. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | Sélectionnez la zone avec des filtres. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | Sélectionnez un champ dans la région comme zone. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | Sélectionnez un champ dans la région comme zone. |
| [setAxisType(int value)](#setAxisType-int-) | Définit la région du tableau croisé dynamique à laquelle cette règle s'applique. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | Indique si le total général de la colonne est inclus. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | Indique si seules les valeurs de données (dans la zone de données de la vue) pour une sélection d'élément sont sélectionnées et n'incluent pas les libellés d'élément. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | Indique si seuls les libellés de données pour une sélection d'élément sont sélectionnés. |
| [setOutline(boolean value)](#setOutline-boolean-) | Indique si la règle fait référence à une zone en mode plan. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | Indique si le total général de la ligne est inclus. |
| [setRuleType(int value)](#setRuleType-int-) | Définit le type de règle de sélection. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


Présente la zone sélectionnée du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

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
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


Obtient la région du tableau croisé dynamique à laquelle cette règle s'applique.

Voir [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Obtient les zones de cellules de cette zone de tableau croisé dynamique.

**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilters() {#getFilters--}
```
public PivotAreaFilterCollection getFilters()
```


Obtient tous les filtres pour cette zone de tableau croisé dynamique.

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


Indique si seules les valeurs de données (dans la zone de données de la vue) pour une sélection d'élément sont sélectionnées et n'incluent pas les libellés d'élément.

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


Indique si seuls les libellés de données pour une sélection d'élément sont sélectionnés.

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Obtient le type de règle de sélection.

Voir [PivotAreaType](../../com.aspose.cells/pivotareatype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isColumnGrandIncluded() {#isColumnGrandIncluded--}
```
public boolean isColumnGrandIncluded()
```


Indique si le total général de la colonne est inclus.

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Indique si la règle fait référence à une zone en mode plan.

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


Indique si le total général de la ligne est inclus.

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




### select(int axisType, int fieldPosition, int selectionType) {#select-int-int-int-}
```
public void select(int axisType, int fieldPosition, int selectionType)
```


Sélectionnez la zone avec des filtres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). La région du tableau croisé dynamique à laquelle cette règle s'applique. |
| fieldPosition | int | Position du champ dans l'axe auquel cette règle s'applique. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Spécifie ce qui peut être sélectionné dans un tableau croisé dynamique lors d'une sélection structurée. |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


Sélectionnez un champ dans la région comme zone.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de région. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Le champ du tableau croisé dynamique. |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


Sélectionnez un champ dans la région comme zone.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Le type de région. |
| fieldName | java.lang.String | Le nom du champ du tableau croisé dynamique. |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


Définit la région du tableau croisé dynamique à laquelle cette règle s'applique.

Voir [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


Indique si le total général de la colonne est inclus.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


Indique si seules les valeurs de données (dans la zone de données de la vue) pour une sélection d'élément sont sélectionnées et n'incluent pas les libellés d'élément.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


Indique si seuls les libellés de données pour une sélection d'élément sont sélectionnés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Indique si la règle fait référence à une zone en mode plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


Indique si le total général de la ligne est inclus.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Définit le type de règle de sélection.

Voir [PivotAreaType](../../com.aspose.cells/pivotareatype).

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

