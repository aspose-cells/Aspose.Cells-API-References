---
title: "ImportTableOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'importation de données dans les cellules."
type: docs
url: /fr/java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

Représente les options d'importation de données dans les cellules.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | Crée les options d'importation par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | Indique si la vérification des cellules fusionnées est effectuée. |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | Obtient les colonnes (indexées à partir de 0) à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées. |
| [getConvertGridStyle()](#getConvertGridStyle--) | Indique si le style de la vue grille doit être appliqué aux cellules. |
| [getConvertNumericData()](#getConvertNumericData--) | Obtient une valeur indiquant si la valeur chaîne doit être convertie en valeur numérique ou date. |
| [getDateFormat()](#getDateFormat--) | Obtient la chaîne de format de date pour les cellules contenant des valeurs datetime importées. |
| [getDefaultValues()](#getDefaultValues--) | La valeur par défaut pour la valeur dans le tableau est null. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | Indique si la légende est exportée comme nom de champ |
| [getInsertRows()](#getInsertRows--) | Indique si de nouvelles lignes doivent être ajoutées pour l'importation des enregistrements de données. |
| [getNumberFormats()](#getNumberFormats--) | Obtient les formats numériques |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | Indique si la première ligne doit être décalée vers le bas lors de l'insertion de lignes. |
| [getStyles()](#getStyles--) | Obtient les styles pour chaque colonne du tableau. |
| [getTotalColumns()](#getTotalColumns--) | Obtient le nombre total de colonnes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée. |
| [getTotalRows()](#getTotalRows--) | Obtient le nombre total de lignes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | Indique si le nom de champ doit être importé. |
| [isFormulas()](#isFormulas--) | Indique si les données sont des formules. |
| [isHtmlString()](#isHtmlString--) | Indique si la valeur contient des balises html. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | Indique si la vérification des cellules fusionnées est effectuée. |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | Définit les colonnes (indexées à partir de 0) à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées. |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | Indique si le style de la vue grille doit être appliqué aux cellules. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Définit une valeur indiquant si la chaîne doit être convertie en valeur numérique ou en date. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | Définit le format de date pour les cellules contenant des valeurs datetime importées. |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | La valeur par défaut pour la valeur dans le tableau est null. |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | Indique si la légende est exportée comme nom de champ |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | Indique si le nom de champ doit être importé. |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | Indique si les données sont des formules. |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | Indique si la valeur contient des balises html. |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | Indique si de nouvelles lignes doivent être ajoutées pour l'importation des enregistrements de données. |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | Définit les formats numériques |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | Indique si la première ligne doit être décalée vers le bas lors de l'insertion de lignes. |
| [setStyles(Style[] value)](#setStyles-com.aspose.cells.Style---) | Définit les styles pour chaque colonne du tableau. |
| [setTotalColumns(int value)](#setTotalColumns-int-) | Définit le nombre total de colonnes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée. |
| [setTotalRows(int value)](#setTotalRows-int-) | Définit le nombre total de lignes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


Crée les options d'importation par défaut.

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


Indique si la vérification des cellules fusionnées est effectuée.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


Obtient les colonnes (indexées à partir de 0) à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées.

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


Indique si le style de la vue grille doit être appliqué aux cellules.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Obtient une valeur indiquant si la valeur chaîne doit être convertie en valeur numérique ou date.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


Obtient la chaîne de format de date pour les cellules contenant des valeurs datetime importées.

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


La valeur par défaut pour la valeur dans le tableau est null.

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


Indique si la légende est exportée comme nom de champ

**Remarks**

Fonctionne uniquement pour DataTable.

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


Indique si de nouvelles lignes doivent être ajoutées pour l'importation des enregistrements de données.

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


Obtient les formats numériques

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


Indique si la première ligne doit être décalée vers le bas lors de l'insertion de lignes.

**Returns:**
boolean
### getStyles() {#getStyles--}
```
public Style[] getStyles()
```


Obtient les styles pour chaque colonne du tableau.

**Returns:**
com.aspose.cells.Style[]
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


Obtient le nombre total de colonnes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée.

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


Obtient le nombre total de lignes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


Indique si le nom de champ doit être importé.

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


Indique si les données sont des formules.

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


Indique si la valeur contient des balises html.

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




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


Indique si la vérification des cellules fusionnées est effectuée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


Définit les colonnes (indexées à partir de 0) à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


Indique si le style de la vue grille doit être appliqué aux cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Définit une valeur indiquant si la chaîne doit être convertie en valeur numérique ou en date.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


Définit le format de date pour les cellules contenant des valeurs datetime importées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


La valeur par défaut pour la valeur dans le tableau est null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


Indique si la légende est exportée comme nom de champ

**Remarks**

Fonctionne uniquement pour DataTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


Indique si le nom de champ doit être importé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


Indique si les données sont des formules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


Indique si la valeur contient des balises html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


Indique si de nouvelles lignes doivent être ajoutées pour l'importation des enregistrements de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


Définit les formats numériques

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


Indique si la première ligne doit être décalée vers le bas lors de l'insertion de lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyles(Style[] value) {#setStyles-com.aspose.cells.Style---}
```
public void setStyles(Style[] value)
```


Définit les styles pour chaque colonne du tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Style\[\]](../../com.aspose.cells/style) |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


Définit le nombre total de colonnes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


Définit le nombre total de lignes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée.

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

