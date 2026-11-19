---
title: "FilterColumn"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un filtre pour une colonne unique ou une colonne du tableau."
type: docs
url: /fr/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

Représente un filtre pour une colonne unique ou une colonne du tableau.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | Obtient [ColorFilter](../../com.aspose.cells/colorfilter) pour filtrer les données par couleur. |
| [getCustomFilters()](#getCustomFilters--) | Obtient [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) pour filtrer les données selon des critères personnalisés. |
| [getDynamicFilter()](#getDynamicFilter--) | Obtient [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) pour filtrer avec des critères dynamiques. |
| [getFieldIndex()](#getFieldIndex--) | Obtient le décalage de colonne dans la plage. |
| [getFilter()](#getFilter--) | Obtient la condition du filtrage des données. |
| [getFilterType()](#getFilterType--) | Obtient le type du filtrage des données. |
| [getFilterValues()](#getFilterValues--) | Obtient [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) pour filtrer les données par libellés ou date/heure. |
| [getIconFilter()](#getIconFilter--) | Obtient [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) pour filtrer les données par icône. |
| [getMultipleFilters()](#getMultipleFilters--) | Obtient [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) pour filtrer les données par libellés ou date/heure. |
| [getTop10Filter()](#getTop10Filter--) | Obtient [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) pour filtrer les données par rang. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | Indique si le bouton AutoFilter de cette colonne est visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | Sélectionne tout. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | Obtient [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) pour filtrer les données selon des critères personnalisés. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | Indique si le bouton AutoFilter de cette colonne est visible. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Définit le décalage de colonne dans la plage. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | Définit la condition du filtrage des données. |
| [setFilterType(int value)](#setFilterType-int-) | Définit le type du filtrage des données. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | Obtient [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) pour filtrer les données par libellés ou date/heure. |
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
### getColorFilter() {#getColorFilter--}
```
public ColorFilter getColorFilter()
```


Obtient [ColorFilter](../../com.aspose.cells/colorfilter) pour filtrer les données par couleur.

**Remarks**

Définit [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) comme [FilterType.COLOR\_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER) d'abord, sinon Null sera renvoyé.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


Obtient [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) pour filtrer les données selon des critères personnalisés.

**Remarks**

NOTE : Ce mutateur de cette propriété est maintenant obsolète. Au lieu de cela, veuillez utiliser la propriété [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) en la définissant comme [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Cette propriété sera supprimée 12 mois plus tard, à partir de juin 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


Obtient [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) pour filtrer avec des critères dynamiques.

**Remarks**

Avant d'utiliser cette propriété, veuillez vous assurer que [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) est [FilterType.DYNAMIC\_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER), sinon null sera renvoyé.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Obtient le décalage de colonne dans la plage.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


Obtient la condition du filtrage des données.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Au lieu de cela, veuillez utiliser la propriété correspondante selon [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). Et pour le type de filtre [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), l'objet renvoyé est désormais [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) au lieu de [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Cette propriété sera supprimée 12 mois plus tard, à partir d'octobre 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Obtient le type du filtrage des données.

Voir [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

L'objet de filtre correspondant sera créé lorsque cette propriété est définie et la propriété correspondante doit être utilisée pour obtenir l'objet de filtre en conséquence :

| FilterType | Propriété |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Returns:**
int
### getFilterValues() {#getFilterValues--}
```
public FilterValueCollection getFilterValues()
```


Obtient [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) pour filtrer les données par libellés ou date/heure.

**Remarks**

Définit [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) comme [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) d'abord, sinon Null sera renvoyé.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


Obtient [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) pour filtrer les données par icône.

**Remarks**

Avant d'utiliser cette propriété, veuillez vous assurer que [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) est [FilterType.ICON\_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER), sinon null sera renvoyé.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


Obtient [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) pour filtrer les données par libellés ou date/heure.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété FilterColumn.FilterValues. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


Obtient [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) pour filtrer les données par rang.

**Remarks**

Avant d'utiliser cette propriété, veuillez vous assurer que [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) est [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10), sinon null sera renvoyé.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDropdownVisible() {#isDropdownVisible--}
```
public boolean isDropdownVisible()
```


Indique si le bouton AutoFilter de cette colonne est visible.

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




### selectAll() {#selectAll--}
```
public void selectAll()
```


Sélectionne tout.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


Obtient [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) pour filtrer les données selon des critères personnalisés.

**Remarks**

NOTE : Ce mutateur de cette propriété est maintenant obsolète. Au lieu de cela, veuillez utiliser la propriété [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) en la définissant comme [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Cette propriété sera supprimée 12 mois plus tard, à partir de juin 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


Indique si le bouton AutoFilter de cette colonne est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Définit le décalage de colonne dans la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


Définit la condition du filtrage des données.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Au lieu de cela, veuillez utiliser la propriété correspondante selon [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). Et pour le type de filtre [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), l'objet renvoyé est désormais [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) au lieu de [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Cette propriété sera supprimée 12 mois plus tard, à partir d'octobre 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


Définit le type du filtrage des données.

Voir [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

L'objet de filtre correspondant sera créé lorsque cette propriété est définie et la propriété correspondante doit être utilisée pour obtenir l'objet de filtre en conséquence :

| FilterType | Propriété |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


Obtient [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) pour filtrer les données par libellés ou date/heure.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété FilterColumn.FilterValues. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) |  |

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

