---
title: "ErrorBar"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la barre d'erreur d'une série de données."
type: docs
url: /fr/java/com.aspose.cells/errorbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```

Représente la barre d'erreur d'une série de données.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("a1").putValue(2);
         cells.get("a2").putValue(5);
         cells.get("a3").putValue(3);
         cells.get("a4").putValue(6);
         cells.get("b1").putValue(4);
         cells.get("b2").putValue(3);
         cells.get("b3").putValue(6);
         cells.get("b4").putValue(7);
 
         cells.get("C1").putValue("Q1");
         cells.get("C2").putValue("Q2");
         cells.get("C3").putValue("Y1");
         cells.get("C4").putValue("Y2");
 
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 11, 0, 27, 10);
 
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:B4", true);
 
         chart.getNSeries().setCategoryData("C1:C4");
 
         for(int i = 0; i <chart.getNSeries().getCount(); i ++)
         {
         		Series aseries = chart.getNSeries().get(i);
         		aseries.getYErrorBar().setDisplayType(ErrorBarDisplayType.MINUS);
         		aseries.getYErrorBar().setType(ErrorBarType.FIXED_VALUE);
         		aseries.getYErrorBar().setAmount(5);
         }
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | Représente la quantité de barre d'erreur. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [getBeginType()](#getBeginType--) | Spécifie une pointe de flèche pour le début d'une ligne. |
| [getCapType()](#getCapType--) | Spécifie les embouts de fin. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Représente la [Color](../../com.aspose.cells/color) de la ligne. |
| [getCompoundType()](#getCompoundType--) | Spécifie le type de ligne composé |
| [getDashType()](#getDashType--) | Spécifie le type de ligne en tirets |
| [getDisplayType()](#getDisplayType--) | Représente le type d'affichage de la barre d'erreur. |
| [getEndArrowLength()](#getEndArrowLength--) | Spécifie la longueur de la pointe de flèche pour l'extrémité d'une ligne. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Spécifie la largeur de la pointe de flèche pour l'extrémité d'une ligne. |
| [getEndType()](#getEndType--) | Spécifie une pointe de flèche pour l'extrémité d'une ligne. |
| [getFormattingType()](#getFormattingType--) | Obtient le type de format. |
| [getGradientFill()](#getGradientFill--) | Représente un remplissage en dégradé. |
| [getJoinType()](#getJoinType--) | Spécifie les embouts de jointure. |
| [getMinusValue()](#getMinusValue--) | Représente la quantité d'erreur négative lorsque le type de barre d'erreur est Custom. |
| [getPlusValue()](#getPlusValue--) | Représente la quantité d'erreur positive lorsque le type de barre d'erreur est Custom. |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | Indique si le formatage des barres d'erreur utilise un T-top. |
| [getStyle()](#getStyle--) | Représente le style de la ligne. |
| [getThemeColor()](#getThemeColor--) | Obtient la couleur du thème. |
| [getTransparency()](#getTransparency--) | Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [getType()](#getType--) | Représente le type de quantité de la barre d'erreur. |
| [getWeight()](#getWeight--) | Obtient le [WeightType](../../com.aspose.cells/weighttype) de la ligne. |
| [getWeightPt()](#getWeightPt--) | Obtient le poids de la ligne en unité de points. |
| [getWeightPx()](#getWeightPx--) | Obtient le poids de la ligne en unité de pixels. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indique si ce style de ligne est attribué automatiquement. |
| [isAutomaticColor()](#isAutomaticColor--) | Indique si la couleur de la ligne est attribuée automatiquement. |
| [isVisible()](#isVisible--) | Représente si la ligne est visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | Représente la quantité de barre d'erreur. |
| [setAuto(boolean value)](#setAuto-boolean-) | Indique si ce style de ligne est attribué automatiquement. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [setBeginType(int value)](#setBeginType-int-) | Spécifie une pointe de flèche pour le début d'une ligne. |
| [setCapType(int value)](#setCapType-int-) | Spécifie les embouts de fin. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Représente la [Color](../../com.aspose.cells/color) de la ligne. |
| [setCompoundType(int value)](#setCompoundType-int-) | Spécifie le type de ligne composé |
| [setDashType(int value)](#setDashType-int-) | Spécifie le type de ligne en tirets |
| [setDisplayType(int value)](#setDisplayType-int-) | Représente le type d'affichage de la barre d'erreur. |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Spécifie la longueur de la pointe de flèche pour l'extrémité d'une ligne. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Spécifie la largeur de la pointe de flèche pour l'extrémité d'une ligne. |
| [setEndType(int value)](#setEndType-int-) | Spécifie une pointe de flèche pour l'extrémité d'une ligne. |
| [setFormattingType(int value)](#setFormattingType-int-) | Définit le type de format. |
| [setJoinType(int value)](#setJoinType-int-) | Spécifie les embouts de jointure. |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | Représente la quantité d'erreur négative lorsque le type de barre d'erreur est Custom. |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | Représente la quantité d'erreur positive lorsque le type de barre d'erreur est Custom. |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | Indique si le formatage des barres d'erreur utilise un T-top. |
| [setStyle(int value)](#setStyle-int-) | Représente le style de la ligne. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Définit la couleur du thème. |
| [setTransparency(double value)](#setTransparency-double-) | Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [setType(int value)](#setType-int-) | Représente le type de quantité de la barre d'erreur. |
| [setVisible(boolean value)](#setVisible-boolean-) | Représente si la ligne est visible. |
| [setWeight(int value)](#setWeight-int-) | Définit le [WeightType](../../com.aspose.cells/weighttype) de la ligne. |
| [setWeightPt(double value)](#setWeightPt-double-) | Définit le poids de la ligne en unité de points. |
| [setWeightPx(double value)](#setWeightPx-double-) | Définit le poids de la ligne en unité de pixels. |
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
### getAmount() {#getAmount--}
```
public double getAmount()
```


Représente la quantité de barre d'erreur.

**Remarks**

La quantité doit être supérieure ou égale à zéro.

**Returns:**
double
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Spécifie la longueur de la pointe de flèche pour le début d'une ligne.

Voir [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Spécifie la largeur de la pointe de flèche pour le début d'une ligne.

Voir [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Spécifie une pointe de flèche pour le début d'une ligne.

Voir [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Spécifie les embouts de fin.

Voir [LineCapType](../../com.aspose.cells/linecaptype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Représente la [Color](../../com.aspose.cells/color) de la ligne.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Spécifie le type de ligne composé

Voir [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Spécifie le type de ligne en tirets

Voir [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```


