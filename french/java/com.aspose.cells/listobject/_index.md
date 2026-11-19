---
title: "ListObject"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un tableau dans une feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Représente un tableau dans une feuille de calcul.

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
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | Applique le style de tableau à la plage. |
| [convertToRange()](#convertToRange--) | Convertit le tableau en plage. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | Convertit le tableau en plage. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | Filtre le tableau. |
| [getAlternativeDescription()](#getAlternativeDescription--) | Obtient la description alternative. |
| [getAlternativeText()](#getAlternativeText--) | Obtient le texte alternatif. |
| [getAutoFilter()](#getAutoFilter--) | Obtient le filtre automatique de ce tableau. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Obtient le commentaire du tableau. |
| [getDataRange()](#getDataRange--) | Obtient la plage de données du tableau. |
| [getDataSourceType()](#getDataSourceType--) | Obtient le type de source de données du tableau. |
| [getDisplayName()](#getDisplayName--) | Obtient le nom d'affichage du tableau. |
| [getEndColumn()](#getEndColumn--) | Obtient la colonne de fin de la plage. |
| [getEndRow()](#getEndRow--) | Obtient la ligne de fin de la plage. |
| [getListColumns()](#getListColumns--) | Obtient la liste [ListColumn](../../com.aspose.cells/listcolumn) de ce tableau. |
| [getQueryTable()](#getQueryTable--) | Obtient le QueryTable lié. |
| [getShowHeaderRow()](#getShowHeaderRow--) | Obtient si ce tableau affiche la ligne d’en-tête. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Indique si le format de bandes de colonnes est appliqué. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Indique si la première colonne du tableau utilise le style appliqué. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Indique si la dernière colonne du tableau utilise le style appliqué. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Indique si le format de bandes de lignes est appliqué. |
| [getShowTotals()](#getShowTotals--) | Obtient si ce TAble affiche la ligne de total. |
| [getStartColumn()](#getStartColumn--) | Obtient la colonne de début de la plage. |
| [getStartRow()](#getStartRow--) | Obtient la ligne de début de la plage. |
| [getTableStyleName()](#getTableStyleName--) | Obtient le nom du style du tableau. |
| [getTableStyleType()](#getTableStyleType--) | Obtient le style de tableau intégré. |
| [getXmlMap()](#getXmlMap--) | Obtient un [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) utilisé pour cette liste. |
| [hasAutoFilter()](#hasAutoFilter--) | Indique si le filtre automatique est appliqué à ce tableau. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | Placez la formule dans la cellule du tableau. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | Placez la formule dans la cellule du tableau. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Placez la valeur dans la cellule. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | Placez la valeur dans la cellule. |
| [removeAutoFilter()](#removeAutoFilter--) | Supprime le filtre automatique appliqué à ce tableau. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Redimensionne la plage de l’objet de liste. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | Définit la description alternative. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Définit le texte alternatif. |
| [setComment(String value)](#setComment-java.lang.String-) | Définit le commentaire du tableau. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Définit le nom d’affichage du tableau. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | Indique si le filtre automatique est appliqué à ce tableau. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | Définit si ce tableau affiche la ligne d’en-tête. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | Indique si le format de bandes de colonnes est appliqué. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | Indique si la première colonne du tableau utilise le style appliqué. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | Indique si la dernière colonne du tableau utilise le style appliqué. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | Indique si le format de bandes de lignes est appliqué. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | Définit si cette TAble affiche la ligne de total. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | Définit le nom du style de tableau. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | Obtient le style de tableau intégré. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Met à jour le nom de toutes les colonnes de liste dans les cellules du tableau. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


Applique le style de tableau à la plage.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


Convertit le tableau en plage.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


Convertit le tableau en plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | les options lors de la conversion du tableau en plage. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


Filtre le tableau.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Au lieu de cela, veuillez définir la propriété ListObject.HasAutoFilter./// Cette propriété sera supprimée 12 mois plus tard à partir d’octobre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


Obtient la description alternative.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Obtient le texte alternatif.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Obtient le filtre automatique de ce tableau.

**Remarks**

Cela ne fonctionne que lorsque [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) est faux.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


Obtient le commentaire du tableau.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Obtient la plage de données du tableau.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Obtient le type de source de données du tableau.

Voir [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Obtient le nom d'affichage du tableau.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Obtient la colonne de fin de la plage.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Obtient la ligne de fin de la plage.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


Obtient la liste [ListColumn](../../com.aspose.cells/listcolumn) de ce tableau.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


Obtient le QueryTable lié.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


Obtient si ce tableau affiche la ligne d’en-tête.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Indique si le format de bandes de colonnes est appliqué.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Indique si la première colonne du tableau utilise le style appliqué.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Indique si la dernière colonne du tableau utilise le style appliqué.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Indique si le format de bandes de lignes est appliqué.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


Obtient si ce TAble affiche la ligne de total.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Obtient la colonne de début de la plage.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Obtient la ligne de début de la plage.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


Obtient le nom du style du tableau.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Obtient le style de tableau intégré.

Voir [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


Obtient un [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) utilisé pour cette liste.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


Indique si le filtre automatique est appliqué à ce tableau.

**Returns:**
boolean
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




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


Placez la formule dans la cellule du tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | Le décalage de ligne dans le tableau. |
| columnOffset | int | Le décalage de colonne dans le tableau. |
| formula | java.lang.String | La formule de la cellule. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


Placez la formule dans la cellule du tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | Le décalage de ligne dans le tableau. |
| columnOffset | int | Le décalage de colonne dans le tableau. |
| formula | java.lang.String | La formule de la cellule. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Placez la valeur dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | Le décalage de ligne dans le tableau. |
| columnOffset | int | Le décalage de colonne dans le tableau. |
| valeur | java.lang.Object | La valeur de la cellule. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


Placez la valeur dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | Le décalage de ligne dans le tableau. |
| columnOffset | int | Le décalage de colonne dans le tableau. |
| valeur | java.lang.Object | La valeur de la cellule. |
| isTotalsRowLabel | boolean | Indique s'il s'agit d'une étiquette pour la ligne de total, ne fonctionne que pour la ligne de total. Si False et que cette ligne est la ligne de total, une nouvelle ligne sera insérée. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Supprime le filtre automatique appliqué à ce tableau.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Redimensionne la plage de l’objet de liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | L'index de ligne de départ de la nouvelle plage. |
| startColumn | int | L'index de colonne de départ de la nouvelle plage. |
| endRow | int | L'index de ligne de fin de la nouvelle plage. |
| endColumn | int | L'index de colonne de fin de la nouvelle plage. |
| hasHeaders | boolean | Indique si ce tableau possède des en-têtes. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


Définit la description alternative.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Définit le texte alternatif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Définit le commentaire du tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Définit le nom d’affichage du tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


Indique si le filtre automatique est appliqué à ce tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


Définit si ce tableau affiche la ligne d’en-tête.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


Indique si le format de bandes de colonnes est appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


Indique si la première colonne du tableau utilise le style appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


Indique si la dernière colonne du tableau utilise le style appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


Indique si le format de bandes de lignes est appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


Définit si cette TAble affiche la ligne de total.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


Définit le nom du style de tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


Obtient le style de tableau intégré.

Voir [TableStyleType](../../com.aspose.cells/tablestyletype).

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
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Met à jour le nom de toutes les colonnes de liste dans les cellules du tableau.

**Remarks**

La valeur des cellules de la ligne d'en-tête du tableau doit être identique au nom de la ListColumn ; Cell.PutValue ne modifie pas automatiquement le nom de la ListColumn pour des raisons de performance.

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

