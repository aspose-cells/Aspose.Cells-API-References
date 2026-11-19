---
title: "PivotShowValuesSetting"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les paramètres d'affichage des valeurs lorsque le calcul ShowDataAs est utilisé."
type: docs
url: /fr/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

Représente les paramètres d'affichage des valeurs lorsque le calcul ShowDataAs est utilisé.

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
 
         PivotField dataField = pivot.getDataFields().get(0);
         // Display value as percentage of the grand total
         dataField.showValuesAs(PivotShowValuesAsType.PERCENTAGE_OF_TOTAL, 0, PivotShowValuesSetting.NEXT_PIVOT_ITEM);
         // Get the display calculation setting of data field
         PivotShowValuesSetting settings = dataField.getShowValuesSetting();
         System.out.println(settings.getShowValuesAs());
 
          pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Champs

| Champ | Description |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | Index d'élément de base spécial : utilisez l'élément pivot suivant. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | Index d'élément de base spécial : utilisez l'élément pivot précédent. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Représente le champ de base pour un calcul ShowDataAs lorsque le calcul ShowDataAs est utilisé. |
| [getBaseFieldName()](#getBaseFieldName--) | Obtient la légende du champ de base du pivot. |
| [getBaseItemCaption()](#getBaseItemCaption--) | Obtient la légende de l'élément pivot dans le champ de base. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Représente l'index personnalisé de l'élément pivot dans le champ de base lorsque le calcul ShowDataAs est utilisé. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | Représente le type de l'élément pivot de base dans le champ de base lorsque le calcul ShowDataAs est utilisé. |
| [getCalculationType()](#getCalculationType--) | Représente la façon d'afficher les valeurs d'un champ de données dans le rapport pivot. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | Obtient la façon d'afficher les valeurs d'un champ de données dans le rapport pivot. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Représente le champ de base pour un calcul ShowDataAs lorsque le calcul ShowDataAs est utilisé. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Représente l'index personnalisé de l'élément pivot dans le champ de base lorsque le calcul ShowDataAs est utilisé. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | Représente le type de l'élément pivot de base dans le champ de base lorsque le calcul ShowDataAs est utilisé. |
| [setCalculationType(int value)](#setCalculationType-int-) | Représente la façon d'afficher les valeurs d'un champ de données dans le rapport pivot. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | Définit la façon d'afficher les valeurs d'un champ de données dans le rapport pivot. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


Indice d'élément de base spécial : utilisez l'élément pivot suivant. Valide pour les calculs « Show Values As » ; effectif dans Excel 2010 et versions ultérieures.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


Indice d'élément de base spécial : utilisez l'élément pivot précédent. Valide pour les calculs « Show Values As » ; effectif dans Excel 2010 et versions ultérieures.

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Représente le champ de base pour un calcul ShowDataAs lorsque le calcul ShowDataAs est utilisé.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


Obtient la légende du champ de base du pivot.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


Obtient la légende de l'élément pivot dans le champ de base.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Représente l'index personnalisé de l'élément pivot dans le champ de base lorsque le calcul ShowDataAs est utilisé.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


Représente le type de l'élément pivot de base dans le champ de base lorsque le calcul ShowDataAs est utilisé. Parce que PivotItemPosition.Custom est uniquement en lecture, si vous devez définir PivotItemPosition.Custom, veuillez définir l'attribut PivotField.BaseItemIndex.

Voir [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotShowValuesSetting.BaseItem. Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


Représente la façon d'afficher les valeurs d'un champ de données dans le rapport pivot.

Voir [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotShowValuesSetting.ShowValuesAs. Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getShowValuesAs() {#getShowValuesAs--}
```
public int getShowValuesAs()
```


Obtient la façon d'afficher les valeurs d'un champ de données dans le rapport pivot.

Voir [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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




### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


Représente le champ de base pour un calcul ShowDataAs lorsque le calcul ShowDataAs est utilisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Représente l'index personnalisé de l'élément pivot dans le champ de base lorsque le calcul ShowDataAs est utilisé.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


Représente le type de l'élément pivot de base dans le champ de base lorsque le calcul ShowDataAs est utilisé. Parce que PivotItemPosition.Custom est uniquement en lecture, si vous devez définir PivotItemPosition.Custom, veuillez définir l'attribut PivotField.BaseItemIndex.

Voir [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotShowValuesSetting.BaseItem. Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


Représente la façon d'afficher les valeurs d'un champ de données dans le rapport pivot.

Voir [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotShowValuesSetting.ShowValuesAs. Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


Définit la façon d'afficher les valeurs d'un champ de données dans le rapport pivot.

Voir [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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

