---
title: "Timeline"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Description résumée de la vue Timeline En raison de MS Excel 2003 qui ne prend pas en charge Timeline"
type: docs
url: /fr/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

Description résumée de la vue Timeline. En raison de MS Excel, Excel 2003 ne prend pas en charge Timeline.

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
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | Obtient la légende de ce Timeline. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | Le niveau de temps actuel du Timeline. |
| [getHeightPixel()](#getHeightPixel--) | Renvoie ou définit la hauteur du timeline spécifié, en pixels. |
| [getLeftPixel()](#getLeftPixel--) | Renvoie ou définit le décalage horizontal de la forme du timeline par rapport à sa colonne de gauche, en pixels. |
| [getName()](#getName--) | Renvoie ou définit le nom du Timeline spécifié |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | Obtient la plage de date et d'heure sélectionnée. |
| [getSelectionLevel()](#getSelectionLevel--) | Obtient le niveau de temps auquel la sélection actuelle a été faite pour le Timeline. |
| [getShape()](#getShape--) | Renvoie l'objet [TimelineShape](../../com.aspose.cells/timelineshape) associé à ce Timeline. |
| [getShowHeader()](#getShowHeader--) | Indique s'il faut afficher l'en-tête de ce timeline. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | Indique s'il faut afficher la barre de défilement horizontale. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | Indique s'il faut afficher le libellé de sélection. |
| [getShowTimeLevel()](#getShowTimeLevel--) | Indique s'il faut afficher la zone de sélection déroulante du niveau de temps. |
| [getStartDate()](#getStartDate--) | Obtient la date de début de la position de défilement de la plage temporelle de ce [Timeline](../../com.aspose.cells/timeline). |
| [getTopPixel()](#getTopPixel--) | Renvoie ou définit le décalage vertical de la forme du timeline par rapport à sa ligne supérieure, en pixels. |
| [getWidthPixel()](#getWidthPixel--) | Renvoie ou définit la largeur du timeline spécifié, en pixels. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | Sélectionner l'élément entre les dates et heures. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Définit la légende de ce Timeline. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | Le niveau de temps actuel du Timeline. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Renvoie ou définit la hauteur du timeline spécifié, en pixels. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Renvoie ou définit le décalage horizontal de la forme du timeline par rapport à sa colonne de gauche, en pixels. |
| [setName(String value)](#setName-java.lang.String-) | Renvoie ou définit le nom du Timeline spécifié |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | Définit le niveau de temps auquel la sélection actuelle a été faite pour le Timeline. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | Indique s'il faut afficher l'en-tête de ce timeline. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | Indique s'il faut afficher la barre de défilement horizontale. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | Indique s'il faut afficher le libellé de sélection. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | Indique s'il faut afficher la zone de sélection déroulante du niveau de temps. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Définit la date de début de la position de défilement de la plage temporelle de ce [Timeline](../../com.aspose.cells/timeline). |
| [setTopPixel(int value)](#setTopPixel-int-) | Renvoie ou définit le décalage vertical de la forme du timeline par rapport à sa ligne supérieure, en pixels. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Renvoie ou définit la largeur du timeline spécifié, en pixels. |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


Obtient la légende de ce Timeline.

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


Le niveau de temps actuel du Timeline.

Voir [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Renvoie ou définit la hauteur du timeline spécifié, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Height. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Renvoie ou définit le décalage horizontal de la forme du timeline par rapport à sa colonne de gauche, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Left. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Renvoie ou définit le nom du Timeline spécifié

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


Obtient la plage de date et d'heure sélectionnée.

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


Obtient le niveau de temps auquel la sélection actuelle a été faite pour le Timeline.

Voir [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


Renvoie l'objet [TimelineShape](../../com.aspose.cells/timelineshape) associé à ce Timeline.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


Indique s'il faut afficher l'en-tête de ce timeline.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


Indique s'il faut afficher la barre de défilement horizontale.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


Indique s'il faut afficher le libellé de sélection.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


Indique s'il faut afficher la zone de sélection déroulante du niveau de temps.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Obtient la date de début de la position de défilement de la plage temporelle de ce [Timeline](../../com.aspose.cells/timeline).

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Renvoie ou définit le décalage vertical de la forme du timeline par rapport à sa ligne supérieure, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Top. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Renvoie ou définit la largeur du timeline spécifié, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Width. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


Sélectionner l'élément entre les dates et heures.

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | La date et l'heure de début |
| end | [DateTime](../../com.aspose.cells/datetime) | La date et l'heure de fin |
| calculer | boolean | Indique s'il faut calculer les tableaux croisés dynamiques relatifs |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Définit la légende de ce Timeline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


Le niveau de temps actuel du Timeline.

Voir [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Renvoie ou définit la hauteur du timeline spécifié, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Height. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Renvoie ou définit le décalage horizontal de la forme du timeline par rapport à sa colonne de gauche, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Left. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Renvoie ou définit le nom du Timeline spécifié

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


Définit le niveau de temps auquel la sélection actuelle a été faite pour le Timeline.

Voir [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


Indique s'il faut afficher l'en-tête de ce timeline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


Indique s'il faut afficher la barre de défilement horizontale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


Indique s'il faut afficher le libellé de sélection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


Indique s'il faut afficher la zone de sélection déroulante du niveau de temps.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Définit la date de début de la position de défilement de la plage temporelle de ce [Timeline](../../com.aspose.cells/timeline).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Renvoie ou définit le décalage vertical de la forme du timeline par rapport à sa ligne supérieure, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Top. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Renvoie ou définit la largeur du timeline spécifié, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Width. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

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

