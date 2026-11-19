---
title: "ListColumn"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une colonne dans un tableau."
type: docs
url: /fr/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

Représente une colonne dans un tableau.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         ListColumn listColumn = table.getListColumns().get(4);
         listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         listColumn.setFormula("=[A]");
         workbook.save("Book1.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | Obtient la formule de cette colonne de liste. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | Obtient la formule de la ligne de totaux de cette colonne de liste. |
| [getDataStyle()](#getDataStyle--) | Obtient le style des données dans cette colonne du tableau. |
| [getFormula()](#getFormula--) | Obtient la formule de la colonne de liste. |
| [getName()](#getName--) | Obtient le nom de la colonne. |
| [getRange()](#getRange--) | Obtient la plage de cette colonne de liste. |
| [getTotalsCalculation()](#getTotalsCalculation--) | Obtient le type de calcul dans la ligne Totaux de la colonne de liste. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | Obtient les libellés d'affichage de la ligne de total. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | Indique si la formule est une formule matricielle. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | Définit la formule pour cette colonne de liste. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | Obtient la formule de la ligne de totaux de cette colonne de liste. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | Définit le style des données dans cette colonne du tableau. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Définit la formule de la colonne de liste. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la colonne. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | Définit le type de calcul dans la ligne Totaux de la colonne de liste. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | Définit les libellés d'affichage de la ligne de total. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```


Obtient la formule de cette colonne de liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - La formule de cette colonne de liste.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


Obtient la formule de la ligne de totaux de cette colonne de liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - La formule de cette colonne de liste.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


Obtient le style des données dans cette colonne du tableau.

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtient la formule de la colonne de liste.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la colonne.

**Remarks**

Si le nom de la colonne est défini, la valeur de la cellule correspondante sera également modifiée.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Obtient la plage de cette colonne de liste.

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


Obtient le type de calcul dans la ligne Totaux de la colonne de liste.

Voir [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


Obtient les libellés d'affichage de la ligne de total.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Indique si la formule est une formule matricielle.

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




### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```


Définit la formule pour cette colonne de liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | la formule de cette colonne de liste. |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


Obtient la formule de la ligne de totaux de cette colonne de liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | la formule de cette colonne de liste. |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


Définit le style des données dans cette colonne du tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Définit la formule de la colonne de liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la colonne.

**Remarks**

Si le nom de la colonne est défini, la valeur de la cellule correspondante sera également modifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


Définit le type de calcul dans la ligne Totaux de la colonne de liste.

Voir [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


Définit les libellés d'affichage de la ligne de total.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

