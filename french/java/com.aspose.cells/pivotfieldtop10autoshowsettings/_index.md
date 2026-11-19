---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les paramètres AutoShow Top 10 pour un champ pivot."
type: docs
url: /fr/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

Représente les paramètres AutoShow Top 10 pour un champ pivot.

**Remarks**

Dans xls : Implémentation des filtres top 10 dans Xls via Top 10 AutoShow. Dans les fichiers ooxml : le format de fichier ooxml sous-jacent prend en charge Top10 AutoShow, mais l'interface utilisateur d'Excel 2007 et ultérieure ne fournit l'accès que via le filtre Top10. Si la compatibilité XLS n'est pas requise, il est recommandé d'utiliser le filtre Top10 à la place.

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
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ de tableau croisé dynamique spécifié. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | Spécifie l'index du champ de données pour le classement AutoShow. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | Indique si un filtre "Top 10 AutoShow" est appliqué à ce champ. |
| [isTop()](#isTop--) | Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indique si un filtre "Top 10 AutoShow" est appliqué à ce champ. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ de tableau croisé dynamique spécifié. |
| [setRankBy(int value)](#setRankBy-int-) | Spécifie l'index du champ de données pour le classement AutoShow. |
| [setTop(boolean value)](#setTop-boolean-) | Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant. |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ de tableau croisé dynamique spécifié.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


Spécifie l'index du champ de données pour le classement AutoShow. Représente l'index du champ d'affichage automatique. -1 signifie le champ PivotField lui‑même. Il doit s'agir de l'index des champs de données.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indique si un filtre "Top 10 AutoShow" est appliqué à ce champ.

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indique si un filtre "Top 10 AutoShow" est appliqué à ce champ.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ de tableau croisé dynamique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


Spécifie l'index du champ de données pour le classement AutoShow. Représente l'index du champ d'affichage automatique. -1 signifie le champ PivotField lui‑même. Il doit s'agir de l'index des champs de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant.

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

