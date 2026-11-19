---
title: "FormatConditionCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la mise en forme conditionnelle."
type: docs
url: /fr/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

Représente le formatage conditionnel. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
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
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | Ajoute une condition de formatage et la plage de cellules affectée aux FormatConditions. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Ajoute une plage de cellules formatée conditionnellement. |
| [addCondition(int type)](#addCondition-int-) | Ajouter une condition de format. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | Ajoute une condition de formatage. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient la condition de formatage par indice. |
| [getCellArea(int index)](#getCellArea-int-) | Obtient la plage de cellules formatée conditionnellement par indice. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre de conditions. |
| [getRangeCount()](#getRangeCount--) | Obtient le nombre de plages formatées conditionnellement. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | Supprime la plage de cellules formatée conditionnellement par indice. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Supprimer le formatage conditionnel dans la plage. |
| [removeCondition(int index)](#removeCondition-int-) | Supprime la condition de formatage par indice. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


Ajoute une condition de formatage et la plage de cellules affectée aux FormatConditions. Les FormatConditions peuvent contenir jusqu’à trois formats conditionnels. Les références aux autres feuilles ne sont pas autorisées dans les formules du formatage conditionnel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Plage de cellules formatée conditionnellement. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Type de formatage conditionnel. Il peut s’agir de l’un des membres de FormatConditionType. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Opérateur de comparaison. Il peut s’agir de l’un des membres de OperatorType. |
| formula1 | java.lang.String | La valeur ou l’expression associée au formatage conditionnel. |
| formula2 | java.lang.String | La valeur ou l’expression associée au formatage conditionnel |

**Returns:**
int[] - [0] : index de l’objet de condition de formatage ;[1] index de la plage de cellules affectée.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


Ajoute une plage de cellules formatée conditionnellement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Plage de cellules formatée conditionnellement. |

**Returns:**
int - index de la plage de cellules formatée conditionnellement.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


Ajouter une condition de format.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Type de condition de format. |

**Returns:**
int - index de l’objet de condition de formatage ;
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


Ajoute une condition de formatage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Le type de condition de format. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Le type d’opérateur |
| formula1 | java.lang.String | La valeur ou l’expression associée au formatage conditionnel. Si la valeur d’entrée commence par '=', elle sera considérée comme une formule. Sinon, elle sera prise comme une valeur simple (texte, nombre, booléen). Pour une valeur texte commençant par '=', l’utilisateur peut la saisir comme formule au format : "=\\"=...\\"". |
| formula2 | java.lang.String | La valeur ou l'expression associée au format conditionnel. Le format d'entrée est le même que formula1 |

**Returns:**
int - index de l’objet de condition de formatage ;
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
### get(int index) {#get-int-}
```
public FormatCondition get(int index)
```


Obtient la condition de formatage par indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l'index de la condition de formatage à renvoyer. |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


Obtient la plage de cellules formatée conditionnellement par indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l'index de la plage de cellules formatées conditionnellement. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre de conditions.

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Obtient le nombre de plages formatées conditionnellement.

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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


Supprime la plage de cellules formatée conditionnellement par indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de la plage de cellules formatées conditionnellement à supprimer. |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


Supprimer le formatage conditionnel dans la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Le startRow de la plage. |
| startColumn | int | Le startColumn de la plage. |
| totalRows | int | Le nombre de lignes de la plage. |
| totalColumns | int | Le nombre de colonnes de la plage. |

**Returns:**
booléen - Retourne TRUE, cette FormatCondtionCollection doit être supprimée.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


Supprime la condition de formatage par indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de la condition de formatage à supprimer. |

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

