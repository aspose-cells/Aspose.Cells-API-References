---
title: "FormatCondition"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la condition de mise en forme conditionnelle."
type: docs
url: /fr/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

Représente la condition de mise en forme conditionnelle.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
 
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
 
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
 
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         //Saving the Excel file
         workbook.save("output.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | Obtenez l'instance "AboveAverage" du format conditionnel. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | Obtenez l'instance "ColorScale" du format conditionnel. |
| [getDataBar()](#getDataBar--) | Obtenez l'instance "DataBar" du format conditionnel. |
| [getFormula1()](#getFormula1--) | Obtient la valeur ou l'expression associée au format conditionnel. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Obtient la valeur ou l'expression associée à cette condition de format. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Obtient la valeur ou l'expression du format conditionnel de la cellule. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | Obtient la formule du format conditionnel de la cellule. |
| [getFormula2()](#getFormula2--) | Obtient la valeur ou l'expression associée au format conditionnel. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Obtient la valeur ou l'expression associée à cette condition de format. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Obtient la valeur ou l'expression du format conditionnel de la cellule. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | Obtient la formule du format conditionnel de la cellule. |
| [getIconSet()](#getIconSet--) | Obtenez l'instance "IconSet" du format conditionnel. |
| [getOperator()](#getOperator--) | Obtient le type d'opérateur du format conditionnel. |
| [getPriority()](#getPriority--) | La priorité de cette règle de format conditionnel. |
| [getStopIfTrue()](#getStopIfTrue--) | Vrai, aucune règle de priorité inférieure ne peut être appliquée à cette règle, lorsque cette règle s'évalue à vrai. |
| [getStyle()](#getStyle--) | Obtient ou définit le style des plages de cellules formatées conditionnellement. |
| [getText()](#getText--) | La valeur texte dans une règle de mise en forme conditionnelle "text contains". |
| [getTimePeriod()](#getTimePeriod--) | La période de temps applicable dans une règle de mise en forme conditionnelle "date occurrin". |
| [getTop10()](#getTop10--) | Obtenez l'instance "Top10" de la mise en forme conditionnelle. |
| [getType()](#getType--) | Obtient le type du format conditionnel. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Définit la valeur ou l'expression associée à la mise en forme conditionnelle. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Définit la valeur ou l'expression associée à cette condition de format. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Définit la valeur ou l'expression associée à la mise en forme conditionnelle. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Définit la valeur ou l'expression associée à cette condition de format. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | Définit la valeur ou l'expression associée à cette condition de format. |
| [setOperator(int value)](#setOperator-int-) | Définit le type d'opérateur du format conditionnel. |
| [setPriority(int value)](#setPriority-int-) | La priorité de cette règle de format conditionnel. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | Vrai, aucune règle de priorité inférieure ne peut être appliquée à cette règle, lorsque cette règle s'évalue à vrai. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Obtient ou définit le style des plages de cellules formatées conditionnellement. |
| [setText(String value)](#setText-java.lang.String-) | La valeur texte dans une règle de mise en forme conditionnelle "text contains". |
| [setTimePeriod(int value)](#setTimePeriod-int-) | La période de temps applicable dans une règle de mise en forme conditionnelle "date occurrin". |
| [setType(int value)](#setType-int-) | Définit le type du format conditionnel. |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


Obtenez l'instance "AboveAverage" de la mise en forme conditionnelle. La règle de l'instance par défaut met en évidence les cellules dont la valeur est supérieure à la moyenne de toutes les valeurs de la plage. Valide uniquement pour le type = AboveAverage.

**Returns:**
[AboveAverage](../../com.aspose.cells/aboveaverage) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorScale() {#getColorScale--}
```
public ColorScale getColorScale()
```


Obtenez l'instance "ColorScale" de la mise en forme conditionnelle. L'instance par défaut est une "green-yellow-red" 3ColorScale. Valide uniquement pour le type = ColorScale.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


Obtenez l'instance "DataBar" de la mise en forme conditionnelle. La couleur de l'instance par défaut est bleue. Valide uniquement pour le type = DataBar.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Obtient la valeur ou l'expression associée au format conditionnel.

**Remarks**

Veuillez ajouter toutes les zones avant de définir la formule. Pour définir la formule de cette condition, si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera considérée comme une valeur simple (texte, nombre, booléen). Pour une valeur texte commençant par '=', l'utilisateur peut la saisir comme formule au format : "=\"=...\"".

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Obtient la valeur ou l'expression associée à cette condition de format.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - La valeur ou l'expression associée à cette condition de format.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtient la valeur ou l'expression du format conditionnel de la cellule.

**Remarks**

La cellule donnée doit être contenue dans cette mise en forme conditionnelle, sinon null sera retourné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
java.lang.String - La valeur ou l'expression associée à la mise en forme conditionnelle de la cellule.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


Obtient la formule du format conditionnel de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
java.lang.String - La formule.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Obtient la valeur ou l'expression associée au format conditionnel.

**Remarks**

Veuillez ajouter toutes les zones avant de définir la formule. Pour définir la formule de cette condition, si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera considérée comme une valeur simple (texte, nombre, booléen). Pour une valeur texte commençant par '=', l'utilisateur peut la saisir comme formule au format : "=\"=...\"".

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Obtient la valeur ou l'expression associée à cette condition de format.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - La valeur ou l'expression associée à cette condition de format.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtient la valeur ou l'expression du format conditionnel de la cellule.

**Remarks**

La cellule donnée doit être contenue dans cette mise en forme conditionnelle, sinon null sera retourné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
java.lang.String - La valeur ou l'expression associée à la mise en forme conditionnelle de la cellule.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


Obtient la formule du format conditionnel de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
java.lang.String - La formule.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


Obtenez l'instance "IconSet" de la mise en forme conditionnelle. Le IconSetType de l'instance par défaut est TrafficLights31. Valide uniquement pour le type = IconSet.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


Obtient le type d'opérateur du format conditionnel.

Voir [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


La priorité de cette règle de mise en forme conditionnelle. Cette valeur est utilisée pour déterminer quel format doit être évalué et rendu. Les valeurs numériques plus faibles ont une priorité plus élevée que les valeurs numériques plus élevées, où '1' est la priorité la plus haute.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


Vrai, aucune règle de priorité inférieure ne peut être appliquée à cette règle, lorsque cette règle s'évalue à vrai. S'applique uniquement à Excel 2007 ;

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtient ou définit le style des plages de cellules formatées conditionnellement.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


La valeur texte dans une règle de mise en forme conditionnelle "text contains". Valide uniquement pour les types = containsText, notContainsText, beginsWith et endsWith. La valeur par défaut est null.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


La période de temps applicable dans une règle de mise en forme conditionnelle "date occurrin". Valide uniquement pour le type = timePeriod. La valeur par défaut est TimePeriodType.Today.

Voir [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


Obtenez l'instance "Top10" de la mise en forme conditionnelle. La règle de l'instance par défaut met en évidence les cellules dont les valeurs se situent dans le top 10. Valide uniquement pour le type = Top10.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


Obtient le type du format conditionnel.

Voir [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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




### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Définit la valeur ou l'expression associée à la mise en forme conditionnelle.

**Remarks**

Veuillez ajouter toutes les zones avant de définir la formule. Pour définir la formule de cette condition, si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera considérée comme une valeur simple (texte, nombre, booléen). Pour une valeur texte commençant par '=', l'utilisateur peut la saisir comme formule au format : "=\"=...\"".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Définit la valeur ou l'expression associée à cette condition de format.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La valeur ou l'expression associée à cette condition de format. Si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera prise comme une valeur simple (texte, nombre, bool). Pour une valeur texte qui commence par '=', l'utilisateur peut la saisir comme formule au format : "=\\"=...\\"". |
| isR1C1 | boolean | Indique si la formule est au format R1C1. |
| isLocal | boolean | Indique si la formule est formatée selon la locale. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Définit la valeur ou l'expression associée à la mise en forme conditionnelle.

**Remarks**

Veuillez ajouter toutes les zones avant de définir la formule. Pour définir la formule de cette condition, si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera considérée comme une valeur simple (texte, nombre, booléen). Pour une valeur texte commençant par '=', l'utilisateur peut la saisir comme formule au format : "=\"=...\"".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Définit la valeur ou l'expression associée à cette condition de format.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La valeur ou l'expression associée à cette condition de format. Si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera prise comme une valeur simple (texte, nombre, bool). Pour une valeur texte qui commence par '=', l'utilisateur peut la saisir comme formule au format : "=\\"=...\\"". |
| isR1C1 | boolean | Indique si la formule est au format R1C1. |
| isLocal | boolean | Indique si la formule est formatée selon la locale. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


Définit la valeur ou l'expression associée à cette condition de format.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula1 | java.lang.String | La valeur ou l'expression associée à cette condition de format. Si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera prise comme une valeur simple (texte, nombre, bool). Pour une valeur texte qui commence par '=', l'utilisateur peut la saisir comme formule au format : "=\\"=...\\"". |
| formula2 | java.lang.String | La valeur ou l'expression associée à cette condition de format. Le format d'entrée est le même que formula1. |
| isR1C1 | boolean | Indique si la formule est au format R1C1. |
| isLocal | boolean | Indique si la formule est formatée selon la locale. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Définit le type d'opérateur du format conditionnel.

Voir [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


La priorité de cette règle de mise en forme conditionnelle. Cette valeur est utilisée pour déterminer quel format doit être évalué et rendu. Les valeurs numériques plus faibles ont une priorité plus élevée que les valeurs numériques plus élevées, où '1' est la priorité la plus haute.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


Vrai, aucune règle de priorité inférieure ne peut être appliquée à cette règle, lorsque cette règle s'évalue à vrai. S'applique uniquement à Excel 2007 ;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Obtient ou définit le style des plages de cellules formatées conditionnellement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


La valeur texte dans une règle de mise en forme conditionnelle "text contains". Valide uniquement pour les types = containsText, notContainsText, beginsWith et endsWith. La valeur par défaut est null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


La période de temps applicable dans une règle de mise en forme conditionnelle "date occurrin". Valide uniquement pour le type = timePeriod. La valeur par défaut est TimePeriodType.Today.

Voir [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Définit le type du format conditionnel.

Voir [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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

