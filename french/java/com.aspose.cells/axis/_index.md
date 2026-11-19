---
title: "Axis"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente un axe d'un graphique."
type: docs
url: /fr/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

Encapsule l'objet qui représente un axe d'un graphique.

**Example**

À partir des codes suivants, vous pouvez apprendre comment définir l'unité, la valeur maximale et minimale de l'Axe.

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
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(4);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(20);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
         //Set the max value of value axis
         chart.getValueAxis().setMaxValue(200);
         //Set the min value of value axis
         chart.getValueAxis().setMinValue(0);
         //Set the major unit
         chart.getValueAxis().setMajorUnit(25);
         //Category(X) axis crosses at the maxinum value.
         chart.getValueAxis().setCrossType(CrossType.MAXIMUM);
         //Set he number of categories or series between tick-mark labels. 
         chart.getCategoryAxis().setTickLabelSpacing(2);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Obtient le [getArea()](../../com.aspose.cells/axis\#getArea--). |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | Représente si l'axe des valeurs croise l'axe des catégories entre les catégories. |
| [getAxisLabels()](#getAxisLabels--) | Obtient les libellés de l'axe après l'appel de la méthode Chart.Calculate(). |
| [getAxisLine()](#getAxisLine--) | Obtient l'apparence d'un Axe. |
| [getAxisTexts()](#getAxisTexts--) | Obtient les libellés de l'axe après l'appel de la méthode Chart.Calculate(). |
| [getBaseUnitScale()](#getBaseUnitScale--) | Représente l'échelle de l'unité de base pour l'axe des catégories. |
| [getBins()](#getBins--) | Représente les intervalles sur l'axe d'un graphique (Histogramme/Pareto) |
| [getCategoryType()](#getCategoryType--) | Représente le type de l'axe des catégories. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | Représente le point sur l'axe des valeurs où l'axe des catégories le croise. |
| [getCrossType()](#getCrossType--) | Représente le [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) sur l'axe spécifié où l'autre axe le croise. |
| [getCustUnit()](#getCustUnit--) | Spécifie une valeur personnalisée pour l'unité d'affichage. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | Spécifie une valeur personnalisée pour l'unité d'affichage. |
| [getCustomUnit()](#getCustomUnit--) | Spécifie une valeur personnalisée pour l'unité d'affichage. |
| [getDisplayUnit()](#getDisplayUnit--) | Représente l'étiquette d'unité pour l'axe spécifié. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | Représente une étiquette d'unité sur un axe dans le graphique spécifié. |
| [getLogBase()](#getLogBase--) | Représente la base logarithmique. |
| [getMajorGridLines()](#getMajorGridLines--) | Représente les lignes de grille majeures sur l'axe d'un graphique. |
| [getMajorTickMark()](#getMajorTickMark--) | Représente le type de repère principal pour l'axe spécifié. |
| [getMajorUnit()](#getMajorUnit--) | Représente les unités majeures pour l'axe. |
| [getMajorUnitScale()](#getMajorUnitScale--) | Représente l'échelle de l'unité majeure pour l'axe de catégorie. |
| [getMaxValue()](#getMaxValue--) | Représente la valeur maximale sur l'axe des valeurs. |
| [getMinValue()](#getMinValue--) | Représente la valeur minimale sur l'axe des valeurs. |
| [getMinorGridLines()](#getMinorGridLines--) | Représente les quadrillages mineurs sur un axe de graphique. |
| [getMinorTickMark()](#getMinorTickMark--) | Représente le type de repère mineur pour l'axe spécifié. |
| [getMinorUnit()](#getMinorUnit--) | Représente les unités mineures pour l'axe. |
| [getMinorUnitScale()](#getMinorUnitScale--) | Représente l'échelle de l'unité majeure pour l'axe de catégorie. |
| [getTickLabelPosition()](#getTickLabelPosition--) | Représente la position des étiquettes de repères sur l'axe spécifié. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | Représente le nombre de catégories ou de séries entre les étiquettes de repères. |
| [getTickLabels()](#getTickLabels--) | Renvoie un objet [getTickLabels()](../../com.aspose.cells/axis\\#getTickLabels--) qui représente les étiquettes de repères pour l'axe spécifié. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | Renvoie ou définit le nombre de catégories ou de séries entre les repères. |
| [getTitle()](#getTitle--) | Obtient le titre de cet axe dans le graphique. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | Indique si les étiquettes doivent être affichées à plusieurs niveaux. |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | Indique si l'espacement des étiquettes de repère est automatique |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | Indique si l'unité majeure de l'axe est attribuée automatiquement. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | Indique si la valeur maximale est attribuée automatiquement. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | Indique si la valeur minimale est attribuée automatiquement. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | Indique si l'unité mineure de l'axe est attribuée automatiquement. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | Représente si l'unité de base est automatique. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | Représente si l'étiquette d'unité d'affichage est affichée sur l'axe spécifié. |
| [isLogarithmic()](#isLogarithmic--) | Représente si le type d'échelle de l'axe des valeurs est logarithmique ou non. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | Représente si Microsoft Excel trace les points de données du dernier au premier. |
| [isVisible()](#isVisible--) | Représente si l'axe est visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | Indique si l'espacement des étiquettes de repère est automatique |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | Indique si l'unité majeure de l'axe est attribuée automatiquement. |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | Indique si la valeur maximale est attribuée automatiquement. |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | Indique si la valeur minimale est attribuée automatiquement. |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | Indique si l'unité mineure de l'axe est attribuée automatiquement. |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | Représente si l'axe des valeurs croise l'axe des catégories entre les catégories. |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | Représente si l'unité de base est automatique. |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | Représente l'échelle de l'unité de base pour l'axe des catégories. |
| [setCategoryType(int value)](#setCategoryType-int-) | Représente le type de l'axe des catégories. |
| [setCrossAt(double value)](#setCrossAt-double-) | Représente le point sur l'axe des valeurs où l'axe des catégories le croise. |
| [setCrossType(int value)](#setCrossType-int-) | Représente le [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) sur l'axe spécifié où l'autre axe le croise. |
| [setCustUnit(int value)](#setCustUnit-int-) | Spécifie une valeur personnalisée pour l'unité d'affichage. |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | Spécifie une valeur personnalisée pour l'unité d'affichage. |
| [setCustomUnit(int value)](#setCustomUnit-int-) | Spécifie une valeur personnalisée pour l'unité d'affichage. |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | Représente l'étiquette d'unité pour l'axe spécifié. |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | Représente si l'étiquette d'unité d'affichage est affichée sur l'axe spécifié. |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | Indique si les étiquettes doivent être affichées à plusieurs niveaux. |
| [setLogBase(double value)](#setLogBase-double-) | Représente la base logarithmique. |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | Représente si le type d'échelle de l'axe des valeurs est logarithmique ou non. |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | Représente le type de repère principal pour l'axe spécifié. |
| [setMajorUnit(double value)](#setMajorUnit-double-) | Représente les unités majeures pour l'axe. |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | Représente l'échelle de l'unité majeure pour l'axe de catégorie. |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | Représente la valeur maximale sur l'axe des valeurs. |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | Représente la valeur minimale sur l'axe des valeurs. |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | Représente le type de repère mineur pour l'axe spécifié. |
| [setMinorUnit(double value)](#setMinorUnit-double-) | Représente les unités mineures pour l'axe. |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | Représente l'échelle de l'unité majeure pour l'axe de catégorie. |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | Représente si Microsoft Excel trace les points de données du dernier au premier. |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | Représente la position des étiquettes de repères sur l'axe spécifié. |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | Représente le nombre de catégories ou de séries entre les étiquettes de repères. |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | Renvoie ou définit le nombre de catégories ou de séries entre les repères. |
| [setVisible(boolean value)](#setVisible-boolean-) | Représente si l'axe est visible. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Obtient le [getArea()](../../com.aspose.cells/axis\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


Représente si l'axe des valeurs croise l'axe des catégories entre les catégories.

**Remarks**

Cette propriété s'applique uniquement aux axes de catégorie, et ne s'applique pas aux graphiques 3D.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


Obtient les libellés de l'axe après l'appel de la méthode Chart.Calculate().

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Axis.GetAxisTexts. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2023. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


Obtient l'apparence d'un Axe.

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


Obtient les libellés de l'axe après l'appel de la méthode Chart.Calculate().

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


Représente l'échelle de l'unité de base pour l'axe des catégories.

Voir [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Ne prend effet que lorsque la propriété CategoryType est définie sur TimeScale.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


Représente les intervalles sur l'axe d'un graphique (Histogramme/Pareto)

**Remarks**

Uniquement pour les graphiques Histogramme ou Pareto.

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


Représente le type de l'axe des catégories.

Voir [CategoryType](../../com.aspose.cells/categorytype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCrossAt() {#getCrossAt--}
```
public double getCrossAt()
```


Représente le point sur l'axe des valeurs où l'axe des catégories le croise.

**Remarks**

Le nombre doit être un entier lorsqu'il s'applique à l'axe des catégories. Et la valeur doit être comprise entre 1 et 31999.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


Représente le [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) sur l'axe spécifié où l'autre axe le croise.

Voir [CrossType](../../com.aspose.cells/crosstype).

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


Spécifie une valeur personnalisée pour l'unité d'affichage.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété Axis.CustomUnit. Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2023. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


Spécifie une valeur personnalisée pour l'unité d'affichage.

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


Spécifie une valeur personnalisée pour l'unité d'affichage.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété Axis.CustomDisplayUnit. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


Représente l'étiquette d'unité pour l'axe spécifié.

Voir [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


Représente une étiquette d'unité sur un axe dans le graphique spécifié. Les étiquettes d'unité sont utiles pour tracer de grandes valeurs - par exemple, en millions ou en milliards.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


Représente la base logarithmique. La valeur par défaut est 10.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


Représente les lignes de grille majeures sur l'axe d'un graphique.

**Example**

```
         chart.getValueAxis().getMajorGridLines().setVisible(false);
         chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

**Returns:**
[Line](../../com.aspose.cells/line)
### getMajorTickMark() {#getMajorTickMark--}
```
public int getMajorTickMark()
```


Représente le type de repère principal pour l'axe spécifié.

Voir [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


Représente les unités majeures pour l'axe.

**Remarks**

Les unités majeures doivent être supérieures à zéro.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


Représente l'échelle de l'unité majeure pour l'axe de catégorie.

Voir [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         /*TimeUnit*/int majorUnitScale = chart.getCategoryAxis().getMajorUnitScale(); //get
         chart.getCategoryAxis().setMajorUnitScale(majorUnitScale); //set
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


Représente la valeur maximale sur l'axe des valeurs.

**Remarks**

Le type maxValue ne peut être que double ou DateTime.

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


Représente la valeur minimale sur l'axe des valeurs.

**Remarks**

Le type minValue ne peut être que double ou DateTime.

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


Représente les quadrillages mineurs sur un axe de graphique.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


Représente le type de repère mineur pour l'axe spécifié.

Voir [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


Représente les unités mineures pour l'axe.

**Remarks**

Les unités mineures doivent être supérieures à zéro.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


Représente l'échelle de l'unité majeure pour l'axe de catégorie.

Voir [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMinorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMinorUnit(2);
```

**Returns:**
int
### getTickLabelPosition() {#getTickLabelPosition--}
```
public int getTickLabelPosition()
```


Représente la position des étiquettes de repères sur l'axe spécifié.

Voir [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


Représente le nombre de catégories ou de séries entre les étiquettes de repères. S'applique uniquement aux axes de catégorie et de séries.

**Remarks**

Le nombre doit être compris entre 1 et 31999.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


Renvoie un objet [getTickLabels()](../../com.aspose.cells/axis\\#getTickLabels--) qui représente les étiquettes de repères pour l'axe spécifié.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


Renvoie ou définit le nombre de catégories ou de séries entre les repères. S'applique uniquement aux axes de catégorie et de séries.

**Remarks**

Le nombre doit être compris entre 1 et 31999.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Obtient le titre de cet axe dans le graphique.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


Indique si les étiquettes doivent être affichées à plusieurs niveaux.

**Remarks**

Valide uniquement pour l'axe des catégories.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


Indique si l'espacement des étiquettes de repère est automatique

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


Indique si l'unité majeure de l'axe est attribuée automatiquement.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


Indique si la valeur maximale est attribuée automatiquement.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


Indique si la valeur minimale est attribuée automatiquement.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


Indique si l'unité mineure de l'axe est attribuée automatiquement.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


Représente si l'unité de base est automatique.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


Représente si l'étiquette d'unité d'affichage est affichée sur l'axe spécifié.

**Remarks**

La valeur par défaut est True. Fonctionne uniquement lorsque [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) n'est pas [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


Représente si le type d'échelle de l'axe des valeurs est logarithmique ou non.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


Représente si Microsoft Excel trace les points de données du dernier au premier.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Représente si l'axe est visible.

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




### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


Indique si l'espacement des étiquettes de repère est automatique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


Indique si l'unité majeure de l'axe est attribuée automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


Indique si la valeur maximale est attribuée automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


Indique si la valeur minimale est attribuée automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


Indique si l'unité mineure de l'axe est attribuée automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


Représente si l'axe des valeurs croise l'axe des catégories entre les catégories.

**Remarks**

Cette propriété s'applique uniquement aux axes de catégorie, et ne s'applique pas aux graphiques 3D.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


Représente si l'unité de base est automatique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


Représente l'échelle de l'unité de base pour l'axe des catégories.

Voir [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Ne prend effet que lorsque la propriété CategoryType est définie sur TimeScale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


Représente le type de l'axe des catégories.

Voir [CategoryType](../../com.aspose.cells/categorytype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


Représente le point sur l'axe des valeurs où l'axe des catégories le croise.

**Remarks**

Le nombre doit être un entier lorsqu'il s'applique à l'axe des catégories. Et la valeur doit être comprise entre 1 et 31999.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


Représente le [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) sur l'axe spécifié où l'autre axe le croise.

Voir [CrossType](../../com.aspose.cells/crosstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


Spécifie une valeur personnalisée pour l'unité d'affichage.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété Axis.CustomUnit. Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2023. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


Spécifie une valeur personnalisée pour l'unité d'affichage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


Spécifie une valeur personnalisée pour l'unité d'affichage.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété Axis.CustomDisplayUnit. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


Représente l'étiquette d'unité pour l'axe spécifié.

Voir [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


Représente si l'étiquette d'unité d'affichage est affichée sur l'axe spécifié.

**Remarks**

La valeur par défaut est True. Fonctionne uniquement lorsque [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) n'est pas [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


Indique si les étiquettes doivent être affichées à plusieurs niveaux.

**Remarks**

Valide uniquement pour l'axe des catégories.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


Représente la base logarithmique. La valeur par défaut est 10.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


Représente si le type d'échelle de l'axe des valeurs est logarithmique ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


Représente le type de repère principal pour l'axe spécifié.

Voir [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


Représente les unités majeures pour l'axe.

**Remarks**

Les unités majeures doivent être supérieures à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


Représente l'échelle de l'unité majeure pour l'axe de catégorie.

Voir [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


Représente la valeur maximale sur l'axe des valeurs.

**Remarks**

Le type maxValue ne peut être que double ou DateTime.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


Représente la valeur minimale sur l'axe des valeurs.

**Remarks**

Le type minValue ne peut être que double ou DateTime.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


Représente le type de repère mineur pour l'axe spécifié.

Voir [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


Représente les unités mineures pour l'axe.

**Remarks**

Les unités mineures doivent être supérieures à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


Représente l'échelle de l'unité majeure pour l'axe de catégorie.

Voir [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


Représente si Microsoft Excel trace les points de données du dernier au premier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


Représente la position des étiquettes de repères sur l'axe spécifié.

Voir [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


Représente le nombre de catégories ou de séries entre les étiquettes de repères. S'applique uniquement aux axes de catégorie et de séries.

**Remarks**

Le nombre doit être compris entre 1 et 31999.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


Renvoie ou définit le nombre de catégories ou de séries entre les repères. S'applique uniquement aux axes de catégorie et de séries.

**Remarks**

Le nombre doit être compris entre 1 et 31999.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Représente si l'axe est visible.

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

