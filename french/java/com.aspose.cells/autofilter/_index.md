---
title: "AutoFiltre"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le filtrage automatique pour la feuille de calcul spécifiée."
type: docs
url: /fr/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

Représente le filtrage automatique pour la feuille de calcul spécifiée.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | Ajoute un filtre de date. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | Ajoute un filtre de couleur de remplissage. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | Ajoute un filtre pour une colonne de filtre. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | Ajoute un filtre de couleur de police. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | Ajoute un filtre d'icône. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | Filtre une liste avec un critère personnalisé. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | Filtre une liste avec des critères personnalisés. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | Ajoute un filtre dynamique. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | Filtre une liste avec des critères spécifiés. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | Filtrer les 10 premiers éléments de la liste |
| [getCellArea()](#getCellArea--) | Obtient la [CellArea](../../com.aspose.cells/cellarea) où cet AutoFiltre s'applique. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | Obtient la [CellArea](../../com.aspose.cells/cellarea) où l'AutoFiltre spécifié s'applique. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | Obtient la collection des colonnes de filtre. |
| [getRange()](#getRange--) | Représente la plage à laquelle l'AutoFiltre spécifié s'applique. |
| [getShowFilterButton()](#getShowFilterButton--) | Indique si le bouton AutoFilter de cette colonne est visible. |
| [getSorter()](#getSorter--) | Obtient le trieur de données. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | Correspond à toutes les cellules vides de la liste. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | Correspond à toutes les cellules non vides de la liste. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Actualise les auto‑filtres pour masquer ou afficher les lignes. |
| [refresh(boolean hideRows)](#refresh-boolean-) | Obtient les index de toutes les lignes masquées. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | Supprime un filtre de date. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | Supprime le filtre spécifique. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | Supprime un filtre pour une colonne de filtre. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | Définit la plage à laquelle l'AutoFiltre spécifié s'applique. |
| [setRange(String value)](#setRange-java.lang.String-) | Représente la plage à laquelle l'AutoFiltre spécifié s'applique. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | Indique si le bouton AutoFilter de cette colonne est visible. |
| [showAll()](#showAll--) | Afficher toutes les lignes. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Ajoute un filtre de date.

**Remarks**

Si DateTimeGroupingType est Year, seul le paramètre year a un effet. Si DateTiemGroupingType est Month, seuls les paramètres year et month ont un effet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Le type de regroupement |
| année | int | L'année. |
| mois | int | Le mois. |
| jour | int | Le jour. |
| heure | int | L'heure. |
| minute | int | La minute. |
| seconde | int | La seconde. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


Ajoute un filtre de couleur de remplissage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Le type de motif d'arrière-plan. |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | La couleur de premier plan. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | La couleur d'arrière-plan. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


Ajoute un filtre pour une colonne de filtre.

**Remarks**

MS Excel 2007 prend en charge la sélection multiple dans une colonne de filtre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| critères | java.lang.String | Le critère spécifié (une chaîne ; par exemple, "101"). Il ne peut être nul ou être l'une des valeurs des cellules dans cette colonne. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


Ajoute un filtre de couleur de police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | L'objet [CellsColor](../../com.aspose.cells/cellscolor). |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


Ajoute un filtre d'icône.

**Remarks**

Ne prend en charge que l'ajout du filtre d'icône. Ne prend pas en charge la vérification de la visibilité des lignes si le filtre est un filtre d'icône.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). Le type d'ensemble d'icônes. |
| iconId | int | L'identifiant de l'icône. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


Filtre une liste avec un critère personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Le type d'opérateur de filtre. |
| criteria1 | java.lang.Object | Le critère personnalisé |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filtre une liste avec des critères personnalisés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Le type d'opérateur de filtre. |
| criteria1 | java.lang.Object | Le critère personnalisé |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Le type d'opérateur de filtre. |
| criteria2 | java.lang.Object | Le critère personnalisé |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


Ajoute un filtre dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). Type de filtre dynamique. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


Filtre une liste avec des critères spécifiés.

**Remarks**

Aspose.Cells supprimera tous les autres paramètres de filtre sur ce champ comme MS Excel 97-2003.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| critères | java.lang.String | Le critère spécifié (une chaîne ; par exemple, "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


Filtrer les 10 premiers éléments de la liste

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| isTop | boolean | Indique si le filtre provient du haut ou du bas |
| isPercent | boolean | Indique si les éléments sont en pourcentage ou en nombre |
| itemCount | int | Le nombre d'éléments |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Obtient la [CellArea](../../com.aspose.cells/cellarea) où cet AutoFiltre s'applique.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


Obtient la [CellArea](../../com.aspose.cells/cellarea) où l'AutoFiltre spécifié s'applique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| refreshAppliedRange | boolean | Indique s'il faut rafraîchir la plage appliquée. Pour la plage appliquée du filtre automatique, la dernière ligne peut changer lorsque les données des cellules changent. Si ce drapeau est vrai, alors la dernière ligne de la plage sera recalculée en fonction des données actuelles des cellules. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


Obtient la collection des colonnes de filtre.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


Représente la plage à laquelle l'AutoFiltre spécifié s'applique.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


Indique si le bouton AutoFilter de cette colonne est visible.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


Obtient le trieur de données.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


Correspond à toutes les cellules vides de la liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


Correspond à toutes les cellules non vides de la liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int[] refresh()
```


Actualise les auto‑filtres pour masquer ou afficher les lignes.

**Returns:**
int[] - Retourne les index de toutes les lignes masquées.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


Obtient les index de toutes les lignes masquées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| hideRows | boolean | Si vrai, masque les lignes filtrées. |

**Returns:**
int[] - Retourne les index de toutes les lignes masquées.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Supprime un filtre de date.

**Remarks**

Si DateTimeGroupingType est Year, seul le paramètre year a un effet. Si DateTiemGroupingType est Month, seuls les paramètres year et month ont un effet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Le type de regroupement |
| année | int | L'année. |
| mois | int | Le mois. |
| jour | int | Le jour. |
| heure | int | L'heure. |
| minute | int | La minute. |
| seconde | int | La seconde. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


Supprime le filtre spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | L'index du filtre spécifique |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


Supprime un filtre pour une colonne de filtre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | int | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| critères | java.lang.String | Le critère spécifié (une chaîne ; par exemple, "101"). Il ne peut être nul ou être l'une des valeurs des cellules dans cette colonne. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


Définit la plage à laquelle l'AutoFiltre spécifié s'applique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| startColumn | int | Indice de colonne de départ. |
| endColumn | int | Index de la colonne de fin. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


Représente la plage à laquelle l'AutoFiltre spécifié s'applique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


Indique si le bouton AutoFilter de cette colonne est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


Afficher toutes les lignes.

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

