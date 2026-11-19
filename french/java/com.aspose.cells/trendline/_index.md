---
title: "Trendline"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une ligne de tendance dans un graphique."
type: docs
url: /fr/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

Représente une ligne de tendance dans un graphique.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //adding a linear trendline
         int index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR);
         Trendline trendline = chart.getNSeries().get(0).getTrendLines().get(index);
         //Setting the custom name of the trendline.
         trendline.setName("Linear");
         //Displaying the equation on chart
         trendline.setDisplayEquation(true);
         //Displaying the R-Squared value on chart
         trendline.setDisplayRSquared(true);
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique en nuage de points) que le trendline étend vers l'arrière. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [getBeginType()](#getBeginType--) | Spécifie une pointe de flèche pour le début d'une ligne. |
| [getCapType()](#getCapType--) | Spécifie les embouts de fin. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Représente la [Color](../../com.aspose.cells/color) de la ligne. |
| [getCompoundType()](#getCompoundType--) | Spécifie le type de ligne composé |
| [getDashType()](#getDashType--) | Spécifie le type de ligne en tirets |
| [getDataLabels()](#getDataLabels--) | Représente l'objet DataLabels pour la série spécifiée. |
| [getDisplayEquation()](#getDisplayEquation--) | Indique si l'équation de la ligne de tendance est affichée sur le graphique (dans la même étiquette de données que la valeur R-carré). |
| [getDisplayRSquared()](#getDisplayRSquared--) | Indique si la valeur R-carré de la ligne de tendance est affichée sur le graphique (dans la même étiquette de données que l'équation). |
| [getEndArrowLength()](#getEndArrowLength--) | Spécifie la longueur de la pointe de flèche pour l'extrémité d'une ligne. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Spécifie la largeur de la pointe de flèche pour l'extrémité d'une ligne. |
| [getEndType()](#getEndType--) | Spécifie une pointe de flèche pour l'extrémité d'une ligne. |
| [getFormattingType()](#getFormattingType--) | Obtient le type de format. |
| [getForward()](#getForward--) | Renvoie ou définit le nombre de périodes (ou d'unités sur un nuage de points) que la ligne de tendance prolonge vers l'avant. |
| [getGradientFill()](#getGradientFill--) | Représente un remplissage en dégradé. |
| [getIntercept()](#getIntercept--) | Renvoie ou définit le point où la ligne de tendance croise l'axe des valeurs. |
| [getJoinType()](#getJoinType--) | Spécifie les embouts de jointure. |
| [getLegendEntry()](#getLegendEntry--) | Obtient l'entrée de légende correspondant à cette ligne de tendance |
| [getName()](#getName--) | Renvoie le nom de la ligne de tendance. |
| [getOrder()](#getOrder--) | Renvoie ou définit l'ordre de la ligne de tendance (un entier supérieur à 1) lorsque le type de ligne de tendance est Polynomial. |
| [getPeriod()](#getPeriod--) | Renvoie ou définit la période pour la ligne de tendance moyenne mobile. |
| [getStyle()](#getStyle--) | Représente le style de la ligne. |
| [getThemeColor()](#getThemeColor--) | Obtient la couleur du thème. |
| [getTransparency()](#getTransparency--) | Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [getType()](#getType--) | Renvoie le type de ligne de tendance. |
| [getWeight()](#getWeight--) | Obtient le [WeightType](../../com.aspose.cells/weighttype) de la ligne. |
| [getWeightPt()](#getWeightPt--) | Obtient le poids de la ligne en unité de points. |
| [getWeightPx()](#getWeightPx--) | Obtient le poids de la ligne en unité de pixels. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indique si ce style de ligne est attribué automatiquement. |
| [isAutomaticColor()](#isAutomaticColor--) | Indique si la couleur de la ligne est attribuée automatiquement. |
| [isInterceptAuto()](#isInterceptAuto--) | Indique si Microsoft Workbook détermine automatiquement l'interception de la courbe de tendance. |
| [isNameAuto()](#isNameAuto--) | Renvoie si Microsoft Excel détermine automatiquement le nom de la courbe de tendance. |
| [isVisible()](#isVisible--) | Représente si la ligne est visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Indique si ce style de ligne est attribué automatiquement. |
| [setBackward(double value)](#setBackward-double-) | Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique en nuage de points) que le trendline étend vers l'arrière. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [setBeginType(int value)](#setBeginType-int-) | Spécifie une pointe de flèche pour le début d'une ligne. |
| [setCapType(int value)](#setCapType-int-) | Spécifie les embouts de fin. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Représente la [Color](../../com.aspose.cells/color) de la ligne. |
| [setCompoundType(int value)](#setCompoundType-int-) | Spécifie le type de ligne composé |
| [setDashType(int value)](#setDashType-int-) | Spécifie le type de ligne en tirets |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | Indique si l'équation de la ligne de tendance est affichée sur le graphique (dans la même étiquette de données que la valeur R-carré). |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | Indique si la valeur R-carré de la ligne de tendance est affichée sur le graphique (dans la même étiquette de données que l'équation). |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Spécifie la longueur de la pointe de flèche pour l'extrémité d'une ligne. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Spécifie la largeur de la pointe de flèche pour l'extrémité d'une ligne. |
| [setEndType(int value)](#setEndType-int-) | Spécifie une pointe de flèche pour l'extrémité d'une ligne. |
| [setFormattingType(int value)](#setFormattingType-int-) | Définit le type de format. |
| [setForward(double value)](#setForward-double-) | Renvoie ou définit le nombre de périodes (ou d'unités sur un nuage de points) que la ligne de tendance prolonge vers l'avant. |
| [setIntercept(double value)](#setIntercept-double-) | Renvoie ou définit le point où la ligne de tendance croise l'axe des valeurs. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | Définit si Microsoft Workbook détermine automatiquement l'interception de la courbe de tendance. |
| [setJoinType(int value)](#setJoinType-int-) | Spécifie les embouts de jointure. |
| [setName(String value)](#setName-java.lang.String-) | Renvoie le nom de la ligne de tendance. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | Renvoie si Microsoft Excel détermine automatiquement le nom de la courbe de tendance. |
| [setOrder(int value)](#setOrder-int-) | Renvoie ou définit l'ordre de la ligne de tendance (un entier supérieur à 1) lorsque le type de ligne de tendance est Polynomial. |
| [setPeriod(int value)](#setPeriod-int-) | Renvoie ou définit la période pour la ligne de tendance moyenne mobile. |
| [setStyle(int value)](#setStyle-int-) | Représente le style de la ligne. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Définit la couleur du thème. |
| [setTransparency(double value)](#setTransparency-double-) | Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la courbe de tendance s'étend vers l'arrière. Le nombre de périodes doit être supérieur ou égal à zéro. Si le type de graphique est en colonnes, le nombre de périodes doit être compris entre 0 et 0,5.

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
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Représente l'objet DataLabels pour la série spécifiée.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


Représente si l'équation de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que la valeur R-carré). Définir cette propriété sur True active automatiquement les étiquettes de données.

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


Représente si la valeur R-carré de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que l'équation). Définir cette propriété sur True active automatiquement les étiquettes de données.

**Returns:**
boolean
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
### getForward() {#getForward--}
```
public double getForward()
```


Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la courbe de tendance s'étend vers l'avant. Le nombre de périodes doit être supérieur ou égal à zéro.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Représente un remplissage en dégradé.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


Renvoie ou définit le point où la ligne de tendance croise l'axe des valeurs.

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Spécifie les embouts de jointure.

Voir [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Obtient l'entrée de légende correspondant à cette ligne de tendance

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


Renvoie le nom de la ligne de tendance.

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


Renvoie ou définit l'ordre de la courbe de tendance (un entier supérieur à 1) lorsque le type de courbe de tendance est Polynomial. L'ordre doit être compris entre 2 et 6.

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


Renvoie ou définit la période pour la ligne de tendance moyenne mobile.

**Remarks**

Cette valeur doit être comprise entre 2 et 255. Et elle doit être inférieure au nombre de points du graphique dans la série

**Returns:**
int
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


Renvoie le type de ligne de tendance.

Voir [TrendlineType](../../com.aspose.cells/trendlinetype).

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
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


Indique si Microsoft Workbook détermine automatiquement l'interception de la courbe de tendance.

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


Renvoie si Microsoft Excel détermine automatiquement le nom de la courbe de tendance.

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




### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


Indique si ce style de ligne est attribué automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la courbe de tendance s'étend vers l'arrière. Le nombre de périodes doit être supérieur ou égal à zéro. Si le type de graphique est en colonnes, le nombre de périodes doit être compris entre 0 et 0,5.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


Représente si l'équation de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que la valeur R-carré). Définir cette propriété sur True active automatiquement les étiquettes de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


Représente si la valeur R-carré de la courbe de tendance est affichée sur le graphique (dans la même étiquette de données que l'équation). Définir cette propriété sur True active automatiquement les étiquettes de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


Renvoie ou définit le nombre de périodes (ou d'unités sur un graphique de dispersion) que la courbe de tendance s'étend vers l'avant. Le nombre de périodes doit être supérieur ou égal à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


Renvoie ou définit le point où la ligne de tendance croise l'axe des valeurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


Définit si Microsoft Workbook détermine automatiquement l'interception de la courbe de tendance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

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

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Renvoie le nom de la ligne de tendance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


Renvoie si Microsoft Excel détermine automatiquement le nom de la courbe de tendance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Renvoie ou définit l'ordre de la courbe de tendance (un entier supérieur à 1) lorsque le type de courbe de tendance est Polynomial. L'ordre doit être compris entre 2 et 6.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


Renvoie ou définit la période pour la ligne de tendance moyenne mobile.

**Remarks**

Cette valeur doit être comprise entre 2 et 255. Et elle doit être inférieure au nombre de points du graphique dans la série

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

