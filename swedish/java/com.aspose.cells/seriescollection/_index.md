---
title: "SeriesCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

Inkapslar en samling av [Series](../../com.aspose.cells/series)-objekt.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | Lägger till [Series](../../com.aspose.cells/series)-samlingen i ett diagram. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | Lägger till [Series](../../com.aspose.cells/series)-samlingen i ett diagram. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | Lägger till [Series](../../com.aspose.cells/series)-samlingen i ett diagram. |
| [changeColors(int type)](#changeColors-int-) | Ställ in monokromatisk palett för diagramserier. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | Ändrar direkt ordningen på de två serierna. |
| [clear()](#clear--) | Rensar samlingen |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [Series](../../com.aspose.cells/series)-elementet på det angivna indexet. |
| [getCategoryData()](#getCategoryData--) | Hämtar intervallet för kategori-axelvärden. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [getSecondCategoryData()](#getSecondCategoryData--) | Hämtar intervallet för sekundära kategori-axelvärden. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | Hämtar [Series](../../com.aspose.cells/series)-elementet efter ordning. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [isColorVaried()](#isColorVaried--) | Anger om färgen på punkterna varierar. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Ta bort en serie på det specifika indexet. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | Ställer in intervallet för kategori-axelvärden. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Anger om färgen på punkterna varierar. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | Ställer in intervallet för sekundära kategori‑Axis‑värden. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | Ställer in namnen på alla serier i diagrammet. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | Ändrar direkt ordningen på de två serierna. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


Lägger till [Series](../../com.aspose.cells/series)-samlingen i ett diagram.

**Remarks**


Om data anges i sammanhängande celler, använd kolon för att separera dem. Till exempel, $C$2:$C$5.

Om data anges i icke‑sammanhängande celler, använd kommatecken för att separera dem. Till exempel: ($C$2,$D$5).

Denna metod behandlar bara enkelt som dataområde. Om du vill smart kontrollera metoden ChartCollection.Add().


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataArea | java.lang.String | Anger värden som dataserien ska plottas från |
| isVertical | boolean | Anger om serierna ska plottas från ett cellvärdesintervall radvis eller kolumnvis. Om sant kommer [Series](../../com.aspose.cells/series) att läggas till kolumn för kolumn. |

**Returns:**
int – Returnerar det första indexet för den tillagda ASeries i NSeries.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


Lägger till [Series](../../com.aspose.cells/series)-samlingen i ett diagram.

**Remarks**


Om data anges i sammanhängande celler, använd kolon för att separera dem. Till exempel, $C$2:$C$5.

Om data anges i icke‑sammanhängande celler, använd kommatecken för att separera dem. Till exempel, ($C$2,$D$5).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | java.lang.String | Anger värden som dataserien ska plottas från |
| isVertical | boolean | Anger om serierna ska plottas från ett cellvärdesintervall radvis eller kolumnvis. |
| checkLabels | boolean | Anger om intervallet innehåller seriens namn |

**Returns:**
int – Returnerar det första indexet för den tillagda ASeries i NSeries.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


Lägger till [Series](../../com.aspose.cells/series)-samlingen i ett diagram.

**Remarks**


Om data anges i sammanhängande celler, använd kolon för att separera dem. Till exempel, R[1]C[1]:R[3]C[2].

Om data anges i sammanhängande celler, använd kommatecken för att separera dem. Till exempel, (R[1]C[1],R[3]C[2]).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | java.lang.String | Anger värden som dataserien ska plottas från |
| isVertical | boolean | Anger om serierna ska plottas från ett cellvärdesintervall radvis eller kolumnvis. |

**Returns:**
int – Returnerar det första indexet för den tillagda ASeries i NSeries.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


Ställ in monokromatisk palett för diagramserier.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). Den monokromatiska typen. |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


Ändrar direkt ordningen på de två serierna.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden SeriesCollection.SwapSeries. Denna metod kommer att tas bort 12 månader senare från och med juni 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceIndex | int | Det aktuella indexet |
| destIndex | int | Det destinationindexet |

### clear() {#clear--}
```
public void clear()
```


Rensar samlingen

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Series get(int index)
```


Hämtar [Series](../../com.aspose.cells/series)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


Hämtar intervallet för kategori Axis‑värden. Det kan vara ett cellintervall (t.ex. "d1:e10") eller en sekvens av värden (t.ex. "\{2,6,8,10\}").

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


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


Hämtar intervallet för sekundära kategori Axis‑värden. Det kan vara ett cellintervall (t.ex. "d1:e10"), eller en sekvens av värden (t.ex. "\{2,6,8,10\}"). Gäller endast när vissa serier har plottats på den sekundära axeln.

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


Hämtar [Series](../../com.aspose.cells/series)-elementet efter ordning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ordning | int | Ordningen för serierna |

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


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Anger om färgen på punkterna varierar.

**Remarks**

Fungerar endast för cirkeldiagram eller när det bara finns en serie.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
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


Ta bort en serie på det specifika indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


Ställer in intervallet för kategoriaxelns värden. Det kan vara ett cellintervall (t.ex. "d1:e10") eller en sekvens av värden (t.ex. "\{2,6,8,10\}").

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Anger om färgen på punkterna varierar.

**Remarks**

Fungerar endast för cirkeldiagram eller när det bara finns en serie.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


Ställer in intervallet för den andra kategoriaxelns värden. Det kan vara ett cellintervall (t.ex. "d1:e10"), eller en sekvens av värden (t.ex. "\{2,6,8,10\}"). Påverkar endast när vissa serier har plottats på den andra axeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


Ställer in namnen på alla serier i diagrammet.

**Remarks**


Om startindexet är större än antalet serier, kommer den att returnera och göra ingenting.

Om data anges i sammanhängande celler, använd kolon för att separera dem. Till exempel, $C$2:$C$5.

Om du anger data i sammanhängande celler, använd kommatecken för att separera dem. Till exempel ($C$2,$D$5).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Indexet för den första serien som du vill ange namn för. |
| area | java.lang.String | Anger området för seriens namn. |
| isVertical | boolean | >Anger om serien ska plottas från ett intervall av cellvärden radvis eller kolumnvis. |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


Ändrar direkt ordningen på de två serierna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceIndex | int | Det aktuella indexet |
| destIndex | int | Det destinationindexet |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

