---
title: "SparklineGroup"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "è organizzato in un gruppo di sparkline."
type: docs
url: /it/java/com.aspose.cells/sparklinegroup/
---

**Inheritance:**
java.lang.Object
```
public class SparklineGroup
```

[Sparkline](../../com.aspose.cells/sparkline) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         // Create CellsColor
         CellsColor clr = book.createCellsColor();
         clr.setColor(Color.getOrange());
         group.setSeriesColor(clr);
 
         // set the high points are colored green and the low points are colored red
         group.setShowHighPoint(true);
         group.setShowLowPoint(true);
         group.getHighPointColor().setColor(Color.getGreen());
         group.getLowPointColor().setColor(Color.getRed());
         // set line weight 
         group.setLineWeight(1.0);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayHidden()](#getDisplayHidden--) | Indica se mostrare i dati in righe e colonne nascoste. |
| [getFirstPointColor()](#getFirstPointColor--) | Ottiene il colore del primo punto dati nel gruppo di sparkline. |
| [getHighPointColor()](#getHighPointColor--) | Ottiene il colore dei punti più alti dei dati nel gruppo di sparkline. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--) | Ottiene il colore dell'asse orizzontale nel gruppo di sparkline. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--) | Rappresenta l'intervallo che contiene i valori di data per i dati di sparkline. |
| [getLastPointColor()](#getLastPointColor--) | Ottiene il colore dell'ultimo punto dati nel gruppo di sparkline. |
| [getLineWeight()](#getLineWeight--) | Ottiene lo spessore della linea in ogni sparkline lineare nel gruppo di sparkline, nell'unità di punti. |
| [getLowPointColor()](#getLowPointColor--) | Ottiene il colore dei punti più bassi dei dati nel gruppo di sparkline. |
| [getMarkersColor()](#getMarkersColor--) | Ottiene il colore dei punti in ogni sparkline lineare nel gruppo di sparkline. |
| [getNegativePointsColor()](#getNegativePointsColor--) | Ottiene il colore dei valori negativi nel gruppo di sparkline. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Indica come tracciare le celle vuote. |
| [getPlotRightToLeft()](#getPlotRightToLeft--) | Indica se i dati del grafico sono da destra a sinistra. |
| [getPresetStyle()](#getPresetStyle--) | Ottiene il tipo di stile predefinito del gruppo di sparkline. |
| [getSeriesColor()](#getSeriesColor--) | Ottiene il colore delle sparkline nel gruppo di sparkline. |
| [getShowFirstPoint()](#getShowFirstPoint--) | Indica se evidenziare il primo punto dati nel gruppo di sparkline. |
| [getShowHighPoint()](#getShowHighPoint--) | Indica se evidenziare i punti più alti dei dati nel gruppo di sparkline. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--) | Indica se mostrare l'asse orizzontale dello sparkline. |
| [getShowLastPoint()](#getShowLastPoint--) | Indica se evidenziare l'ultimo punto dei dati nel gruppo di sparkline. |
| [getShowLowPoint()](#getShowLowPoint--) | Indica se evidenziare i punti più bassi dei dati nel gruppo di sparkline. |
| [getShowMarkers()](#getShowMarkers--) | Indica se evidenziare ogni punto in ciascuna sparkline a linee nel gruppo di sparkline. |
| [getShowNegativePoints()](#getShowNegativePoints--) | Indica se evidenziare i valori negativi nel gruppo di sparkline con un colore o marcatore diverso. |
| [getSparklineCollection()](#getSparklineCollection--) | Ottiene la collezione di oggetti [Sparkline](../../com.aspose.cells/sparkline). |
| [getSparklines()](#getSparklines--) | Ottiene la collezione di oggetti [Sparkline](../../com.aspose.cells/sparkline). |
| [getType()](#getType--) | Indica il tipo di sparkline del gruppo di sparkline. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--) | Ottiene il valore massimo personalizzato per l'asse verticale. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--) | Rappresenta il tipo di valore massimo dell'asse verticale. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--) | Ottiene il valore minimo personalizzato per l'asse verticale. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--) | Rappresenta il tipo di valore minimo dell'asse verticale. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [resetRanges(String dataRange, boolean isVertical, CellArea locationRange)](#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-) | Reimposta l'intervallo dei dati e l'intervallo di posizione del gruppo di sparkline. |
| [setDisplayHidden(boolean value)](#setDisplayHidden-boolean-) | Indica se mostrare i dati in righe e colonne nascoste. |
| [setFirstPointColor(CellsColor value)](#setFirstPointColor-com.aspose.cells.CellsColor-) | Imposta il colore del primo punto dei dati nel gruppo di sparkline. |
| [setHighPointColor(CellsColor value)](#setHighPointColor-com.aspose.cells.CellsColor-) | Imposta il colore dei punti più alti dei dati nel gruppo di sparkline. |
| [setHorizontalAxisColor(CellsColor value)](#setHorizontalAxisColor-com.aspose.cells.CellsColor-) | Imposta il colore dell'asse orizzontale nel gruppo di sparkline. |
| [setHorizontalAxisDateRange(String value)](#setHorizontalAxisDateRange-java.lang.String-) | Rappresenta l'intervallo che contiene i valori di data per i dati di sparkline. |
| [setLastPointColor(CellsColor value)](#setLastPointColor-com.aspose.cells.CellsColor-) | Imposta il colore dell'ultimo punto dei dati nel gruppo di sparkline. |
| [setLineWeight(double value)](#setLineWeight-double-) | Imposta lo spessore della linea in ogni sparkline a linee nel gruppo di sparkline, nell'unità di punti. |
| [setLowPointColor(CellsColor value)](#setLowPointColor-com.aspose.cells.CellsColor-) | Imposta il colore dei punti più bassi dei dati nel gruppo di sparkline. |
| [setMarkersColor(CellsColor value)](#setMarkersColor-com.aspose.cells.CellsColor-) | Imposta il colore dei punti in ogni sparkline a linee nel gruppo di sparkline. |
| [setNegativePointsColor(CellsColor value)](#setNegativePointsColor-com.aspose.cells.CellsColor-) | Imposta il colore dei valori negativi nel gruppo di sparkline. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Indica come tracciare le celle vuote. |
| [setPlotRightToLeft(boolean value)](#setPlotRightToLeft-boolean-) | Indica se i dati del grafico sono da destra a sinistra. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Imposta il tipo di stile predefinito del gruppo di sparkline. |
| [setSeriesColor(CellsColor value)](#setSeriesColor-com.aspose.cells.CellsColor-) | Imposta il colore delle sparkline nel gruppo di sparkline. |
| [setShowFirstPoint(boolean value)](#setShowFirstPoint-boolean-) | Indica se evidenziare il primo punto dati nel gruppo di sparkline. |
| [setShowHighPoint(boolean value)](#setShowHighPoint-boolean-) | Indica se evidenziare i punti più alti dei dati nel gruppo di sparkline. |
| [setShowHorizontalAxis(boolean value)](#setShowHorizontalAxis-boolean-) | Indica se mostrare l'asse orizzontale dello sparkline. |
| [setShowLastPoint(boolean value)](#setShowLastPoint-boolean-) | Indica se evidenziare l'ultimo punto dei dati nel gruppo di sparkline. |
| [setShowLowPoint(boolean value)](#setShowLowPoint-boolean-) | Indica se evidenziare i punti più bassi dei dati nel gruppo di sparkline. |
| [setShowMarkers(boolean value)](#setShowMarkers-boolean-) | Indica se evidenziare ogni punto in ciascuna sparkline a linee nel gruppo di sparkline. |
| [setShowNegativePoints(boolean value)](#setShowNegativePoints-boolean-) | Indica se evidenziare i valori negativi nel gruppo di sparkline con un colore o marcatore diverso. |
| [setType(int value)](#setType-int-) | Indica il tipo di sparkline del gruppo di sparkline. |
| [setVerticalAxisMaxValue(double value)](#setVerticalAxisMaxValue-double-) | Imposta il valore massimo personalizzato per l'asse verticale. |
| [setVerticalAxisMaxValue(int type, double value)](#setVerticalAxisMaxValue-int-double-) | Imposta il valore massimo personalizzato per l'asse verticale dello sparkline con il tipo di valore dell'asse specificato. |
| [setVerticalAxisMaxValueType(int value)](#setVerticalAxisMaxValueType-int-) | Rappresenta il tipo di valore massimo dell'asse verticale. |
| [setVerticalAxisMinValue(double value)](#setVerticalAxisMinValue-double-) | Imposta il valore minimo personalizzato per l'asse verticale. |
| [setVerticalAxisMinValue(int type, double value)](#setVerticalAxisMinValue-int-double-) | Imposta il valore minimo personalizzato per l'asse verticale dello sparkline con il tipo di valore dell'asse specificato. |
| [setVerticalAxisMinValueType(int value)](#setVerticalAxisMinValueType-int-) | Rappresenta il tipo di valore minimo dell'asse verticale. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDisplayHidden() {#getDisplayHidden--}
```
public boolean getDisplayHidden()
```


Indica se mostrare i dati in righe e colonne nascoste.

**Returns:**
boolean
### getFirstPointColor() {#getFirstPointColor--}
```
public CellsColor getFirstPointColor()
```


Ottiene il colore del primo punto dati nel gruppo di sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHighPointColor() {#getHighPointColor--}
```
public CellsColor getHighPointColor()
```


Ottiene il colore dei punti più alti dei dati nel gruppo di sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisColor() {#getHorizontalAxisColor--}
```
public CellsColor getHorizontalAxisColor()
```


Ottiene il colore dell'asse orizzontale nel gruppo di sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}
```
public String getHorizontalAxisDateRange()
```


Rappresenta l'intervallo che contiene i valori di data per i dati di sparkline.

**Returns:**
java.lang.String
### getLastPointColor() {#getLastPointColor--}
```
public CellsColor getLastPointColor()
```


Ottiene il colore dell'ultimo punto dati nel gruppo di sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getLineWeight() {#getLineWeight--}
```
public double getLineWeight()
```


Ottiene lo spessore della linea in ogni sparkline lineare nel gruppo di sparkline, nell'unità di punti.

**Returns:**
double
### getLowPointColor() {#getLowPointColor--}
```
public CellsColor getLowPointColor()
```


Ottiene il colore dei punti più bassi dei dati nel gruppo di sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getMarkersColor() {#getMarkersColor--}
```
public CellsColor getMarkersColor()
```


Ottiene il colore dei punti in ogni sparkline lineare nel gruppo di sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getNegativePointsColor() {#getNegativePointsColor--}
```
public CellsColor getNegativePointsColor()
```


Ottiene il colore dei valori negativi nel gruppo di sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Indica come tracciare le celle vuote.

Vedi [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotRightToLeft() {#getPlotRightToLeft--}
```
public boolean getPlotRightToLeft()
```


Indica se i dati del grafico sono da destra a sinistra.

**Returns:**
boolean
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Ottiene il tipo di stile predefinito del gruppo di sparkline.

Vedi [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Se questa proprietà è impostata, queste proprietà: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor saranno sovrascritte. Quindi, imposta prima la proprietà, poi le altre.

**Returns:**
int
### getSeriesColor() {#getSeriesColor--}
```
public CellsColor getSeriesColor()
```


Ottiene il colore delle sparkline nel gruppo di sparkline.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getShowFirstPoint() {#getShowFirstPoint--}
```
public boolean getShowFirstPoint()
```


Indica se evidenziare il primo punto dati nel gruppo di sparkline.

**Returns:**
boolean
### getShowHighPoint() {#getShowHighPoint--}
```
public boolean getShowHighPoint()
```


Indica se evidenziare i punti più alti dei dati nel gruppo di sparkline.

**Returns:**
boolean
### getShowHorizontalAxis() {#getShowHorizontalAxis--}
```
public boolean getShowHorizontalAxis()
```


Indica se mostrare l'asse orizzontale dello sparkline. L'asse orizzontale appare se lo sparkline contiene dati che attraversano l'asse zero.

**Returns:**
boolean
### getShowLastPoint() {#getShowLastPoint--}
```
public boolean getShowLastPoint()
```


Indica se evidenziare l'ultimo punto dei dati nel gruppo di sparkline.

**Returns:**
boolean
### getShowLowPoint() {#getShowLowPoint--}
```
public boolean getShowLowPoint()
```


Indica se evidenziare i punti più bassi dei dati nel gruppo di sparkline.

**Returns:**
boolean
### getShowMarkers() {#getShowMarkers--}
```
public boolean getShowMarkers()
```


Indica se evidenziare ogni punto in ciascuna sparkline a linee nel gruppo di sparkline.

**Returns:**
boolean
### getShowNegativePoints() {#getShowNegativePoints--}
```
public boolean getShowNegativePoints()
```


Indica se evidenziare i valori negativi nel gruppo di sparkline con un colore o marcatore diverso.

**Returns:**
boolean
### getSparklineCollection() {#getSparklineCollection--}
```
public SparklineCollection getSparklineCollection()
```


Ottiene la collezione di oggetti [Sparkline](../../com.aspose.cells/sparkline).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà SparklineGroup.Sparklines. Questa proprietà sarà rimossa tra 12 mesi a partire da novembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getSparklines() {#getSparklines--}
```
public SparklineCollection getSparklines()
```


Ottiene la collezione di oggetti [Sparkline](../../com.aspose.cells/sparkline).

**Returns:**
[SparklineCollection](../../com.aspose.cells/sparklinecollection)
### getType() {#getType--}
```
public int getType()
```


Indica il tipo di sparkline del gruppo di sparkline.

Vedi [SparklineType](../../com.aspose.cells/sparklinetype).

**Returns:**
int
### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}
```
public double getVerticalAxisMaxValue()
```


Ottiene il valore massimo personalizzato per l'asse verticale.

**Remarks**

Se questa proprietà è impostata, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) sarà [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}
```
public int getVerticalAxisMaxValueType()
```


Rappresenta il tipo di valore massimo dell'asse verticale.

Vedi [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Returns:**
int
### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}
```
public double getVerticalAxisMinValue()
```


Ottiene il valore minimo personalizzato per l'asse verticale.

**Remarks**

Se questa proprietà è impostata, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) sarà [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Returns:**
double
### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}
```
public int getVerticalAxisMinValueType()
```


Rappresenta il tipo di valore minimo dell'asse verticale.

Vedi [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

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




### resetRanges(String dataRange, boolean isVertical, CellArea locationRange) {#resetRanges-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public void resetRanges(String dataRange, boolean isVertical, CellArea locationRange)
```


Reimposta l'intervallo di dati e l'intervallo di posizione del gruppo sparkline. Questo metodo cancellerà gli elementi sparkline originali nel gruppo e creerà nuovi elementi sparkline per i nuovi intervalli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataRange | java.lang.String | Specifica il nuovo intervallo di dati del gruppo sparkline. |
| isVertical | boolean | Specifica se tracciare gli sparklines dall'intervallo di dati nuovo per riga o per colonna. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Specifica dove posizionare gli sparklines. |

### setDisplayHidden(boolean value) {#setDisplayHidden-boolean-}
```
public void setDisplayHidden(boolean value)
```


Indica se mostrare i dati in righe e colonne nascoste.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFirstPointColor(CellsColor value) {#setFirstPointColor-com.aspose.cells.CellsColor-}
```
public void setFirstPointColor(CellsColor value)
```


Imposta il colore del primo punto dei dati nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHighPointColor(CellsColor value) {#setHighPointColor-com.aspose.cells.CellsColor-}
```
public void setHighPointColor(CellsColor value)
```


Imposta il colore dei punti più alti dei dati nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisColor(CellsColor value) {#setHorizontalAxisColor-com.aspose.cells.CellsColor-}
```
public void setHorizontalAxisColor(CellsColor value)
```


Imposta il colore dell'asse orizzontale nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setHorizontalAxisDateRange(String value) {#setHorizontalAxisDateRange-java.lang.String-}
```
public void setHorizontalAxisDateRange(String value)
```


Rappresenta l'intervallo che contiene i valori di data per i dati di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLastPointColor(CellsColor value) {#setLastPointColor-com.aspose.cells.CellsColor-}
```
public void setLastPointColor(CellsColor value)
```


Imposta il colore dell'ultimo punto dei dati nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setLineWeight(double value) {#setLineWeight-double-}
```
public void setLineWeight(double value)
```


Imposta lo spessore della linea in ogni sparkline a linee nel gruppo di sparkline, nell'unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLowPointColor(CellsColor value) {#setLowPointColor-com.aspose.cells.CellsColor-}
```
public void setLowPointColor(CellsColor value)
```


Imposta il colore dei punti più bassi dei dati nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setMarkersColor(CellsColor value) {#setMarkersColor-com.aspose.cells.CellsColor-}
```
public void setMarkersColor(CellsColor value)
```


Imposta il colore dei punti in ogni sparkline a linee nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setNegativePointsColor(CellsColor value) {#setNegativePointsColor-com.aspose.cells.CellsColor-}
```
public void setNegativePointsColor(CellsColor value)
```


Imposta il colore dei valori negativi nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Indica come tracciare le celle vuote.

Vedi [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPlotRightToLeft(boolean value) {#setPlotRightToLeft-boolean-}
```
public void setPlotRightToLeft(boolean value)
```


Indica se i dati del grafico sono da destra a sinistra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Imposta il tipo di stile predefinito del gruppo di sparkline.

Vedi [SparklinePresetStyleType](../../com.aspose.cells/sparklinepresetstyletype).

**Remarks**

Se questa proprietà è impostata, queste proprietà: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor saranno sovrascritte. Quindi, imposta prima la proprietà, poi le altre.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSeriesColor(CellsColor value) {#setSeriesColor-com.aspose.cells.CellsColor-}
```
public void setSeriesColor(CellsColor value)
```


Imposta il colore delle sparkline nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setShowFirstPoint(boolean value) {#setShowFirstPoint-boolean-}
```
public void setShowFirstPoint(boolean value)
```


Indica se evidenziare il primo punto dati nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowHighPoint(boolean value) {#setShowHighPoint-boolean-}
```
public void setShowHighPoint(boolean value)
```


Indica se evidenziare i punti più alti dei dati nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowHorizontalAxis(boolean value) {#setShowHorizontalAxis-boolean-}
```
public void setShowHorizontalAxis(boolean value)
```


Indica se mostrare l'asse orizzontale dello sparkline. L'asse orizzontale appare se lo sparkline contiene dati che attraversano l'asse zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowLastPoint(boolean value) {#setShowLastPoint-boolean-}
```
public void setShowLastPoint(boolean value)
```


Indica se evidenziare l'ultimo punto dei dati nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowLowPoint(boolean value) {#setShowLowPoint-boolean-}
```
public void setShowLowPoint(boolean value)
```


Indica se evidenziare i punti più bassi dei dati nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowMarkers(boolean value) {#setShowMarkers-boolean-}
```
public void setShowMarkers(boolean value)
```


Indica se evidenziare ogni punto in ciascuna sparkline a linee nel gruppo di sparkline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowNegativePoints(boolean value) {#setShowNegativePoints-boolean-}
```
public void setShowNegativePoints(boolean value)
```


Indica se evidenziare i valori negativi nel gruppo di sparkline con un colore o marcatore diverso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Indica il tipo di sparkline del gruppo di sparkline.

Vedi [SparklineType](../../com.aspose.cells/sparklinetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVerticalAxisMaxValue(double value) {#setVerticalAxisMaxValue-double-}
```
public void setVerticalAxisMaxValue(double value)
```


Imposta il valore massimo personalizzato per l'asse verticale.

**Remarks**

Se questa proprietà è impostata, [getVerticalAxisMaxValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMaxValueType--) sarà [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setVerticalAxisMaxValue(int type, double value) {#setVerticalAxisMaxValue-int-double-}
```
public void setVerticalAxisMaxValue(int type, double value)
```


Imposta il valore massimo personalizzato per l'asse verticale dello sparkline con il tipo di valore dell'asse specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Tipo che specifica come viene applicato il valore massimo dell'asse. |
| value | double | Valore massimo personalizzato dell'asse verticale. Ignorato se il tipo non è [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMaxValueType(int value) {#setVerticalAxisMaxValueType-int-}
```
public void setVerticalAxisMaxValueType(int value)
```


Rappresenta il tipo di valore massimo dell'asse verticale.

Vedi [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVerticalAxisMinValue(double value) {#setVerticalAxisMinValue-double-}
```
public void setVerticalAxisMinValue(double value)
```


Imposta il valore minimo personalizzato per l'asse verticale.

**Remarks**

Se questa proprietà è impostata, [getVerticalAxisMinValueType()](../../com.aspose.cells/sparklinegroup\#getVerticalAxisMinValueType--) sarà [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setVerticalAxisMinValue(int type, double value) {#setVerticalAxisMinValue-int-double-}
```
public void setVerticalAxisMinValue(int type, double value)
```


Imposta il valore minimo personalizzato per l'asse verticale dello sparkline con il tipo di valore dell'asse specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype). Tipo che specifica come viene applicato il valore minimo dell'asse. |
| value | double | Valore minimo personalizzato dell'asse verticale. Ignorato se il tipo non è [SparklineAxisMinMaxType.CUSTOM](../../com.aspose.cells/sparklineaxisminmaxtype\#CUSTOM). |

### setVerticalAxisMinValueType(int value) {#setVerticalAxisMinValueType-int-}
```
public void setVerticalAxisMinValueType(int value)
```


Rappresenta il tipo di valore minimo dell'asse verticale.

Vedi [SparklineAxisMinMaxType](../../com.aspose.cells/sparklineaxisminmaxtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

