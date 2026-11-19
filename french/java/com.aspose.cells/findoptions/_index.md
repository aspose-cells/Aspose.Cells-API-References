---
title: "FindOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de recherche."
type: docs
url: /fr/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

Représente les options de recherche.

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Indique si la chaîne recherchée est sensible à la casse. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | Obtient une valeur qui indique si la conversion de la chaîne recherchée en données numériques. |
| [getLookAtType()](#getLookAtType--) | Regarder le type. |
| [getLookInType()](#getLookInType--) | Regarder dans le type. |
| [getRange()](#getRange--) | Obtient et définit la plage recherchée. |
| [getRegexKey()](#getRegexKey--) | Indique si la clé recherchée est une expression régulière. |
| [getSearchBackward()](#getSearchBackward--) | Indique si la recherche se fait en arrière pour les cellules. |
| [getSearchNext()](#getSearchNext--) | Ordre de recherche. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | Indique si l'ordre de recherche est par lignes ou par colonnes. |
| [getStyle()](#getStyle--) | Le format à rechercher. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Indique si le type de valeur de la cellule recherchée doit être le même que la clé recherchée. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Indique si la plage recherchée est définie. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Indique si la chaîne recherchée est sensible à la casse. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Définit une valeur qui indique si la conversion de la valeur de chaîne recherchée en données numériques. |
| [setLookAtType(int value)](#setLookAtType-int-) | Regarder le type. |
| [setLookInType(int value)](#setLookInType-int-) | Regarder dans le type. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Définit la plage recherchée. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | Indique si la clé recherchée est une expression régulière. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | Indique si la recherche se fait en arrière pour les cellules. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | Ordre de recherche. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | Indique si l'ordre de recherche est par lignes ou par colonnes. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Le format à rechercher. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | Indique si le type de valeur de la cellule recherchée doit être le même que la clé recherchée. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Indique si la chaîne recherchée est sensible à la casse.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Obtient une valeur qui indique si la conversion de la chaîne recherchée en données numériques.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


Regarder le type.

Voir [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Lorsque [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) est vrai et que l'utilisateur a spécifié la règle exacte pour l'expression régulière, pour des raisons de performances cette propriété doit être définie sur [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). Sinon, nous reformulerons la clé de recherche afin de garantir qu'elle puisse correspondre au type spécifique. Par exemple, lorsque le type est [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (c'est la valeur par défaut pour cette propriété), nous ajouterons automatiquement des caractères génériques au début et à la fin de la clé de recherche. Dans ce cas, les expressions régulières deviendront plus complexes et les performances diminueront également.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


Regarder dans le type.

Voir [LookInType](../../com.aspose.cells/lookintype).

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


Obtient et définit la plage recherchée.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


Indique si la clé recherchée est une expression régulière. Si vrai, la clé recherchée sera prise comme expression régulière et analysée. Sinon, la clé sera analysée selon les règles de MS Excel.

**Remarks**

Même si la clé de recherche a été spécifiée comme expression régulière, elle peut être reformulée selon le [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) spécifié. Par exemple, lorsque le type est [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (c'est la valeur par défaut pour ces options), des caractères génériques seront ajoutés automatiquement au début et à la fin de la clé de recherche pour garantir que la correspondance soit vérifiée comme \"contains\". Dans ce cas, les expressions régulières deviendront plus complexes et les performances diminueront également. Ainsi, pour des raisons de performances, si l'utilisateur a spécifié la règle exacte pour l'expression régulière, il n'est pas nécessaire d'utiliser [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) comme contrainte supplémentaire et l'utilisateur peut le définir sur [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) pour obtenir de meilleures performances.

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


Indique si la recherche se fait en arrière pour les cellules.

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


Ordre de recherche. Vrai : rechercher suivant. Faux : rechercher précédent.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété FindOptions.SearchBackward. Cette propriété sera supprimée 12 mois plus tard, depuis novembre 2018. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


Indique si l'ordre de recherche est par lignes ou par colonnes.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Le format à rechercher.

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


Indique si le type de valeur de la cellule recherchée doit être le même que la clé recherchée.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


Indique si la plage recherchée est définie.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Indique si la chaîne recherchée est sensible à la casse.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Définit une valeur qui indique si la conversion de la valeur de chaîne recherchée en données numériques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


Regarder le type.

Voir [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Lorsque [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) est vrai et que l'utilisateur a spécifié la règle exacte pour l'expression régulière, pour des raisons de performances cette propriété doit être définie sur [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). Sinon, nous reformulerons la clé de recherche afin de garantir qu'elle puisse correspondre au type spécifique. Par exemple, lorsque le type est [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (c'est la valeur par défaut pour cette propriété), nous ajouterons automatiquement des caractères génériques au début et à la fin de la clé de recherche. Dans ce cas, les expressions régulières deviendront plus complexes et les performances diminueront également.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


Regarder dans le type.

Voir [LookInType](../../com.aspose.cells/lookintype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


Définit la plage recherchée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | la plage recherchée. |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


Indique si la clé recherchée est une expression régulière. Si vrai, la clé recherchée sera prise comme expression régulière et analysée. Sinon, la clé sera analysée selon les règles de MS Excel.

**Remarks**

Même si la clé de recherche a été spécifiée comme expression régulière, elle peut être reformulée selon le [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) spécifié. Par exemple, lorsque le type est [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (c'est la valeur par défaut pour ces options), des caractères génériques seront ajoutés automatiquement au début et à la fin de la clé de recherche pour garantir que la correspondance soit vérifiée comme \"contains\". Dans ce cas, les expressions régulières deviendront plus complexes et les performances diminueront également. Ainsi, pour des raisons de performances, si l'utilisateur a spécifié la règle exacte pour l'expression régulière, il n'est pas nécessaire d'utiliser [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) comme contrainte supplémentaire et l'utilisateur peut le définir sur [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) pour obtenir de meilleures performances.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


Indique si la recherche se fait en arrière pour les cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


Ordre de recherche. Vrai : rechercher suivant. Faux : rechercher précédent.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété FindOptions.SearchBackward. Cette propriété sera supprimée 12 mois plus tard, depuis novembre 2018. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


Indique si l'ordre de recherche est par lignes ou par colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Le format à rechercher.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


Indique si le type de valeur de la cellule recherchée doit être le même que la clé recherchée.

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

