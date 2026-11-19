---
title: "ExportTableOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente toutes les options d'exportation de tableau."
type: docs
url: /fr/java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

Représente toutes les options d'exportation de tableau.

**Remarks**

S'il existe des exigences particulières concernant l'exportation, comme ignorer les valeurs d'erreur, l'utilisateur peut étendre cette classe pour remplacer les API correspondantes afin d'atteindre l'objectif.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | Cette valeur indique si les DBNull sont autorisés dans cette table. |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False, Aspose.Cells définira le type du DataColumn en fonction du type de valeur de la première ligne pour des performances optimales. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Exporte la valeur chaîne html des cellules vers le DataTable. |
| [getExportAsString()](#getExportAsString--) | Exporte la valeur chaîne des cellules vers le DataTable. |
| [getExportColumnName()](#getExportColumnName--) | Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. |
| [getFormatStrategy()](#getFormatStrategy--) | Obtient la stratégie de formatage lors de l'exportation de la valeur en tant que chaîne. |
| [getIndexes()](#getIndexes--) | Les index des colonnes/lignes qui doivent être exportés. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Exporte uniquement les cellules visibles. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Exporte uniquement les colonnes visibles. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Exporte uniquement les lignes visibles. |
| [getRenameStrategy()](#getRenameStrategy--) | Stratégie pour les noms de colonnes en double. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Indique s'il faut ignorer les valeurs invalides pour la colonne. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | Vrai si une ligne du fichier Workbook représente une ligne dans le DataTable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | Prétraiter la valeur de la cellule actuelle à exporter. |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | Cette valeur indique si les DBNull sont autorisés dans cette table. |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | False, Aspose.Cells définira le type du DataColumn en fonction du type de valeur de la première ligne pour des performances optimales. |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | Exporte la valeur chaîne html des cellules vers le DataTable. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Exporte la valeur chaîne des cellules vers le DataTable. |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Définit la stratégie de format lors de l'exportation de la valeur en tant que chaîne. |
| [setIndexes(int[] value)](#setIndexes-int---) | Les index des colonnes/lignes qui doivent être exportés. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Exporte uniquement les cellules visibles. |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | Exporte uniquement les colonnes visibles. |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | Exporte uniquement les lignes visibles. |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | Stratégie pour les noms de colonnes en double. |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | Indique s'il faut ignorer les valeurs invalides pour la colonne. |
| [setVertical(boolean value)](#setVertical-boolean-) | Vrai si une ligne du fichier Workbook représente une ligne dans le DataTable. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExportTableOptions() {#ExportTableOptions--}
```
public ExportTableOptions()
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
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```


Cette valeur indique si les DBNull sont autorisés dans cette table.

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


False, Aspose.Cells définira le type du DataColumn's selon le type de valeur de la première ligne pour des performances. True, Aspose.Cells vérifiera si le type de valeur dans la colonne est mixte avant de définir le type du DataColumn's. Et si le type de valeur est mixte, le type du DataColumn's sera string.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExportAsHtmlString() {#getExportAsHtmlString--}
```
public boolean getExportAsHtmlString()
```


Exporte la valeur chaîne html des cellules vers le DataTable.

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Exporte la valeur chaîne des cellules vers le DataTable.

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. La valeur par défaut est false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Obtient la stratégie de formatage lors de l'exportation de la valeur en tant que chaîne.

Voir [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

La valeur par défaut est [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


Les index des colonnes/lignes qui doivent être exportés.

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Exporte uniquement les cellules visibles.

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


Exporte uniquement les colonnes visibles.

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


Exporte uniquement les lignes visibles.

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


Stratégie pour les noms de colonnes en double.

Voir [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


Indique s'il faut ignorer les valeurs invalides pour la colonne. Par exemple, si le type de la colonne est decimal, que la valeur dépasse decimal.MaxValue et que cette propriété est true, nous ne relancerons pas d'exception. La valeur par défaut est false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVertical() {#isVertical--}
```
public boolean isVertical()
```


Vrai si une ligne du fichier Workbook représente une ligne dans le DataTable. Faux si une colonne du fichier Workbook représente une ligne dans le DataTable.

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




### preprocessExportedValue(int cellRow, int cellColumn, CellValue value) {#preprocessExportedValue-int-int-com.aspose.cells.CellValue-}
```
public boolean preprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```


Prétraiter la valeur de la cellule actuelle à exporter.

**Remarks**

Les index de ligne et de colonne sont les index absolus de la cellule dans la feuille de calcul, pas les index dans le tableau exporté. L'utilisateur peut vérifier la valeur de la cellule actuelle dans l'implémentation de substitution de cette méthode ; si la cellule actuelle doit être remplacée par un autre type et une autre valeur, l'implémentation doit alors définir le type et la valeur attendus dans l'objet CellValue et retourner true. Par défaut, cette méthode ne fait rien et retourne false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellRow | int | l'index de ligne de la cellule actuelle |
| cellColumn | int | l'index de colonne de la cellule |
| value | [CellValue](../../com.aspose.cells/cellvalue) | valeur et type de la cellule actuelle |

**Returns:**
booléen - Indique si la cellule actuelle a été remplacée par un type et/ou une valeur différents.
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```


Cette valeur indique si les DBNull sont autorisés dans cette table.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


False, Aspose.Cells définira le type du DataColumn's selon le type de valeur de la première ligne pour des performances. True, Aspose.Cells vérifiera si le type de valeur dans la colonne est mixte avant de définir le type du DataColumn's. Et si le type de valeur est mixte, le type du DataColumn's sera string.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


Exporte la valeur chaîne html des cellules vers le DataTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Exporte la valeur chaîne des cellules vers le DataTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Définit la stratégie de format lors de l'exportation de la valeur en tant que chaîne.

Voir [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

La valeur par défaut est [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


Les index des colonnes/lignes qui doivent être exportés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Exporte uniquement les cellules visibles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


Exporte uniquement les colonnes visibles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


Exporte uniquement les lignes visibles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


Stratégie pour les noms de colonnes en double.

Voir [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


Indique s'il faut ignorer les valeurs invalides pour la colonne. Par exemple, si le type de la colonne est decimal, que la valeur dépasse decimal.MaxValue et que cette propriété est true, nous ne relancerons pas d'exception. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


Vrai si une ligne du fichier Workbook représente une ligne dans le DataTable. Faux si une colonne du fichier Workbook représente une ligne dans le DataTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

