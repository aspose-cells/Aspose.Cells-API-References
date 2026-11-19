---
title: "PivotItem"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un élément dans un rapport PivotField."
type: docs
url: /fr/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

Représente un élément dans un rapport PivotField.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
          //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Hide the first item
         PivotItem item = rowField.getPivotItems().get(0);          
         item.setHidden(true);
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Champs

| Champ | Description |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | Indice sentinelle de sélection de tous les éléments de page (0x7FFD, indice non valide) |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | Obtient la valeur date/heure de l'élément pivot. Si la valeur est null, elle renverra DateTime.MinValue. |
| [getDoubleValue()](#getDoubleValue--) | Obtient la valeur double de l'élément pivot. Si la valeur est null ou n'est pas un nombre, elle renverra 0. |
| [getFormula()](#getFormula--) | Obtient la formule de cet élément calculé. |
| [getIndex()](#getIndex--) | Obtient l'indice de l'élément pivot dans le champ de cache. |
| [getName()](#getName--) | Obtient le nom de l'élément pivot. |
| [getPosition()](#getPosition--) | Spécifier l'index de cet élément dans tous les PivotItems du champ. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | Spécifier l'index de position dans les PivotItems sous le même nœud parent. |
| [getStringValue()](#getStringValue--) | Obtient la valeur chaîne de l'élément pivot. Si la valeur est nulle, elle renverra "" |
| [getValue()](#getValue--) | Obtient la valeur de l'élément pivot |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | Définit si l'élément pivot est masqué. |
| [isCalculatedItem()](#isCalculatedItem--) | Indique si cet élément pivot est un élément de formule calculée. |
| [isDetailHidden()](#isDetailHidden--) | Obtient si le détail de cet élément pivot est masqué. |
| [isFormula()](#isFormula--) | Indique si cet élément pivot est un élément de formule calculée. |
| [isHidden()](#isHidden--) | Obtient si l'élément pivot est masqué. |
| [isHideDetail()](#isHideDetail--) | Obtient si l'élément pivot masque le détail. |
| [isMissing()](#isMissing--) | Indique si l'élément a été supprimé de la source de données. |
| [move(int offset)](#move-int-) | Déplace l'élément vers le haut ou vers le bas dans le champ pivot |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | Déplace l'élément vers le haut ou vers le bas |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | Définit si le détail de cet élément pivot est masqué. |
| [setFormula(boolean value)](#setFormula-boolean-) | Indique si cet élément pivot est un élément de formule calculée. |
| [setHidden(boolean value)](#setHidden-boolean-) | Définit si l'élément pivot est masqué. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | Définit si l'élément pivot masque le détail. |
| [setIndex(int value)](#setIndex-int-) | Obtient l'indice de l'élément pivot dans le champ de cache. |
| [setName(String value)](#setName-java.lang.String-) | Obtient le nom de l'élément pivot. |
| [setPosition(int value)](#setPosition-int-) | Spécifier l'index de cet élément dans tous les PivotItems du champ. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | Spécifier l'index de position dans les PivotItems sous le même nœud parent. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


Indice sentinelle de sélection de tous les éléments de page (0x7FFD, indice non valide)

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
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Obtient la valeur date/heure de l'élément pivot. Si la valeur est null, elle renverra DateTime.MinValue.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Obtient la valeur double de l'élément pivot. Si la valeur est null ou n'est pas un nombre, elle renverra 0.

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtient la formule de cet élément calculé. Fonctionne uniquement lorsque cet élément est un élément calculé.

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'indice de l'élément pivot dans le champ de cache.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotItem.Position. Cette méthode sera supprimée 6 mois plus tard à compter d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de l'élément pivot.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Spécifier l'index de cet élément dans tous les PivotItems du champ.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


Spécifier l'index de position dans les PivotItems sous le même nœud parent.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.MoveItem(PivotFieldType, string[],bool,int). Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Obtient la valeur chaîne de l'élément pivot. Si la valeur est nulle, elle renverra ""

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Obtient la valeur de l'élément pivot

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


Définit si l'élément pivot est masqué.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Aspose.Cells.Pivot.PivotItem.IsHidden. Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2012. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


Indique si cet élément pivot est un élément de formule calculée.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


Obtient si le détail de cet élément pivot est masqué.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Indique si cet élément pivot est un élément de formule calculée.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotItem.IsCalculatedItem. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Obtient si l'élément pivot est masqué.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Obtient si l'élément pivot masque le détail.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotItem.IsDetailHidden. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


Indique si l'élément a été supprimé de la source de données.

**Remarks**

Vrai signifie que cette valeur a été supprimée de la source de données.

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


Déplace l'élément vers le haut ou vers le bas dans le champ pivot

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| décalage | int | Le nombre de déplacements vers le haut ou vers le bas. Déplacez l'élément vers le haut si cette valeur est inférieure à zéro ; déplacez l'élément vers le bas si cette valeur est supérieure à zéro. |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


Déplace l'élément vers le haut ou vers le bas

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.MoveItem(PivotFieldType, string[],bool,int) ou la méthode PivotItem.Move(int). Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| décalage | int | Le nombre de déplacements vers le haut ou vers le bas. Déplacez l'élément vers le haut si cette valeur est inférieure à zéro ; déplacez l'élément vers le bas si cette valeur est supérieure à zéro. |
| isSameParent | boolean | Spécifier si l'opération de déplacement se trouve dans le même nœud parent ou non |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


Définit si le détail de cet élément pivot est masqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


Indique si cet élément pivot est un élément de formule calculée.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotItem.IsCalculatedItem. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Définit si l'élément pivot est masqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


Définit si l'élément pivot masque le détail.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotItem.IsDetailHidden. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


Obtient l'indice de l'élément pivot dans le champ de cache.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotItem.Position. Cette méthode sera supprimée 6 mois plus tard à compter d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Obtient le nom de l'élément pivot.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Spécifier l'index de cet élément dans tous les PivotItems du champ.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


Spécifier l'index de position dans les PivotItems sous le même nœud parent.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.MoveItem(PivotFieldType, string[],bool,int). Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

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

