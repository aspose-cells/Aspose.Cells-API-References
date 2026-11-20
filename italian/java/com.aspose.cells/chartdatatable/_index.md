---
title: "ChartDataTable"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una tabella dati del grafico."
type: docs
url: /it/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

Rappresenta una tabella dati del grafico.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. |
| [getBackgroundMode()](#getBackgroundMode--) | Restituisce la modalità di visualizzazione dello sfondo |
| [getBorder()](#getBorder--) | Restituisce un oggetto Border che rappresenta il bordo dell'oggetto |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Ottiene un oggetto [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) che rappresenta l'impostazione del carattere della tabella dati del grafico specificata. |
| [getShowLegendKey()](#getShowLegendKey--) | True se la chiave della legenda dell'etichetta dati è visibile. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | True se la tabella dati del grafico ha bordi orizzontali delle celle |
| [hasBorderOutline()](#hasBorderOutline--) | True se la tabella dati del grafico ha bordi di contorno |
| [hasBorderVertical()](#hasBorderVertical--) | True se la tabella dati del grafico ha bordi verticali delle celle |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | True se la tabella dati del grafico ha bordi orizzontali delle celle |
| [hasOutlineBorder()](#hasOutlineBorder--) | True se la tabella dati del grafico ha bordi di contorno |
| [hasVerticalBorder()](#hasVerticalBorder--) | True se la tabella dati del grafico ha bordi verticali delle celle |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Imposta la modalità di visualizzazione dello sfondo |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | True se la tabella dati del grafico ha bordi orizzontali delle celle |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | True se la tabella dati del grafico ha bordi di contorno |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | True se la tabella dati del grafico ha bordi verticali delle celle |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | True se la tabella dati del grafico ha bordi orizzontali delle celle |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | True se la tabella dati del grafico ha bordi di contorno |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | True se la tabella dati del grafico ha bordi verticali delle celle |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | True se la chiave della legenda dell'etichetta dati è visibile. |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Restituisce la modalità di visualizzazione dello sfondo

Vedi [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Restituisce un oggetto Border che rappresenta il bordo dell'oggetto

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


Ottiene un oggetto [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) che rappresenta l'impostazione del carattere della tabella dati del grafico specificata.

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


True se la chiave della legenda dell'etichetta dati è visibile.

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


True se la tabella dati del grafico ha bordi orizzontali delle celle

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartDataTable.HasHorizontalBorder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


True se la tabella dati del grafico ha bordi di contorno

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartDataTable.HasOutlineBorder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


True se la tabella dati del grafico ha bordi verticali delle celle

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartDataTable.HasVerticalBorder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


True se la tabella dati del grafico ha bordi orizzontali delle celle

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


True se la tabella dati del grafico ha bordi di contorno

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


True se la tabella dati del grafico ha bordi verticali delle celle

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


True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Imposta la modalità di visualizzazione dello sfondo

Vedi [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


True se la tabella dati del grafico ha bordi orizzontali delle celle

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartDataTable.HasHorizontalBorder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


True se la tabella dati del grafico ha bordi di contorno

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartDataTable.HasOutlineBorder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


True se la tabella dati del grafico ha bordi verticali delle celle

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartDataTable.HasVerticalBorder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


True se la tabella dati del grafico ha bordi orizzontali delle celle

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


True se la tabella dati del grafico ha bordi di contorno

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


True se la tabella dati del grafico ha bordi verticali delle celle

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


True se la chiave della legenda dell'etichetta dati è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

