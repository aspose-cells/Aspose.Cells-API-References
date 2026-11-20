---
title: "Axis"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das eine Achse eines Diagramms darstellt."
type: docs
url: /de/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

Kapselt das Objekt, das eine Achse eines Diagramms darstellt.

**Example**

Aus den folgenden Codebeispielen können Sie lernen, wie Sie Einheit, Maximal‑ und Minimalwert der Achse festlegen.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Ruft die [getArea()](../../com.aspose.cells/axis\#getArea--) ab. |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | Gibt an, ob die Werte‑Achse die Kategorien‑Achse zwischen den Kategorien schneidet. |
| [getAxisLabels()](#getAxisLabels--) | Ruft die Beschriftungen der Achse nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getAxisLine()](#getAxisLine--) | Ruft das Erscheinungsbild einer Achse ab. |
| [getAxisTexts()](#getAxisTexts--) | Ruft die Beschriftungen der Achse nach dem Aufruf der Methode Chart.Calculate() ab. |
| [getBaseUnitScale()](#getBaseUnitScale--) | Stellt die Basiseinheitsskala für die Kategorien‑Achse dar. |
| [getBins()](#getBins--) | Stellt Klassen (Bins) auf einer Diagramm‑Achse (Histogramm/Pareto) dar. |
| [getCategoryType()](#getCategoryType--) | Stellt den Typ der Kategorien‑Achse dar. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | Stellt den Punkt auf der Werte‑Achse dar, an dem die Kategorien‑Achse sie schneidet. |
| [getCrossType()](#getCrossType--) | Stellt die [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) auf der angegebenen Achse dar, an der die andere Achse kreuzt. |
| [getCustUnit()](#getCustUnit--) | Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| [getCustomUnit()](#getCustomUnit--) | Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| [getDisplayUnit()](#getDisplayUnit--) | Stellt die Einheitbeschriftung für die angegebene Achse dar. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | Stellt eine Einheitbeschriftung auf einer Achse im angegebenen Diagramm dar. |
| [getLogBase()](#getLogBase--) | Stellt die logarithmische Basis dar. |
| [getMajorGridLines()](#getMajorGridLines--) | Stellt Hauptgitternetzlinien auf einer Diagrammachse dar. |
| [getMajorTickMark()](#getMajorTickMark--) | Stellt den Typ der Hauptteilstriche für die angegebene Achse dar. |
| [getMajorUnit()](#getMajorUnit--) | Stellt die Hauptintervalle für die Achse dar. |
| [getMajorUnitScale()](#getMajorUnitScale--) | Stellt die Skalierung der Hauptintervalle für die Kategorienachse dar. |
| [getMaxValue()](#getMaxValue--) | Stellt den Maximalwert auf der Werteachse dar. |
| [getMinValue()](#getMinValue--) | Stellt den Minimalwert auf der Werteachse dar. |
| [getMinorGridLines()](#getMinorGridLines--) | Stellt Neben\-gitternetzlinien auf einer Diagrammachse dar. |
| [getMinorTickMark()](#getMinorTickMark--) | Stellt den Typ der Neben\-teilstriche für die angegebene Achse dar. |
| [getMinorUnit()](#getMinorUnit--) | Stellt die Nebenintervalle für die Achse dar. |
| [getMinorUnitScale()](#getMinorUnitScale--) | Stellt die Skalierung der Hauptintervalle für die Kategorienachse dar. |
| [getTickLabelPosition()](#getTickLabelPosition--) | Stellt die Position der Teilstrich\-Beschriftungen auf der angegebenen Achse dar. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | Stellt die Anzahl der Kategorien oder Serien zwischen Teilstrich\-Beschriftungen dar. |
| [getTickLabels()](#getTickLabels--) | Gibt ein [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--)\-Objekt zurück, das die Teilstrich\-Beschriftungen für die angegebene Achse darstellt. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | Gibt die Anzahl der Kategorien oder Serien zwischen Teilstrichen zurück oder legt sie fest. |
| [getTitle()](#getTitle--) | Liest den Titel dieser Achse im Diagramm. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | Gibt an, ob die Beschriftungen mehrstufig angezeigt werden sollen. |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | Gibt an, ob der Abstand der Teilstrich\-Beschriftungen automatisch ist |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | Gibt an, ob die Haupteinheit der Achse automatisch zugewiesen wird. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | Gibt an, ob der Maximalwert automatisch zugewiesen wird. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | Gibt an, ob der Minimalwert automatisch zugewiesen wird. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | Gibt an, ob die Nebeneinheit der Achse automatisch zugewiesen wird. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | Gibt an, ob die Basiseinheit automatisch ist. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | Gibt an, ob das Anzeigeeinheiten‑Label auf der angegebenen Achse angezeigt wird. |
| [isLogarithmic()](#isLogarithmic--) | Gibt an, ob der Skalierungstyp der Werteachse logarithmisch ist oder nicht. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | Gibt an, ob Microsoft Excel Datenpunkte von zuletzt nach zuerst darstellt. |
| [isVisible()](#isVisible--) | Gibt an, ob die Achse sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | Gibt an, ob der Abstand der Teilstrich\-Beschriftungen automatisch ist |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | Gibt an, ob die Haupteinheit der Achse automatisch zugewiesen wird. |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | Gibt an, ob der Maximalwert automatisch zugewiesen wird. |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | Gibt an, ob der Minimalwert automatisch zugewiesen wird. |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | Gibt an, ob die Nebeneinheit der Achse automatisch zugewiesen wird. |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | Gibt an, ob die Werte‑Achse die Kategorien‑Achse zwischen den Kategorien schneidet. |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | Gibt an, ob die Basiseinheit automatisch ist. |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | Stellt die Basiseinheitsskala für die Kategorien‑Achse dar. |
| [setCategoryType(int value)](#setCategoryType-int-) | Stellt den Typ der Kategorien‑Achse dar. |
| [setCrossAt(double value)](#setCrossAt-double-) | Stellt den Punkt auf der Werte‑Achse dar, an dem die Kategorien‑Achse sie schneidet. |
| [setCrossType(int value)](#setCrossType-int-) | Stellt die [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) auf der angegebenen Achse dar, an der die andere Achse kreuzt. |
| [setCustUnit(int value)](#setCustUnit-int-) | Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| [setCustomUnit(int value)](#setCustomUnit-int-) | Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | Stellt die Einheitbeschriftung für die angegebene Achse dar. |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | Gibt an, ob das Anzeigeeinheiten‑Label auf der angegebenen Achse angezeigt wird. |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | Gibt an, ob die Beschriftungen mehrstufig angezeigt werden sollen. |
| [setLogBase(double value)](#setLogBase-double-) | Stellt die logarithmische Basis dar. |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | Gibt an, ob der Skalierungstyp der Werteachse logarithmisch ist oder nicht. |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | Stellt den Typ der Hauptteilstriche für die angegebene Achse dar. |
| [setMajorUnit(double value)](#setMajorUnit-double-) | Stellt die Hauptintervalle für die Achse dar. |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | Stellt die Skalierung der Hauptintervalle für die Kategorienachse dar. |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | Stellt den Maximalwert auf der Werteachse dar. |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | Stellt den Minimalwert auf der Werteachse dar. |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | Stellt den Typ der Neben\-teilstriche für die angegebene Achse dar. |
| [setMinorUnit(double value)](#setMinorUnit-double-) | Stellt die Nebenintervalle für die Achse dar. |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | Stellt die Skalierung der Hauptintervalle für die Kategorienachse dar. |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | Gibt an, ob Microsoft Excel Datenpunkte von zuletzt nach zuerst darstellt. |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | Stellt die Position der Teilstrich\-Beschriftungen auf der angegebenen Achse dar. |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | Stellt die Anzahl der Kategorien oder Serien zwischen Teilstrich\-Beschriftungen dar. |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | Gibt die Anzahl der Kategorien oder Serien zwischen Teilstrichen zurück oder legt sie fest. |
| [setVisible(boolean value)](#setVisible-boolean-) | Gibt an, ob die Achse sichtbar ist. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArea() {#getArea--}
```
public Area getArea()
```


Ruft die [getArea()](../../com.aspose.cells/axis\#getArea--) ab.

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


Gibt an, ob die Werte‑Achse die Kategorien‑Achse zwischen den Kategorien schneidet.

**Remarks**

Diese Eigenschaft gilt nur für Kategorienachsen und nicht für 3‑D‑Diagramme.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


Ruft die Beschriftungen der Achse nach dem Aufruf der Methode Chart.Calculate() ab.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode Axis.GetAxisTexts. Diese Eigenschaft wird 12 Monate nach November 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


Ruft das Erscheinungsbild einer Achse ab.

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


Ruft die Beschriftungen der Achse nach dem Aufruf der Methode Chart.Calculate() ab.

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


Stellt die Basiseinheitsskala für die Kategorien‑Achse dar.

Siehe [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Wirkt nur, wenn die Eigenschaft CategoryType auf TimeScale gesetzt ist.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


Stellt Klassen (Bins) auf einer Diagramm‑Achse (Histogramm/Pareto) dar.

**Remarks**

Nur für Histogramm‑ oder Pareto‑Diagramme.

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


Stellt den Typ der Kategorien‑Achse dar.

Siehe [CategoryType](../../com.aspose.cells/categorytype).

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


Stellt den Punkt auf der Werte‑Achse dar, an dem die Kategorien‑Achse sie schneidet.

**Remarks**

Die Zahl sollte eine ganze Zahl sein, wenn sie für die Kategorienachse gilt. Und der Wert muss zwischen 1 und 31999 liegen.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


Stellt die [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) auf der angegebenen Achse dar, an der die andere Achse kreuzt.

Siehe [CrossType](../../com.aspose.cells/crosstype).

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Axis.CustomUnit. Diese Eigenschaft wird 12 Monate nach Januar 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an.

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Axis.CustomDisplayUnit. Diese Eigenschaft wird 12 Monate nach Februar 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


Stellt die Einheitbeschriftung für die angegebene Achse dar.

Siehe [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


Stellt ein Einheitsetikett auf einer Achse im angegebenen Diagramm dar. Einheitsetiketten sind nützlich, um große Werte zu visualisieren – zum Beispiel in Millionen oder Milliarden.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


Gibt die logarithmische Basis an. Der Standardwert ist 10.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


Stellt Hauptgitternetzlinien auf einer Diagrammachse dar.

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


Stellt den Typ der Hauptteilstriche für die angegebene Achse dar.

Siehe [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


Stellt die Hauptintervalle für die Achse dar.

**Remarks**

Die Hauptintervalle müssen größer als Null sein.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


Stellt die Skalierung der Hauptintervalle für die Kategorienachse dar.

Siehe [TimeUnit](../../com.aspose.cells/timeunit).

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


Stellt den Maximalwert auf der Werteachse dar.

**Remarks**

Der Typ von maxValue kann nur double oder DateTime sein.

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


Stellt den Minimalwert auf der Werteachse dar.

**Remarks**

Der Typ von minValue kann nur double oder DateTime sein.

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


Stellt Neben\-gitternetzlinien auf einer Diagrammachse dar.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


Stellt den Typ der Neben\-teilstriche für die angegebene Achse dar.

Siehe [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


Stellt die Nebenintervalle für die Achse dar.

**Remarks**

Die Nebenintervalle müssen größer als Null sein.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


Stellt die Skalierung der Hauptintervalle für die Kategorienachse dar.

Siehe [TimeUnit](../../com.aspose.cells/timeunit).

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


Stellt die Position der Teilstrich\-Beschriftungen auf der angegebenen Achse dar.

Siehe [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


Gibt die Anzahl der Kategorien oder Reihen zwischen den Tick‑Marken‑Beschriftungen an. Gilt nur für Kategorien‑ und Reihenachsen.

**Remarks**

Die Zahl muss zwischen 1 und 31999 liegen.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


Gibt ein [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--)\-Objekt zurück, das die Teilstrich\-Beschriftungen für die angegebene Achse darstellt.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


Gibt die Anzahl der Kategorien oder Reihen zwischen den Teilstrichen zurück oder legt sie fest. Gilt nur für Kategorien- und Reihenachsen.

**Remarks**

Die Zahl muss zwischen 1 und 31999 liegen.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Liest den Titel dieser Achse im Diagramm.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


Gibt an, ob die Beschriftungen mehrstufig angezeigt werden sollen.

**Remarks**

Nur gültig für die Kategorienachse.

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


Gibt an, ob der Abstand der Teilstrich\-Beschriftungen automatisch ist

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


Gibt an, ob die Haupteinheit der Achse automatisch zugewiesen wird.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


Gibt an, ob der Maximalwert automatisch zugewiesen wird.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


Gibt an, ob der Minimalwert automatisch zugewiesen wird.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


Gibt an, ob die Nebeneinheit der Achse automatisch zugewiesen wird.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


Gibt an, ob die Basiseinheit automatisch ist.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


Gibt an, ob das Anzeigeeinheiten‑Label auf der angegebenen Achse angezeigt wird.

**Remarks**

Der Standardwert ist True. Funktioniert nur, wenn [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) nicht [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE) ist.

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


Gibt an, ob der Skalierungstyp der Werteachse logarithmisch ist oder nicht.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


Gibt an, ob Microsoft Excel Datenpunkte von zuletzt nach zuerst darstellt.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Gibt an, ob die Achse sichtbar ist.

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


Gibt an, ob der Abstand der Teilstrich\-Beschriftungen automatisch ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


Gibt an, ob die Haupteinheit der Achse automatisch zugewiesen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


Gibt an, ob der Maximalwert automatisch zugewiesen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


Gibt an, ob der Minimalwert automatisch zugewiesen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


Gibt an, ob die Nebeneinheit der Achse automatisch zugewiesen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


Gibt an, ob die Werte‑Achse die Kategorien‑Achse zwischen den Kategorien schneidet.

**Remarks**

Diese Eigenschaft gilt nur für Kategorienachsen und nicht für 3‑D‑Diagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


Gibt an, ob die Basiseinheit automatisch ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


Stellt die Basiseinheitsskala für die Kategorien‑Achse dar.

Siehe [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Wirkt nur, wenn die Eigenschaft CategoryType auf TimeScale gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


Stellt den Typ der Kategorien‑Achse dar.

Siehe [CategoryType](../../com.aspose.cells/categorytype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


Stellt den Punkt auf der Werte‑Achse dar, an dem die Kategorien‑Achse sie schneidet.

**Remarks**

Die Zahl sollte eine ganze Zahl sein, wenn sie für die Kategorienachse gilt. Und der Wert muss zwischen 1 und 31999 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


Stellt die [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) auf der angegebenen Achse dar, an der die andere Achse kreuzt.

Siehe [CrossType](../../com.aspose.cells/crosstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Axis.CustomUnit. Diese Eigenschaft wird 12 Monate nach Januar 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Axis.CustomDisplayUnit. Diese Eigenschaft wird 12 Monate nach Februar 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


Stellt die Einheitbeschriftung für die angegebene Achse dar.

Siehe [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


Gibt an, ob das Anzeigeeinheiten‑Label auf der angegebenen Achse angezeigt wird.

**Remarks**

Der Standardwert ist True. Funktioniert nur, wenn [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) nicht [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE) ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


Gibt an, ob die Beschriftungen mehrstufig angezeigt werden sollen.

**Remarks**

Nur gültig für die Kategorienachse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


Gibt die logarithmische Basis an. Der Standardwert ist 10.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


Gibt an, ob der Skalierungstyp der Werteachse logarithmisch ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


Stellt den Typ der Hauptteilstriche für die angegebene Achse dar.

Siehe [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


Stellt die Hauptintervalle für die Achse dar.

**Remarks**

Die Hauptintervalle müssen größer als Null sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


Stellt die Skalierung der Hauptintervalle für die Kategorienachse dar.

Siehe [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


Stellt den Maximalwert auf der Werteachse dar.

**Remarks**

Der Typ von maxValue kann nur double oder DateTime sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


Stellt den Minimalwert auf der Werteachse dar.

**Remarks**

Der Typ von minValue kann nur double oder DateTime sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


Stellt den Typ der Neben\-teilstriche für die angegebene Achse dar.

Siehe [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


Stellt die Nebenintervalle für die Achse dar.

**Remarks**

Die Nebenintervalle müssen größer als Null sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


Stellt die Skalierung der Hauptintervalle für die Kategorienachse dar.

Siehe [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


Gibt an, ob Microsoft Excel Datenpunkte von zuletzt nach zuerst darstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


Stellt die Position der Teilstrich\-Beschriftungen auf der angegebenen Achse dar.

Siehe [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


Gibt die Anzahl der Kategorien oder Reihen zwischen den Tick‑Marken‑Beschriftungen an. Gilt nur für Kategorien‑ und Reihenachsen.

**Remarks**

Die Zahl muss zwischen 1 und 31999 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


Gibt die Anzahl der Kategorien oder Reihen zwischen den Teilstrichen zurück oder legt sie fest. Gilt nur für Kategorien- und Reihenachsen.

**Remarks**

Die Zahl muss zwischen 1 und 31999 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Gibt an, ob die Achse sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