Représente le type d'affichage de la barre d'erreur.

Voir [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Spécifie la longueur de la pointe de flèche pour l'extrémité d'une ligne.

Voir [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Spécifie la largeur de la pointe de flèche pour l'extrémité d'une ligne.

Voir [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Spécifie une pointe de flèche pour l'extrémité d'une ligne.

Voir [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Obtient le type de format.

Voir [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Représente un remplissage en dégradé.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Spécifie les embouts de jointure.

Voir [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```


Représente la quantité d'erreur négative lorsque le type de barre d'erreur est Custom.

**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```


Représente la quantité d'erreur positive lorsque le type de barre d'erreur est Custom.

**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```


Indique si le formatage des barres d'erreur utilise un T-top.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Représente le style de la ligne.

Voir [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Obtient la couleur du thème.

**Remarks**

Si la couleur de premier plan n'est pas une couleur de thème, NULL sera renvoyé.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Représente le type de quantité de la barre d'erreur.

Voir [ErrorBarType](../../com.aspose.cells/errorbartype).

**Example**

```
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         Series aseries = chart.getNSeries().get(0);
         //Gets custom error bar type
         /*ErrorBarType*/int errBarType = aseries.getYErrorBar().getType();
         //Sets custom error bar type
         aseries.getYErrorBar().setType(ErrorBarType.CUSTOM);
         aseries.getYErrorBar().setPlusValue("=Sheet1!A1");
         aseries.getYErrorBar().setMinusValue("=Sheet1!A2");
```

**Returns:**
int
### getWeight() {#getWeight--}
```
public int getWeight()
```


Obtient le [WeightType](../../com.aspose.cells/weighttype) de la ligne.

Voir [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Obtient le poids de la ligne en unité de points.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Obtient le poids de la ligne en unité de pixels.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAuto() {#isAuto--}
```
public boolean isAuto()
```


Indique si ce style de ligne est attribué automatiquement.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Indique si la couleur de la ligne est attribuée automatiquement.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Représente si la ligne est visible.

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




### setAmount(double value) {#setAmount-double-}
```
public void setAmount(double value)
```


Représente la quantité de barre d'erreur.

**Remarks**

La quantité doit être supérieure ou égale à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


Indique si ce style de ligne est attribué automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


Spécifie la longueur de la pointe de flèche pour le début d'une ligne.

Voir [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


Spécifie la largeur de la pointe de flèche pour le début d'une ligne.

Voir [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


Spécifie une pointe de flèche pour le début d'une ligne.

Voir [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Spécifie les embouts de fin.

Voir [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Représente la [Color](../../com.aspose.cells/color) de la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Spécifie le type de ligne composé

Voir [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


Spécifie le type de ligne en tirets

Voir [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```


Représente le type d'affichage de la barre d'erreur.

Voir [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


Spécifie la longueur de la pointe de flèche pour l'extrémité d'une ligne.

Voir [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


Spécifie la largeur de la pointe de flèche pour l'extrémité d'une ligne.

Voir [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


Spécifie une pointe de flèche pour l'extrémité d'une ligne.

Voir [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


Définit le type de format.

Voir [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Spécifie les embouts de jointure.

Voir [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```


Représente la quantité d'erreur négative lorsque le type de barre d'erreur est Custom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```


Représente la quantité d'erreur positive lorsque le type de barre d'erreur est Custom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```


Indique si le formatage des barres d'erreur utilise un T-top.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Représente le style de la ligne.

Voir [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Définit la couleur du thème.

**Remarks**

Si la couleur de premier plan n'est pas une couleur de thème, NULL sera renvoyé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Représente le type de quantité de la barre d'erreur.

Voir [ErrorBarType](../../com.aspose.cells/errorbartype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Représente si la ligne est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


Définit le [WeightType](../../com.aspose.cells/weighttype) de la ligne.

Voir [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


Définit le poids de la ligne en unité de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


Définit le poids de la ligne en unité de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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

