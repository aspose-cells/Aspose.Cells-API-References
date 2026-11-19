---
title: "Segment"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "description résumée de la vue Slicer"
type: docs
url: /fr/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

description résumée de la vue Slicer

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
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | Ajoute une connexion de tableau croisé dynamique. |
| [clearFilter()](#clearFilter--) | Supprimer les filtres |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Renvoie ou définit la chaîne de texte descriptive (alternative) de l’objet Slicer. |
| [getCaption()](#getCaption--) | Renvoie ou définit la légende du slicer spécifié. |
| [getCaptionVisible()](#getCaptionVisible--) | Renvoie ou définit si l’en-tête affichant la légende du slicer est visible. |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | Renvoie ou définit la largeur de chaque colonne du slicer en points. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | Obtient la largeur de\u807deach column in\u807dthe slicer, en unité de\u807dpixels.\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | Spécifie l’indice zéro‑bas du premier élément du slicer. |
| [getHeight()](#getHeight--) | Renvoie ou définit la hauteur du slicer spécifié, en points. |
| [getHeightPixel()](#getHeightPixel--) | Renvoie ou définit la hauteur du slicer spécifié, en pixels. |
| [getLeftPixel()](#getLeftPixel--) | Renvoie ou définit le décalage horizontal de la forme du slicer par rapport à sa colonne de gauche, en pixels. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | Indique si le verrouillage du ratio d'aspect est activé. |
| [getLockedPosition()](#getLockedPosition--) | Indique si le slicer spécifié peut être déplacé ou redimensionné via l'interface utilisateur. |
| [getName()](#getName--) | Renvoie ou définit le nom du slicer spécifié |
| [getNumberOfColumns()](#getNumberOfColumns--) | Renvoie ou définit le nombre de colonnes du slicer. |
| [getParent()](#getParent--) | Renvoie l'objet [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) qui contient ce slicer. |
| [getPlacement()](#getPlacement--) | Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. |
| [getRowHeight()](#getRowHeight--) | Renvoie ou définit la hauteur de chaque ligne du slicer spécifié en points. |
| [getRowHeightPixel()](#getRowHeightPixel--) | Renvoie ou définit la hauteur de chaque ligne du slicer spécifié, en pixels. |
| [getShape()](#getShape--) | Renvoie l'objet Shape associé au slicer spécifié. |
| [getShowAllItems()](#getShowAllItems--) | Indique s'il faut afficher tous les éléments même s'il n'y a pas de données ou s'ils sont supprimés. |
| [getShowCaption()](#getShowCaption--) | Indique si l'en-tête du slicer est visible. |
| [getShowMissing()](#getShowMissing--) | Indique s'il faut afficher les éléments supprimés de la source de données. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | Indique s'il faut afficher les éléments supprimés de la source de données. |
| [getSlicerCache()](#getSlicerCache--) | Renvoie l'objet SlicerCache associé au slicer. |
| [getSortOrderType()](#getSortOrderType--) | Indique le type de tri des éléments. |
| [getStyleType()](#getStyleType--) | Spécifiez le type de style de slicer intégré. |
| [getTitle()](#getTitle--) | Spécifie le titre de l'objet Slicer actuel. |
| [getTopPixel()](#getTopPixel--) | Renvoie ou définit le décalage vertical de la forme du slicer par rapport à sa ligne supérieure, en pixels. |
| [getWidth()](#getWidth--) | Renvoie ou définit la largeur du slicer spécifié, en points. |
| [getWidthPixel()](#getWidthPixel--) | Renvoie ou définit la largeur du slicer spécifié, en pixels. |
| [getWorksheet()](#getWorksheet--) | Renvoie l'objet [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) qui contient ce slicer. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | Indique si la forme du slicer est verrouillée. |
| [isPrintable()](#isPrintable--) | Indique si l'objet slicer est imprimable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Actualisation des éléments du slicer à partir des tableaux croisés dynamiques associés. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | Supprime la connexion du tableau croisé dynamique. |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **Remarques** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Renvoie ou définit la chaîne de texte descriptive (alternative) de l’objet Slicer. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Renvoie ou définit la légende du slicer spécifié. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | Renvoie ou définit si l’en-tête affichant la légende du slicer est visible. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Renvoie ou définit la largeur de chaque colonne du slicer en points. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | Définit la largeur de\\u807dchaque colonne dans\\u807dle slicer, en unité de\\u807dpixels.\\u807d |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | Spécifie l’indice zéro‑bas du premier élément du slicer. |
| [setHeight(double value)](#setHeight-double-) | Renvoie ou définit la hauteur du slicer spécifié, en points. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Renvoie ou définit la hauteur du slicer spécifié, en pixels. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Renvoie ou définit le décalage horizontal de la forme du slicer par rapport à sa colonne de gauche, en pixels. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indique si la forme du slicer est verrouillée. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | Indique si le verrouillage du ratio d'aspect est activé. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | Indique si le slicer spécifié peut être déplacé ou redimensionné via l'interface utilisateur. |
| [setName(String value)](#setName-java.lang.String-) | Renvoie ou définit le nom du slicer spécifié |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Renvoie ou définit le nombre de colonnes du slicer. |
| [setPlacement(int value)](#setPlacement-int-) | Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Indique si l'objet slicer est imprimable. |
| [setRowHeight(double value)](#setRowHeight-double-) | Renvoie ou définit la hauteur de chaque ligne du slicer spécifié en points. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | Renvoie ou définit la hauteur de chaque ligne du slicer spécifié, en pixels. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Indique s'il faut afficher tous les éléments même s'il n'y a pas de données ou s'ils sont supprimés. |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | Indique si l'en-tête du slicer est visible. |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | Indique s'il faut afficher les éléments supprimés de la source de données. |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | Indique s'il faut afficher les éléments supprimés de la source de données. |
| [setSortOrderType(int value)](#setSortOrderType-int-) | Indique le type de tri des éléments. |
| [setStyleType(int value)](#setStyleType-int-) | Spécifiez le type de style de slicer intégré. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Spécifie le titre de l'objet Slicer actuel. |
| [setTopPixel(int value)](#setTopPixel-int-) | Renvoie ou définit le décalage vertical de la forme du slicer par rapport à sa ligne supérieure, en pixels. |
| [setWidth(double value)](#setWidth-double-) | Renvoie ou définit la largeur du slicer spécifié, en points. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Renvoie ou définit la largeur du slicer spécifié, en pixels. |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | Supprimer les libellés de filtre sélectionnés. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


Ajoute une connexion de tableau croisé dynamique.

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | L'objet PivotTable |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Supprimer les filtres

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Renvoie ou définit la chaîne de texte descriptive (alternative) de l’objet Slicer.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


Renvoie ou définit la légende du slicer spécifié.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


Renvoie ou définit si l'en-tête qui affiche la légende du segment est visible. La valeur par défaut est true.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Renvoie ou définit la largeur de chaque colonne du slicer en points.

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


Obtient la largeur de\u807deach column in\u807dthe slicer, en unité de\u807dpixels.\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


Spécifie l’indice zéro‑bas du premier élément du slicer.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Renvoie ou définit la hauteur du slicer spécifié, en points.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.HeightPt. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Renvoie ou définit la hauteur du slicer spécifié, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Height. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Renvoie ou définit le décalage horizontal de la forme du slicer par rapport à sa colonne de gauche, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Left. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


Indique si le verrouillage du ratio d'aspect est activé.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


Indique si le slicer spécifié peut être déplacé ou redimensionné via l'interface utilisateur.

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Renvoie ou définit le nom du slicer spécifié

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Renvoie ou définit le nombre de colonnes du segment. La valeur par défaut est 1.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


Renvoie l'objet [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) qui contient ce segment. Lecture seule.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul.

Voir [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Renvoie ou définit la hauteur de chaque ligne du slicer spécifié en points.

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


Renvoie ou définit la hauteur de chaque ligne du slicer spécifié, en pixels.

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


Renvoie l'objet Shape associé au segment spécifié. Lecture seule.

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indique s'il faut afficher tous les éléments même s'il n'y a pas de données ou s'ils sont supprimés. La valeur par défaut est true ;

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


Indique si l'en-tête du segment est visible. La valeur par défaut est true.

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


Indique s'il faut afficher les éléments supprimés de la source de données.

**Remarks**

Fonctionne uniquement lorsque [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) est true.

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


Indique s'il faut afficher les éléments supprimés de la source de données.

Voir [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Fonctionne uniquement lorsque [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) est true.

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


Renvoie l'objet SlicerCache associé au segment. Lecture seule.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


Indique le type de tri des éléments.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


Spécifiez le type de style de segment intégré. Le type par défaut est SlicerStyleLight1.

Voir [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


Spécifie le titre de l'objet Slicer actuel.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Renvoie ou définit le décalage vertical de la forme du slicer par rapport à sa ligne supérieure, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Top. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Renvoie ou définit la largeur du slicer spécifié, en points.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.WidthPt. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Renvoie ou définit la largeur du slicer spécifié, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Width. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Renvoie l'objet [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) qui contient ce segment. Lecture seule.

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Indique si la forme du slicer est verrouillée.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Indique si l'objet slicer est imprimable.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Example**

```
         slicer.removePivotConnection(pivot);
```

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




### refresh() {#refresh--}
```
public void refresh()
```


Actualisation des éléments du slicer à partir des tableaux croisés dynamiques associés.

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


Supprime la connexion du tableau croisé dynamique.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | L'objet PivotTable |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

Si vous souhaitez sélectionner tous les éléments, veuillez utiliser la méthode [clearFilter()](../../com.aspose.cells/slicer\#clearFilter--) .

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| étiquettes | java.lang.String[] | Étiquettes sélectionnées. |
| ajouter | boolean | False signifie ne sélectionner que ces étiquettes et désélectionner les autres. True signifie conserver les éléments sélectionnés précédemment et sélectionner ces étiquettes. |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Renvoie ou définit la chaîne de texte descriptive (alternative) de l’objet Slicer.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Renvoie ou définit la légende du slicer spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


Renvoie ou définit si l'en-tête qui affiche la légende du segment est visible. La valeur par défaut est true.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Renvoie ou définit la largeur de chaque colonne du slicer en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


Définit la largeur de\\u807dchaque colonne dans\\u807dle slicer, en unité de\\u807dpixels.\\u807d

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


Spécifie l’indice zéro‑bas du premier élément du slicer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Renvoie ou définit la hauteur du slicer spécifié, en points.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.HeightPt. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Renvoie ou définit la hauteur du slicer spécifié, en pixels.

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


Renvoie ou définit le décalage horizontal de la forme du slicer par rapport à sa colonne de gauche, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Left. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indique si la forme du slicer est verrouillée.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


Indique si le verrouillage du ratio d'aspect est activé.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


Indique si le slicer spécifié peut être déplacé ou redimensionné via l'interface utilisateur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Renvoie ou définit le nom du slicer spécifié

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Renvoie ou définit le nombre de colonnes du segment. La valeur par défaut est 1.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul.

Voir [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Indique si l'objet slicer est imprimable.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Renvoie ou définit la hauteur de chaque ligne du slicer spécifié en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


Renvoie ou définit la hauteur de chaque ligne du slicer spécifié, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Indique s'il faut afficher tous les éléments même s'il n'y a pas de données ou s'ils sont supprimés. La valeur par défaut est true ;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


Indique si l'en-tête du segment est visible. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


Indique s'il faut afficher les éléments supprimés de la source de données.

**Remarks**

Fonctionne uniquement lorsque [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


Indique s'il faut afficher les éléments supprimés de la source de données.

Voir [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Fonctionne uniquement lorsque [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


Indique le type de tri des éléments.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


Spécifiez le type de style de segment intégré. Le type par défaut est SlicerStyleLight1.

Voir [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Spécifie le titre de l'objet Slicer actuel.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) . Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Renvoie ou définit le décalage vertical de la forme du slicer par rapport à sa ligne supérieure, en pixels.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Top. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Renvoie ou définit la largeur du slicer spécifié, en points.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.WidthPt. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Renvoie ou définit la largeur du slicer spécifié, en pixels.

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
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


Supprimer les libellés de filtre sélectionnés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| étiquettes | java.lang.String[] | Les étiquettes. |

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

