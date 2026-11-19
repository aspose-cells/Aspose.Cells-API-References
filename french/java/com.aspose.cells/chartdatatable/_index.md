---
title: "ChartDataTable"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un tableau de données de graphique."
type: docs
url: /fr/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

Représente un tableau de données de graphique.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         chart.setShowDataTable(true);
 
         //Getting Chart Table
         ChartDataTable chartTable = chart.getChartDataTable();
 
         //Setting Chart Table Font Color
         chartTable.getFont().setColor(com.aspose.cells.Color.getRed());
 
         //Setting Legend Key VisibilityOptions
         chartTable.setShowLegendKey(false);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtient le mode d'affichage de l'arrière-plan |
| [getBorder()](#getBorder--) | Renvoie un objet Border qui représente la bordure de l'objet |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Obtient un objet [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) qui représente le paramètre de police du tableau de données de graphique spécifié. |
| [getShowLegendKey()](#getShowLegendKey--) | Vrai si la clé de légende de l'étiquette de données est visible. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | Vrai si le tableau de données de graphique possède des bordures de cellules horizontales |
| [hasBorderOutline()](#hasBorderOutline--) | Vrai si le tableau de données de graphique possède des bordures de contour |
| [hasBorderVertical()](#hasBorderVertical--) | Vrai si le tableau de données de graphique possède des bordures de cellules verticales |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | Vrai si le tableau de données de graphique possède des bordures de cellules horizontales |
| [hasOutlineBorder()](#hasOutlineBorder--) | Vrai si le tableau de données de graphique possède des bordures de contour |
| [hasVerticalBorder()](#hasVerticalBorder--) | Vrai si le tableau de données de graphique possède des bordures de cellules verticales |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Définit le mode d'affichage de l'arrière-plan |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | Vrai si le tableau de données de graphique possède des bordures de cellules horizontales |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | Vrai si le tableau de données de graphique possède des bordures de contour |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | Vrai si le tableau de données de graphique possède des bordures de cellules verticales |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | Vrai si le tableau de données de graphique possède des bordures de cellules horizontales |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | Vrai si le tableau de données de graphique possède des bordures de contour |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | Vrai si le tableau de données de graphique possède des bordures de cellules verticales |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Vrai si la clé de légende de l'étiquette de données est visible. |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Obtient le mode d'affichage de l'arrière-plan

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Renvoie un objet Border qui représente la bordure de l'objet

**Returns:**
[Line](../../com.aspose.cells/line)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


Obtient un objet [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) qui représente le paramètre de police du tableau de données de graphique spécifié.

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Vrai si la clé de légende de l'étiquette de données est visible.

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


Vrai si le tableau de données de graphique possède des bordures de cellules horizontales

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ChartDataTable.HasHorizontalBorder. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


Vrai si le tableau de données de graphique possède des bordures de contour

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ChartDataTable.HasOutlineBorder. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


Vrai si le tableau de données de graphique possède des bordures de cellules verticales

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ChartDataTable.HasVerticalBorder. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


Vrai si le tableau de données de graphique possède des bordures de cellules horizontales

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


Vrai si le tableau de données de graphique possède des bordures de contour

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


Vrai si le tableau de données de graphique possède des bordures de cellules verticales

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Définit le mode d'affichage de l'arrière-plan

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


Vrai si le tableau de données de graphique possède des bordures de cellules horizontales

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ChartDataTable.HasHorizontalBorder. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


Vrai si le tableau de données de graphique possède des bordures de contour

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ChartDataTable.HasOutlineBorder. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


Vrai si le tableau de données de graphique possède des bordures de cellules verticales

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ChartDataTable.HasVerticalBorder. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


Vrai si le tableau de données de graphique possède des bordures de cellules horizontales

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


Vrai si le tableau de données de graphique possède des bordures de contour

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


Vrai si le tableau de données de graphique possède des bordures de cellules verticales

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Vrai si la clé de légende de l'étiquette de données est visible.

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

