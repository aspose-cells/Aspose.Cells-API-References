---
title: "SeriesCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

Incapsula una raccolta di oggetti [Series](../../com.aspose.cells/series).

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
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | Aggiunge la raccolta [Series](../../com.aspose.cells/series) a un grafico. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | Aggiunge la raccolta [Series](../../com.aspose.cells/series) a un grafico. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | Aggiunge la raccolta [Series](../../com.aspose.cells/series) a un grafico. |
| [changeColors(int type)](#changeColors-int-) | Imposta la palette monocromatica per le serie del grafico. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | Modifica direttamente l'ordine delle due serie. |
| [clear()](#clear--) | Cancella la raccolta |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Restituisce l'elemento [Series](../../com.aspose.cells/series) all'indice specificato. |
| [getCategoryData()](#getCategoryData--) | Restituisce l'intervallo dei valori dell'asse di categoria. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [getSecondCategoryData()](#getSecondCategoryData--) | Restituisce l'intervallo dei valori del secondo asse di categoria. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | Restituisce l'elemento [Series](../../com.aspose.cells/series) per ordine. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [isColorVaried()](#isColorVaried--) | Rappresenta se il colore dei punti è variabile. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove una serie all'indice specificato. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | Imposta l'intervallo dei valori dell'asse di categoria. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Rappresenta se il colore dei punti è variabile. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | Imposta l'intervallo dei valori del secondo asse di categoria. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | Imposta i nomi di tutte le serie nel grafico. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | Modifica direttamente l'ordine delle due serie. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


Aggiunge la raccolta [Series](../../com.aspose.cells/series) a un grafico.

**Remarks**


Se i dati sono impostati su celle contigue, usa i due punti per separarle. Ad esempio, $C$2:$C$5.

Se i dati sono impostati su celle non contigue, usa la virgola per separarle. Ad esempio: ($C$2,$D$5).

Questo metodo elabora semplicemente come intervallo di dati. Se vuoi verificare in modo intelligente il metodo ChartCollection.Add().


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataArea | java.lang.String | Specifica i valori da cui tracciare la serie di dati |
| isVertical | boolean | Specifica se tracciare la serie da un intervallo di valori di celle per riga o per colonna. Se vero, [Series](../../com.aspose.cells/series) verrà aggiunto colonna per colonna |

**Returns:**
int - Restituisce il primo indice della ASeries aggiunta in NSeries.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


Aggiunge la raccolta [Series](../../com.aspose.cells/series) a un grafico.

**Remarks**


Se i dati sono impostati su celle contigue, usa i due punti per separarle. Per esempio, $C$2:$C$5.

Se i dati sono impostati su celle non contigue, usa la virgola per separarle. Per esempio, ($C$2,$D$5).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | java.lang.String | Specifica i valori da cui tracciare la serie di dati |
| isVertical | boolean | Specifica se tracciare la serie da un intervallo di valori di celle per riga o per colonna. |
| checkLabels | boolean | Indica se l'intervallo contiene il nome della serie |

**Returns:**
int - Restituisce il primo indice della ASeries aggiunta in NSeries.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


Aggiunge la raccolta [Series](../../com.aspose.cells/series) a un grafico.

**Remarks**


Se i dati sono impostati su celle contigue, usa i due punti per separarle. Per esempio, R[1]C[1]:R[3]C[2].

Se i dati sono impostati su celle contigue, usa la virgola per separarle. Per esempio, (R[1]C[1],R[3]C[2]).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | java.lang.String | Specifica i valori da cui tracciare la serie di dati |
| isVertical | boolean | Specifica se tracciare la serie da un intervallo di valori di celle per riga o per colonna. |

**Returns:**
int - Restituisce il primo indice della ASeries aggiunta in NSeries.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


Imposta la palette monocromatica per le serie del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). Il tipo monocromatico. |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


Modifica direttamente l'ordine delle due serie.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo SeriesCollection.SwapSeries. Questo metodo sarà rimosso 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceIndex | int | L'indice corrente |
| destIndex | int | L'indice di destinazione |

### clear() {#clear--}
```
public void clear()
```


Cancella la raccolta

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
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
### get(int index) {#get-int-}
```
public Series get(int index)
```


Restituisce l'elemento [Series](../../com.aspose.cells/series) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


Ottiene l'intervallo dei valori dell'asse di categoria. Può essere un intervallo di celle (ad esempio "d1:e10") o una sequenza di valori (ad esempio "\{2,6,8,10\}").

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


Ottiene l'intervallo dei valori del secondo asse di categoria. Può essere un intervallo di celle (ad esempio, "d1:e10"), o una sequenza di valori (ad esempio, "\{2,6,8,10\}"). Ha effetto solo quando alcune serie sono state tracciate sul secondo asse.

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


Restituisce l'elemento [Series](../../com.aspose.cells/series) per ordine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| order | int | L'ordine delle serie |

**Returns:**
[Series](../../com.aspose.cells/series) - The element series
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Rappresenta se il colore dei punti è variabile.

**Remarks**

Funziona solo per i grafici a torta o quando c'è una sola serie.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove una serie all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice. |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


Imposta l'intervallo dei valori dell'asse di categoria. Può essere un intervallo di celle (ad esempio "d1:e10") o una sequenza di valori (ad esempio "\\{2,6,8,10\\}").

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Rappresenta se il colore dei punti è variabile.

**Remarks**

Funziona solo per i grafici a torta o quando c'è una sola serie.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


Imposta l'intervallo dei valori del secondo asse di categoria. Può essere un intervallo di celle (ad esempio, "d1:e10"), o una sequenza di valori (ad esempio,"\\{2,6,8,10\\}"). Ha effetto solo quando alcune serie sono state tracciate sul secondo asse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


Imposta i nomi di tutte le serie nel grafico.

**Remarks**


Se l'indice di partenza è più grande del conteggio delle serie, ritornerà e non farà nulla.

Se i dati sono impostati su celle contigue, usa i due punti per separarle. Per esempio, $C$2:$C$5.

Se i dati sono impostati su celle contigue, usa la virgola per separarle. Per esempio, ($C$2,$D$5).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice della prima serie per cui vuoi impostare il nome. |
| area | java.lang.String | Specifica l'area per il nome della serie. |
| isVertical | boolean | >Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna. |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


Modifica direttamente l'ordine delle due serie.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceIndex | int | L'indice corrente |
| destIndex | int | L'indice di destinazione |

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

