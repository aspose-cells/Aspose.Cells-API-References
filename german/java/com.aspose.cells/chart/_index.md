---
title: "Diagramm"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das ein einzelnes Excel‑Diagramm darstellt."
type: docs
url: /de/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

Kapselt das Objekt, das ein einzelnes Excel‑Diagramm darstellt.

**Example**

Der folgende Code zeigt, wie man ein Diagramm mit .NET-Code erstellt.

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
 
         	Chart chart = sheet.getCharts().get(chartIndex);
         chart.setChartDataRange("A1:B4", true);
         	chart.setShowLegend(true);
         	chart.getTitle().setText("Income Analysis");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [calculate()](#calculate--) | Berechnet die benutzerdefinierten Positionen des Plotbereichs und der Achsen, wenn deren Positionen automatisch zugewiesen werden. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | Berechnet die benutzerdefinierte Position des Plotbereichs und der Achsen, wenn deren Position automatisch zugewiesen wird, mit den Chart-Berechnungsoptionen. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | Diagrammtyp mit einer vordefinierten Vorlage ändern. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | Ermittelt die tatsächliche Größe des Diagramms in Pixel. |
| [getActualSize()](#getActualSize--) | Ermittelt die tatsächliche Größe des Diagramms in Pixel. |
| [getAutoScaling()](#getAutoScaling--) | Wahr, wenn Microsoft Excel ein 3‑D‑Diagramm skaliert, sodass es in der Größe dem entsprechenden 2‑D‑Diagramm näher kommt. |
| [getBackWall()](#getBackWall--) | Gibt ein [getWalls()](../../com.aspose.cells/chart\#getWalls--) Objekt zurück, das die Rückwand eines 3‑D‑Diagramms darstellt. |
| [getCategoryAxis()](#getCategoryAxis--) | Ermittelt die X‑Achse des Diagramms. |
| [getChartArea()](#getChartArea--) | Ermittelt den Diagrammbereich im Arbeitsblatt. |
| [getChartDataRange()](#getChartDataRange--) | Ermittelt den Datenquellenbereich des Diagramms. |
| [getChartDataTable()](#getChartDataTable--) | Stellt die Diagrammdatentabelle dar. |
| [getChartObject()](#getChartObject--) | Stellt das chartShape dar; |
| [getChartShape()](#getChartShape--) | Stellt das chartShape dar; |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | Stellt die Tiefe eines 3-D-Diagramms als Prozentsatz der Diagrammbreite dar (zwischen 20 und 2000 Prozent). |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | Gibt an, ob \#N/A als leerer Wert angezeigt werden soll. |
| [getElevation()](#getElevation--) | Stellt die Elevation der 3-D-Diagrammansicht in Grad dar. |
| [getFilteredNSeries()](#getFilteredNSeries--) | Ruft eine [SeriesCollection](../../com.aspose.cells/seriescollection)-Sammlung ab, die die Datenreihen darstellt, die im Diagramm gefiltert werden. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Ruft den Winkel des ersten Kuchen- oder Donut-Diagrammsegments in Grad ab (im Uhrzeigersinn von vertikal aus). |
| [getFloor()](#getFloor--) | Gibt ein [getFloor()](../../com.aspose.cells/chart\\#getFloor--)‑Objekt zurück, das die Wände eines 3-D-Diagramms darstellt. |
| [getGapDepth()](#getGapDepth--) | Ruft den Abstand zwischen den Datenreihen in einem 3-D-Diagramm als Prozentsatz der Markierungsbreite ab. |
| [getGapWidth()](#getGapWidth--) | Gibt den Abstand zwischen Balken‑ oder Säulen‑Clustern zurück oder setzt ihn, als Prozentsatz der Balken‑ oder Säulenbreite. |
| [getHeightPercent()](#getHeightPercent--) | Gibt die Höhe eines 3-D-Diagramms zurück oder setzt sie, als Prozentsatz der Diagrammbreite (zwischen 5 und 500 Prozent). |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | Gibt an, ob die Pivot‑Diagramm‑Feldschaltflächen nur ausgeblendet werden sollen, wenn das Diagramm ein PivotChart ist. |
| [getIs3D()](#getIs3D--) | Gibt an, ob das Diagramm ein 3-D-Diagramm ist. |
| [getLegend()](#getLegend--) | Ruft die Diagrammlegende ab. |
| [getLine()](#getLine--) | Ruft die Linie ab. |
| [getNSeries()](#getNSeries--) | Ruft eine [SeriesCollection](../../com.aspose.cells/seriescollection)-Sammlung ab, die die Datenreihen im Diagramm darstellt. |
| [getName()](#getName--) | Ruft den Namen des Diagramms ab. |
| [getPageSetup()](#getPageSetup--) | Stellt die Seitenlayoutbeschreibung in diesem Diagramm dar. |
| [getPerspective()](#getPerspective--) | Gibt die Perspektive für die three\\\\u9225\\\\u6178dimensional‑Diagrammansicht zurück oder setzt sie. |
| [getPivotOptions()](#getPivotOptions--) | Gibt die Pivot‑Steuerelemente an, die im Diagramm angezeigt werden. |
| [getPivotSource()](#getPivotSource--) | Die Quelle sind die Daten der Pivot‑Tabelle. |
| [getPlacement()](#getPlacement--) | Stellt die Art dar, wie das Diagramm an den darunter liegenden Zellen befestigt ist. |
| [getPlotArea()](#getPlotArea--) | Ruft den Plot‑Bereich des Diagramms ab, der Achsen‑Tick‑Beschriftungen enthält. |
| [getPlotBy()](#getPlotBy--) | Ruft ab, ob nach Zeile oder Spalte geplottet wird. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Ruft ab, wie leere Zellen geplottet werden. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Gibt an, ob nur sichtbare Zellen geplottet werden. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | Gibt an, ob nur sichtbare Zellen des Diagramms angezeigt werden. |
| [getPrintSize()](#getPrintSize--) | Ermittelt die gedruckte Diagrammgröße. |
| [getRightAngleAxes()](#getRightAngleAxes--) | True, wenn die Diagrammachsen rechtwinklig sind. |
| [getRotationAngle()](#getRotationAngle--) | Stellt die Drehung der 3‑D‑Diagrammansicht dar (die Drehung des Diagrammbereichs um die Z‑Achse, in Grad). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | Ermittelt die zweite X‑Achse des Diagramms. |
| [getSecondValueAxis()](#getSecondValueAxis--) | Ermittelt die zweite Y‑Achse des Diagramms. |
| [getSeriesAxis()](#getSeriesAxis--) | Ermittelt die Reihen‑Achse des Diagramms. |
| [getShapes()](#getShapes--) | Gibt alle Zeichenformen in diesem Diagramm zurück. |
| [getShowDataTable()](#getShowDataTable--) | Ermittelt einen Wert, der angibt, ob das Diagramm eine Datentabelle anzeigt. |
| [getShowLegend()](#getShowLegend--) | Ermittelt einen Wert, der angibt, ob die Diagrammlegende angezeigt wird. |
| [getSideWall()](#getSideWall--) | Gibt ein [getWalls()](../../com.aspose.cells/chart\#getWalls--) Objekt zurück, das die Seitenwand eines 3‑D‑Diagramms darstellt. |
| [getSizeWithWindow()](#getSizeWithWindow--) | True, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblattfensters anpasst. |
| [getStyle()](#getStyle--) | Ermittelt den integrierten Stil. |
| [getSubTitle()](#getSubTitle--) | Ermittelt den Untertitel des Diagramms. |
| [getTitle()](#getTitle--) | Ermittelt den Titel des Diagramms. |
| [getType()](#getType--) | Ermittelt den Typ eines Diagramms. |
| [getValueAxis()](#getValueAxis--) | Ermittelt die Y‑Achse des Diagramms. |
| [getWalls()](#getWalls--) | Gibt ein [getWalls()](../../com.aspose.cells/chart\#getWalls--) Objekt zurück, das die Wände eines 3‑D‑Diagramms darstellt. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | True, wenn Rasterlinien zweidimensional in einem 3‑D‑Diagramm gezeichnet werden. |
| [getWorksheet()](#getWorksheet--) | Ermittelt das Arbeitsblatt, das dieses Diagramm enthält. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | Gibt zurück, welche Achsen im Diagramm vorhanden sind. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | Gibt zurück, ob die vom Diagramm referenzierte Zelle. |
| [isChartDataChanged()](#isChartDataChanged--) | Erkennt, ob die Datenquelle eines Diagramms geändert wurde. |
| [isRectangularCornered()](#isRectangularCornered--) | Ermittelt einen Wert, der angibt, ob der Diagrammbereich rechteckige Ecken hat. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | Gibt zurück, ob die Zelle vom Diagramm referenziert wird. |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | Verschiebt das Diagramm an einen angegebenen Ort. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | Aktualisiert die Diagrammdaten aus der Pivot‑Tabelle. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | Wahr, wenn Microsoft Excel ein 3‑D‑Diagramm skaliert, sodass es in der Größe dem entsprechenden 2‑D‑Diagramm näher kommt. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | Gibt den Datenbereich für ein Diagramm an. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | Stellt die Tiefe eines 3-D-Diagramms als Prozentsatz der Diagrammbreite dar (zwischen 20 und 2000 Prozent). |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | Gibt an, ob \#N/A als leerer Wert angezeigt werden soll. |
| [setElevation(int value)](#setElevation-int-) | Stellt die Elevation der 3-D-Diagrammansicht in Grad dar. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | Legt den Winkel des ersten Kuchendiagramm‑ oder Donutdiagramm‑Scheibchens in Grad fest (im Uhrzeigersinn von vertikal aus). |
| [setGapDepth(int value)](#setGapDepth-int-) | Legt den Abstand zwischen den Datenreihen in einem 3‑D‑Diagramm als Prozentsatz der Markierungsbreite fest. |
| [setGapWidth(int value)](#setGapWidth-int-) | Gibt den Abstand zwischen Balken‑ oder Säulen‑Clustern zurück oder setzt ihn, als Prozentsatz der Balken‑ oder Säulenbreite. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | Gibt die Höhe eines 3-D-Diagramms zurück oder setzt sie, als Prozentsatz der Diagrammbreite (zwischen 5 und 500 Prozent). |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | Gibt an, ob die Pivot‑Diagramm‑Feldschaltflächen nur ausgeblendet werden sollen, wenn das Diagramm ein PivotChart ist. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen des Diagramms fest. |
| [setPerspective(short value)](#setPerspective-short-) | Gibt die Perspektive für die three\\\\u9225\\\\u6178dimensional‑Diagrammansicht zurück oder setzt sie. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | Die Quelle sind die Daten der Pivot‑Tabelle. |
| [setPlacement(int value)](#setPlacement-int-) | Stellt die Art dar, wie das Diagramm an den darunter liegenden Zellen befestigt ist. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Legt fest, wie leere Zellen dargestellt werden. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Gibt an, ob nur sichtbare Zellen geplottet werden. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | Gibt an, ob nur sichtbare Zellen des Diagramms angezeigt werden. |
| [setPrintSize(int value)](#setPrintSize-int-) | Legt die Druckgröße des Diagramms fest. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | Setzt einen Wert, der angibt, ob der Diagrammbereich rechteckig mit Ecken ist. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | True, wenn die Diagrammachsen rechtwinklig sind. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Stellt die Drehung der 3‑D‑Diagrammansicht dar (die Drehung des Diagrammbereichs um die Z‑Achse, in Grad). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | Setzt einen Wert, der angibt, ob das Diagramm eine Datentabelle anzeigt. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | Setzt einen Wert, der angibt, ob die Diagrammlegende angezeigt wird. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | True, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblattfensters anpasst. |
| [setStyle(int value)](#setStyle-int-) | Legt den integrierten Stil fest. |
| [setType(int value)](#setType-int-) | Legt den Typ eines Diagramms fest. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | True, wenn Rasterlinien zweidimensional in einem 3‑D‑Diagramm gezeichnet werden. |
| [switchRowColumn()](#switchRowColumn--) | Wechselt Zeile/Spalte. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Erstellt das Diagrammbild und speichert es in einen Stream im angegebenen Format. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | Erstellt das Diagrammbild und speichert es in einer Datei. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Format. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Erstellt das Diagrammbild und speichert es in einer Datei. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Bildtyp. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | Erstellt das Diagrammbild und speichert es in einer Datei im JPEG‑Format. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | Erstellt das Diagramm‑PDF und speichert es in einen Stream. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | Erstellt das Diagramm‑PDF und speichert es in einen Stream. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | Speichert das Diagramm in einer PDF‑Datei. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | Speichert das Diagramm in einer PDF‑Datei. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


Berechnet die benutzerdefinierten Positionen des Plotbereichs und der Achsen, wenn deren Positionen automatisch zugewiesen werden.

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


Berechnet die benutzerdefinierte Position des Plotbereichs und der Achsen, wenn deren Position automatisch zugewiesen wird, mit den Chart-Berechnungsoptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


Diagrammtyp mit einer vordefinierten Vorlage ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Daten | byte[] | Die Daten der Diagrammvorlagendatei (.crtx). |

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
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


Ermittelt die tatsächliche Größe des Diagramms in Pixel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Chart.getActualSize(). Diese Eigenschaft wird 12 Monate nach Juli 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
int[] – Tatsächliche Größe in einem Array (Breite und Höhe). [0] ist die Breite; [1] ist die Höhe.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


Ermittelt die tatsächliche Größe des Diagramms in Pixel.

**Returns:**
int[] – Tatsächliche Größe in einem Array (Breite und Höhe). [0] ist die Breite; [1] ist die Höhe.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


True, wenn Microsoft Excel ein 3‑D‑Diagramm so skaliert, dass es der Größe des entsprechenden 2‑D‑Diagramms näher kommt. Die RightAngleAxes‑Property muss True sein.

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


Gibt ein [getWalls()](../../com.aspose.cells/chart\#getWalls--) Objekt zurück, das die Rückwand eines 3‑D‑Diagramms darstellt.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


Ermittelt die X‑Achse des Diagramms.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


Ermittelt den Diagrammbereich im Arbeitsblatt.

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


Ermittelt den Datenquellenbereich des Diagramms.

**Remarks**

Unterstützt nur Bereiche. Wenn Series.Values, Name und XValues in einem zusammenhängenden Bereich liegen, wird ein Bereich, der sie enthält, zurückgegeben.

**Returns:**
java.lang.String – Die Datenquelle.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


Stellt die Diagrammdatentabelle dar.

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


Stellt das chartShape dar;

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


Stellt das chartShape dar;

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Aspose.Cells.Charts.Chart.ChartObject‑Property. Diese Property wird 12 Monate später, seit JANUAR 2012, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sind.

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDepthPercent() {#getDepthPercent--}
```
public int getDepthPercent()
```


Stellt die Tiefe eines 3-D-Diagramms als Prozentsatz der Diagrammbreite dar (zwischen 20 und 2000 Prozent).

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


Gibt an, ob \#N/A als leerer Wert angezeigt werden soll.

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


Stellt die Elevation der 3-D-Diagrammansicht in Grad dar.

**Remarks**

Die Diagrammhöhe ist die Höhe, aus der Sie das Diagramm betrachten, in Grad. Der Standardwert ist 15 für die meisten Diagrammtypen. Der Wert dieser Property muss zwischen -90 und 90 liegen, außer bei 3‑D‑Balkendiagrammen, wo er zwischen 0 und 44 liegen muss.

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


Ruft eine [SeriesCollection](../../com.aspose.cells/seriescollection)-Sammlung ab, die die Datenreihen darstellt, die im Diagramm gefiltert werden.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


Gibt den Winkel des ersten Kuchen‑ oder Donut‑Diagrammsegments in Grad zurück (im Uhrzeigersinn von der Vertikalen). Gilt nur für Kuchen-, 3‑D‑Kuchen- und Donut‑Diagramme, 0 bis 360.

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


Gibt ein [getFloor()](../../com.aspose.cells/chart\\#getFloor--)‑Objekt zurück, das die Wände eines 3-D-Diagramms darstellt.

**Remarks**

Diese Property gilt nicht für 3‑D‑Kuchendiagramme.

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


Gibt den Abstand zwischen den Datenreihen in einem 3‑D‑Diagramm als Prozentsatz der Markierungsbreite zurück. Der Wert dieser Property muss zwischen 0 und 500 liegen.

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


Gibt den Abstand zwischen Balken‑ oder Säulen‑Clustern zurück oder legt ihn fest, als Prozentsatz der Balken‑ oder Säulenbreite. Der Wert dieser Property muss zwischen 0 und 500 liegen.

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


Gibt die Höhe eines 3-D-Diagramms zurück oder setzt sie, als Prozentsatz der Diagrammbreite (zwischen 5 und 500 Prozent).

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


Gibt an, ob die Pivot‑Diagramm‑Feldschaltflächen nur ausgeblendet werden sollen, wenn das Diagramm ein PivotChart ist.

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


Gibt an, ob das Diagramm ein 3-D-Diagramm ist.

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


Ruft die Diagrammlegende ab.

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


Ruft die Linie ab.

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


Ruft eine [SeriesCollection](../../com.aspose.cells/seriescollection)-Sammlung ab, die die Datenreihen im Diagramm darstellt.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


Ruft den Namen des Diagramms ab.

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Stellt die Seitenlayoutbeschreibung in diesem Diagramm dar.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


Gibt die Perspektive für die dreidimensionale Diagrammansicht zurück oder legt sie fest. Muss zwischen 0 und 100 liegen. Diese Property wird ignoriert, wenn die RightAngleAxes‑Property True ist.

**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


Gibt die Pivot‑Steuerelemente an, die im Diagramm angezeigt werden.

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


Die Quelle sind die Daten der Pivot‑Tabelle. Wenn PivotSource nicht leer ist, ist das Diagramm ein PivotChart.

**Remarks**

Wenn die Pivot‑Tabelle "PivotTable1" im Arbeitsblatt "Sheet1" in der Datei "Book1.xls" liegt. Der pivotSource könnte "[Book1.xls]Sheet1!PivotTable1" sein, wenn das Diagramm und die Pivot‑Tabelle nicht im selben Arbeitsbuch sind. Wenn Sie diese Property setzen, geht die vorherige Datenquelleneinstellung verloren.

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Stellt die Art dar, wie das Diagramm an den darunter liegenden Zellen befestigt ist.

Siehe [PlacementType](../../com.aspose.cells/placementtype).

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


Ruft den Plot‑Bereich des Diagramms ab, der Achsen‑Tick‑Beschriftungen enthält.

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


Ruft ab, ob nach Zeile oder Spalte geplottet wird.

Siehe [PlotDataByType](../../com.aspose.cells/plotdatabytype).

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Ruft ab, wie leere Zellen geplottet werden.

Siehe [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Gibt an, ob nur sichtbare Zellen geplottet werden.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die PlotVisibleCellsOnly‑Property. Diese Methode wird 12 Monate später, seit Dezember 2022, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sind.

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


Gibt an, ob nur sichtbare Zellen des Diagramms angezeigt werden.

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


Ermittelt die gedruckte Diagrammgröße.

Siehe [PrintSizeType](../../com.aspose.cells/printsizetype).

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


True, wenn die Diagrammachsen rechtwinklig sind. Gilt nur für 3‑D‑Diagramme (außer Column3D und 3‑D‑Kuchendiagrammen).

**Remarks**

Wenn diese Property True ist, wird die Perspective‑Property ignoriert.

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Stellt die Drehung der 3‑D‑Diagrammansicht dar (die Drehung des Diagrammbereichs um die Z‑Achse, in Grad).

**Remarks**

Der Wert dieser Property muss zwischen 0 und 360 liegen, außer bei 3‑D‑Balkendiagrammen, wo er zwischen 0 und 44 liegen muss. Der Standardwert ist 20. Gilt nur für 3‑D‑Diagramme.

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


Ermittelt die zweite X‑Achse des Diagramms.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


Ermittelt die zweite Y‑Achse des Diagramms.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


Ermittelt die Reihen‑Achse des Diagramms.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Gibt alle Zeichenformen in diesem Diagramm zurück.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


Ermittelt einen Wert, der angibt, ob das Diagramm eine Datentabelle anzeigt.

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


Gibt einen Wert zurück, der angibt, ob die Diagrammlegende angezeigt wird. Standard ist true.

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


Gibt ein [getWalls()](../../com.aspose.cells/chart\#getWalls--) Objekt zurück, das die Seitenwand eines 3‑D‑Diagramms darstellt.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


True, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblattfensters anpasst.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Ermittelt den integrierten Stil.

**Remarks**

Sie sollte zwischen 1 und 48 liegen. Gibt -1 zurück, wenn sie nicht gesetzt ist.

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


Gibt den Untertitel des Diagramms zurück. Gilt nur für ODS‑Dateien.

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Ermittelt den Titel des Diagramms.

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


Ermittelt den Typ eines Diagramms.

Siehe [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


Ermittelt die Y‑Achse des Diagramms.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


Gibt ein [getWalls()](../../com.aspose.cells/chart\#getWalls--) Objekt zurück, das die Wände eines 3‑D‑Diagramms darstellt.

**Remarks**

Diese Property gilt nicht für 3‑D‑Kuchendiagramme.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


True, wenn Rasterlinien zweidimensional in einem 3‑D‑Diagramm gezeichnet werden.

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Ermittelt das Arbeitsblatt, das dieses Diagramm enthält.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


Gibt zurück, welche Achsen im Diagramm vorhanden sind.

**Remarks**

Normalerweise haben Pie, PieExploded, PiePie, PieBar, Pie3D, Pie3DExploded, Doughnut und DoughnutExploded keine Achse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| aixsType | int |  |
| isPrimary | boolean |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex) {#isCellReferedByChart-int-int-int-}
```
public boolean isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```


Gibt zurück, ob die vom Diagramm referenzierte Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Der Blattindex -1 bedeutet das Arbeitsblatt, das das aktuelle Diagramm enthält. |
| rowIndex | int | Der Zeilenindex |
| columnIndex | int | Der Spaltenindex |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


Erkennt, ob die Datenquelle eines Diagramms geändert wurde.

**Remarks**

Die Methode erkennt Änderungen in der Datenquelle des Diagramms, bevor das Diagramm in ein Bildformat gerendert wird. Beim ersten Aufruf von Chart.toImage werden die Diagrammdaten (z. B. XValuesParseData, ValuesParseData) aufgezeichnet. Bevor die Methode Chart.toImage erneut aufgerufen wird, rufen Sie die Methode IsChartDataChanged auf, um zu prüfen, ob das Diagramm erneut gerendert werden muss.

**Returns:**
boolean – Gibt true zurück, wenn das Diagramm geändert wurde, andernfalls false.
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


Gibt einen Wert zurück, der angibt, ob der Diagrammbereich rechteckig ist. Standard ist true.

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


Gibt zurück, ob die Zelle vom Diagramm referenziert wird.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode IsCellReferedByChart(int,int,int). Diese Methode wird 12 Monate später, seit April 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Der Zeilenindex |
| columnIndex | int | Der Spaltenindex |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Verschiebt das Diagramm an einen angegebenen Ort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| bottomRow | int | Index der unteren rechten Zeile |
| rightColumn | int | Index der unteren rechten Spalte |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshPivotData() {#refreshPivotData--}
```
public void refreshPivotData()
```


Aktualisiert die Diagrammdaten aus der Pivot‑Tabelle.

**Remarks**

Wir sammeln Daten aus der Pivot-Datenquelle für den Pivot-Tabellenbericht. Diese Methode wird nur verwendet, um alle Daten für ein Pivot-Diagramm zu sammeln.

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


True, wenn Microsoft Excel ein 3‑D‑Diagramm so skaliert, dass es der Größe des entsprechenden 2‑D‑Diagramms näher kommt. Die RightAngleAxes‑Property muss True sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


Gibt den Datenbereich für ein Diagramm an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | java.lang.String | Gibt die Werte an, aus denen die Datenreihe geplottet wird. |
| isVertical | boolean | Gibt an, ob die Serie aus einem Zellwertbereich zeilenweise oder spaltenweise geplottet werden soll. |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


Stellt die Tiefe eines 3-D-Diagramms als Prozentsatz der Diagrammbreite dar (zwischen 20 und 2000 Prozent).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


Gibt an, ob \#N/A als leerer Wert angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


Stellt die Elevation der 3-D-Diagrammansicht in Grad dar.

**Remarks**

Die Diagrammhöhe ist die Höhe, aus der Sie das Diagramm betrachten, in Grad. Der Standardwert ist 15 für die meisten Diagrammtypen. Der Wert dieser Property muss zwischen -90 und 90 liegen, außer bei 3‑D‑Balkendiagrammen, wo er zwischen 0 und 44 liegen muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


Legt den Winkel des ersten Stücks eines Kreis- oder Donut-Diagramms in Grad fest (im Uhrzeigersinn von vertikal aus). Gilt nur für Kreis-, 3‑D‑Kreis- und Donut‑Diagramme, 0 bis 360.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


Legt den Abstand zwischen den Datenreihen in einem 3‑D‑Diagramm als Prozentsatz der Markierungsbreite fest. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


Gibt den Abstand zwischen Balken‑ oder Säulen‑Clustern zurück oder legt ihn fest, als Prozentsatz der Balken‑ oder Säulenbreite. Der Wert dieser Property muss zwischen 0 und 500 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


Gibt die Höhe eines 3-D-Diagramms zurück oder setzt sie, als Prozentsatz der Diagrammbreite (zwischen 5 und 500 Prozent).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


Gibt an, ob die Pivot‑Diagramm‑Feldschaltflächen nur ausgeblendet werden sollen, wenn das Diagramm ein PivotChart ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Legt den Namen des Diagramms fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


Gibt die Perspektive für die dreidimensionale Diagrammansicht zurück oder legt sie fest. Muss zwischen 0 und 100 liegen. Diese Property wird ignoriert, wenn die RightAngleAxes‑Property True ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


Die Quelle sind die Daten der Pivot‑Tabelle. Wenn PivotSource nicht leer ist, ist das Diagramm ein PivotChart.

**Remarks**

Wenn die Pivot‑Tabelle "PivotTable1" im Arbeitsblatt "Sheet1" in der Datei "Book1.xls" liegt. Der pivotSource könnte "[Book1.xls]Sheet1!PivotTable1" sein, wenn das Diagramm und die Pivot‑Tabelle nicht im selben Arbeitsbuch sind. Wenn Sie diese Property setzen, geht die vorherige Datenquelleneinstellung verloren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Stellt die Art dar, wie das Diagramm an den darunter liegenden Zellen befestigt ist.

Siehe [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Legt fest, wie leere Zellen dargestellt werden.

Siehe [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Gibt an, ob nur sichtbare Zellen geplottet werden.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die PlotVisibleCellsOnly‑Property. Diese Methode wird 12 Monate später, seit Dezember 2022, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


Gibt an, ob nur sichtbare Zellen des Diagramms angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


Legt die Druckgröße des Diagramms fest.

Siehe [PrintSizeType](../../com.aspose.cells/printsizetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


Legt einen Wert fest, der angibt, ob der Diagrammbereich rechteckig ist. Standard ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


True, wenn die Diagrammachsen rechtwinklig sind. Gilt nur für 3‑D‑Diagramme (außer Column3D und 3‑D‑Kuchendiagrammen).

**Remarks**

Wenn diese Property True ist, wird die Perspective‑Property ignoriert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Stellt die Drehung der 3‑D‑Diagrammansicht dar (die Drehung des Diagrammbereichs um die Z‑Achse, in Grad).

**Remarks**

Der Wert dieser Property muss zwischen 0 und 360 liegen, außer bei 3‑D‑Balkendiagrammen, wo er zwischen 0 und 44 liegen muss. Der Standardwert ist 20. Gilt nur für 3‑D‑Diagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


Setzt einen Wert, der angibt, ob das Diagramm eine Datentabelle anzeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


Legt einen Wert fest, der angibt, ob die Diagrammlegende angezeigt wird. Standard ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


True, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblattfensters anpasst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Legt den integrierten Stil fest.

**Remarks**

Sie sollte zwischen 1 und 48 liegen. Gibt -1 zurück, wenn sie nicht gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Legt den Typ eines Diagramms fest.

Siehe [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


True, wenn Rasterlinien zweidimensional in einem 3‑D‑Diagramm gezeichnet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


Wechselt Zeile/Spalte.

**Returns:**
boolean – False bedeutet, dass das Vertauschen von Zeile/Spalte fehlschlägt.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Erstellt das Diagrammbild und speichert es in einen Stream im angegebenen Format.

**Remarks**

Das Format des Bildes wird über `options.ImageFormat` angegeben. Die folgenden Formate werden unterstützt: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.

Wenn Breite oder Höhe null ist oder das Diagramm laut Supported Charts List nicht unterstützt wird, führt diese Methode nichts aus. Bitte beachten Sie die [Supported Charts List][] für weitere Details.


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Ausgabestream. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Zusätzliche Optionen zur Bildgenerierung |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


Erstellt das Diagrammbild und speichert es in einer Datei. Die Dateierweiterung bestimmt das Format des Bildes.

**Remarks**

Das Format des Bildes wird über die Dateierweiterung angegeben. Zum Beispiel, wenn Sie "myfile.png" angeben, wird das Bild im PNG-Format gespeichert. Die folgenden Dateierweiterungen werden erkannt: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Wenn Breite oder Höhe null ist oder das Diagramm laut Supported Charts List nicht unterstützt wird, führt diese Methode nichts aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | java.lang.String | Der Bilddateiname mit vollständigem Pfad. |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Format.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Chart.ToImage(string, ImageType). Diese Eigenschaft wird 12 Monate später, seit Juli 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | java.lang.String | Der Bilddateiname mit vollständigem Pfad. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Das Format, in dem das Bild gespeichert werden soll. |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Erstellt das Diagrammbild und speichert es in einer Datei. Die Dateierweiterung bestimmt das Format des Bildes.

**Remarks**

Das Format des Bildes wird über die Dateierweiterung angegeben. Zum Beispiel, wenn Sie "myfile.png" angeben, wird das Bild im PNG-Format gespeichert. Die folgenden Dateierweiterungen werden erkannt: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Wenn Breite oder Höhe null ist oder das Diagramm laut Supported Charts List nicht unterstützt wird, führt diese Methode nichts aus. Bitte beachten Sie die [Supported Charts List][] für weitere Details.

**Example**

Speichert als Tiff mit 300 dpi und CCITT4-Kompression.

```
         ImageOrPrintOptions options = new ImageOrPrintOptions();
         options.setHorizontalResolution(300);
         options.setVerticalResolution(300);
         options.setTiffCompression(TiffCompression.COMPRESSION_CCITT_4);
 
         Workbook book = new Workbook("test.xls");
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.Tiff", options);
```


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | java.lang.String | Der Bilddateiname mit vollständigem Pfad. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Zusätzliche Optionen zur Bildgenerierung |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Bildtyp.

**Remarks**

Der Bildtyp wird über `imageType` angegeben. Die folgenden Typen werden unterstützt: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Wenn Breite oder Höhe null ist oder das Diagramm laut Supported Charts List nicht unterstützt wird, führt diese Methode nichts aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | java.lang.String | Der Bilddateiname mit vollständigem Pfad. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). Der Bildtyp, in dem das Bild gespeichert werden soll. |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


Erstellt das Diagrammbild und speichert es in einer Datei im JPEG‑Format.

**Remarks**

Wenn die Breite oder Höhe null ist oder das Diagramm laut der unterstützten Diagrammliste nicht unterstützt wird, führt diese Methode nichts aus. HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode ToImage(string,ImageOrPrintOptions) mit der angegebenen Qualität. Diese Methode wird 12 Monate später, seit März 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | java.lang.String | Der Bilddateiname mit vollständigem Pfad. |
| jpegQuality | long | Jpeg-Qualität. |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


Erstellt das Diagramm‑PDF und speichert es in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Ausgabestream. |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Erstellt das Diagramm‑PDF und speichert es in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Ausgabestream. |
| desiredPageWidth | float | Die gewünschte Seitenbreite in Zoll. |
| desiredPageHeight | float | Die gewünschte Seitenhöhe in Zoll. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Der horizontale Ausrichtungstyp des Diagramms auf der Ausgabeseite. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Der vertikale Ausrichtungstyp des Diagramms auf der Ausgabeseite. |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


Speichert das Diagramm in einer PDF‑Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | der PDF-Dateiname mit vollständigem Pfad |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Speichert das Diagramm in einer PDF‑Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | der PDF-Dateiname mit vollständigem Pfad |
| desiredPageWidth | float | Die gewünschte Seitenbreite in Zoll. |
| desiredPageHeight | float | Die gewünschte Seitenhöhe in Zoll. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Der horizontale Ausrichtungstyp des Diagramms auf der Ausgabeseite. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Der vertikale Ausrichtungstyp des Diagramms auf der Ausgabeseite. |

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

