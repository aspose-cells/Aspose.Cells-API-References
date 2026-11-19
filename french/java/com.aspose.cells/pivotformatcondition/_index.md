---
title: "PivotFormatCondition"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une condition de format de tableau croisé dynamique dans la collection PivotFormatCondition."
type: docs
url: /fr/java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

Représente une condition de format de tableau croisé dynamique dans la collection PivotFormatCondition.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser la classe [PivotConditionalFormat](../../com.aspose.cells/pivotconditionalformat). Cette méthode sera supprimée 12 mois plus tard, à compter de décembre 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de colonne. |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de colonne. |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de données. |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de données. |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de ligne. |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de ligne. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Obtient les conditions du format conditionnel du tableau croisé dynamique. |
| [getRuleType()](#getRuleType--) | Obtient le type de règle du format conditionnel du tableau croisé dynamique. |
| [getScopeType()](#getScopeType--) | Obtient le type de portée du format conditionnel du tableau croisé dynamique. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | Définit les zones conditionnelles de l'objet PivotFormatCondition. |
| [setRuleType(int value)](#setRuleType-int-) | Définit le type de règle du format conditionnel du tableau croisé dynamique. |
| [setScopeType(int value)](#setScopeType-int-) | Définit le type de portée du format conditionnel du tableau croisé dynamique. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | Le PivotField dans les champs de colonne. |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | Le nom du PivotField. |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | Le PivotField dans les champs de données. |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | Le nom du PivotField. |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | Le PivotField dans les champs de ligne. |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


Ajoute la limite de format conditionnel du tableau croisé dynamique dans les champs de ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | Le nom du PivotField. |

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
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Obtient les conditions du format conditionnel du tableau croisé dynamique.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Obtient le type de règle du format conditionnel du tableau croisé dynamique.

Voir [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Obtient le type de portée du format conditionnel du tableau croisé dynamique.

Voir [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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




### setConditionalAreas() {#setConditionalAreas--}
```
public void setConditionalAreas()
```


Définit les zones conditionnelles de l'objet PivotFormatCondition.

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Définit le type de règle du format conditionnel du tableau croisé dynamique.

Voir [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Définit le type de portée du format conditionnel du tableau croisé dynamique.

Voir [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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

