---
title: "PivotFieldGroupOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Options pour les paramètres de groupement du champ de tableau croisé dynamique."
type: docs
url: /fr/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

Options pour les paramètres de groupement du champ de tableau croisé dynamique.

**Example**

```
         // Load the sample workbook
         Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
         // Access the second worksheet and its pivot table
         PivotTable pt = wb.getWorksheets().get(1).getPivotTables().get(0);
         // Group the first row field (a date field) by months and quarters
         PivotFieldGroupOptions options = new PivotFieldGroupOptions();
         options.setStartDate(new DateTime(2008, 1, 1));
         options.setEndDate(new DateTime(2008, 9, 5));
         options.setGroupTypes(new /*PivotGroupByType*/int[] { PivotGroupByType.MONTHS, PivotGroupByType.QUARTERS });
         pt.getRowFields().get(0).group(options);
         // Calculate the pivot table data and save the output file
         pt.calculateData();
         wb.save("outputGroupPivotFieldsInPivotTable.xlsx");
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | Obtient les éléments de groupe discrets. |
| [getEndDate()](#getEndDate--) | Obtient la valeur de fin de la plage de regroupement. |
| [getEndNumber()](#getEndNumber--) | Obtient la valeur de fin de la plage de regroupement. |
| [getGroupType()](#getGroupType--) | Obtient le type de regroupement pour le champ pivot. |
| [getGroupTypes()](#getGroupTypes--) | Obtient le type de regroupement pour le champ pivot. |
| [getInterval()](#getInterval--) | Obtient la taille d'intervalle pour chaque groupe. |
| [getNewPivotField()](#getNewPivotField--) | Obtient une valeur indiquant si de nouveaux champs pivot doivent être créés après le regroupement. |
| [getStartDate()](#getStartDate--) | Obtient la valeur de début de la plage de regroupement. |
| [getStartNumber()](#getStartNumber--) | Obtient la valeur de début de la plage de regroupement. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | Obtient une valeur indiquant si la valeur de fin est déterminée automatiquement. |
| [isAutoStart()](#isAutoStart--) | Obtient une valeur indiquant si la valeur de début est déterminée automatiquement. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | Définit une valeur indiquant si la valeur de fin est déterminée automatiquement. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | Définit une valeur indiquant si la valeur de début est déterminée automatiquement. |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | Définit les éléments de groupe discrets. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | Définit la valeur de fin de la plage de regroupement. |
| [setEndNumber(double value)](#setEndNumber-double-) | Définit la valeur de fin de la plage de regroupement. |
| [setGroupType(int value)](#setGroupType-int-) | Définit le type de regroupement pour le champ pivot. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | Définit le type de regroupement pour le champ pivot. |
| [setInterval(double value)](#setInterval-double-) | Définit la taille d'intervalle pour chaque groupe. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | Définit une valeur indiquant si de nouveaux champs pivot doivent être créés après le regroupement. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Définit la valeur de début de la plage de regroupement. |
| [setStartNumber(double value)](#setStartNumber-double-) | Définit la valeur de début de la plage de regroupement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupOptions() {#PivotFieldGroupOptions--}
```
public PivotFieldGroupOptions()
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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


Obtient les éléments de groupe discrets.

**Remarks**

Si cette propriété est définie,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


Obtient la valeur de fin de la plage de regroupement.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


Obtient la valeur de fin de la plage de regroupement.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


Obtient le type de regroupement pour le champ pivot. Uniquement pour le regroupement des champs pivot de type date/heure.

Voir [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Example**

```
         //init
         PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
         // Group by year and month together
         /*PivotGroupByType*/int pivotGroupByType = pivotFieldGroupOptions.getGroupType();
         pivotGroupByType = PivotGroupByType.YEARS | PivotGroupByType.MONTHS;
         pivotFieldGroupOptions.setGroupType(pivotGroupByType);
```

**Returns:**
int
### getGroupTypes() {#getGroupTypes--}
```
public int[] getGroupTypes()
```


Obtient le type de regroupement pour le champ pivot.

Voir [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

L'ordre dans cette propriété sera ignoré. Lors de la spécification de plusieurs types de groupe, les champs de groupe de base seront insérés par ordre croissant et le champ de groupe sera affiché dans la région ligne/colonne par ordre décroissant (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


Obtient la taille d'intervalle pour chaque groupe.

**Remarks**

Uniquement pour le groupe de nombres et de jours.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


Obtient une valeur indiquant si de nouveaux champs pivot doivent être créés après le regroupement.

**Remarks**

Si elle n'est pas explicitement définie, la valeur par défaut est false pour le regroupement numérique et true pour le regroupement date-heure, true pour le groupe discret. Fonctionne uniquement pour le premier nouveau champ pivot de groupe du champ de base.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Obtient la valeur de début de la plage de regroupement.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


Obtient la valeur de début de la plage de regroupement.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoEnd() {#isAutoEnd--}
```
public boolean isAutoEnd()
```


Obtient une valeur indiquant si la valeur de fin est déterminée automatiquement.

**Remarks**

Si [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) ou [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) est définie, cette propriété sera false.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


Obtient une valeur indiquant si la valeur de début est déterminée automatiquement.

**Remarks**

Si [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) ou [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) est définie, cette propriété sera false.

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




### setAutoEnd(boolean value) {#setAutoEnd-boolean-}
```
public void setAutoEnd(boolean value)
```


Définit une valeur indiquant si la valeur de fin est déterminée automatiquement.

**Remarks**

Si [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) ou [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) est définie, cette propriété sera false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


Définit une valeur indiquant si la valeur de début est déterminée automatiquement.

**Remarks**

Si [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) ou [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) est définie, cette propriété sera false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


Définit les éléments de groupe discrets.

**Remarks**

Si cette propriété est définie,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


Définit la valeur de fin de la plage de regroupement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


Définit la valeur de fin de la plage de regroupement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


Définit le type de regroupement pour le champ pivot. Uniquement pour le regroupement des champs pivot de type date/heure.

Voir [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


Définit le type de regroupement pour le champ pivot.

Voir [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

L'ordre dans cette propriété sera ignoré. Lors de la spécification de plusieurs types de groupe, les champs de groupe de base seront insérés par ordre croissant et le champ de groupe sera affiché dans la région ligne/colonne par ordre décroissant (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


Définit la taille d'intervalle pour chaque groupe.

**Remarks**

Uniquement pour le groupe de nombres et de jours.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


Définit une valeur indiquant si de nouveaux champs pivot doivent être créés après le regroupement.

**Remarks**

Si elle n'est pas explicitement définie, la valeur par défaut est false pour le regroupement numérique et true pour le regroupement date-heure, true pour le groupe discret. Fonctionne uniquement pour le premier nouveau champ pivot de groupe du champ de base.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Définit la valeur de début de la plage de regroupement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


Définit la valeur de début de la plage de regroupement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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

