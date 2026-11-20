---
title: "SeriesCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

Kapselt eine Sammlung von [Series](../../com.aspose.cells/series)-Objekten.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | Fügt die [Series](../../com.aspose.cells/series)-Sammlung zu einem Diagramm hinzu. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | Fügt die [Series](../../com.aspose.cells/series)-Sammlung zu einem Diagramm hinzu. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | Fügt die [Series](../../com.aspose.cells/series)-Sammlung zu einem Diagramm hinzu. |
| [changeColors(int type)](#changeColors-int-) | Monochromatische Palette für Diagrammserien festlegen. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | Ändert direkt die Reihenfolge der beiden Serien. |
| [clear()](#clear--) | Leert die Sammlung |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liest das [Series](../../com.aspose.cells/series)-Element am angegebenen Index. |
| [getCategoryData()](#getCategoryData--) | Liest den Bereich der Kategorienachsenwerte. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [getSecondCategoryData()](#getSecondCategoryData--) | Liest den Bereich der zweiten Kategorienachsenwerte. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | Ermittelt das [Series](../../com.aspose.cells/series)-Element nach Reihenfolge. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [isColorVaried()](#isColorVaried--) | Gibt an, ob die Farbe der Punkte variiert. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt eine Serie am angegebenen Index. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | Legt den Wertebereich der Kategorienachse fest. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Gibt an, ob die Farbe der Punkte variiert. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | Legt den Wertebereich der zweiten Kategorienachse fest. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | Setzt die Namen aller Serien im Diagramm. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | Ändert direkt die Reihenfolge der beiden Serien. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


Fügt die [Series](../../com.aspose.cells/series)-Sammlung zu einem Diagramm hinzu.

**Remarks**


Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie einen Doppelpunkt, um sie zu trennen. Zum Beispiel, $C$2:$C$5.

Wenn Daten in nicht zusammenhängenden Zellen festgelegt werden, verwenden Sie ein Komma, um sie zu trennen. Zum Beispiel: ($C$2,$D$5).

Diese Methode verarbeitet nur einfach den Bereich als Datenbereich. Wenn Sie die Methode ChartCollection.Add() intelligent prüfen möchten.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataArea | java.lang.String | Gibt die Werte an, aus denen die Datenreihe geplottet wird. |
| isVertical | boolean | Gibt an, ob die Serie aus einem Zellwertbereich zeilenweise oder spaltenweise geplottet werden soll. Wenn true, wird [Series](../../com.aspose.cells/series) spaltenweise hinzugefügt. |

**Returns:**
int – Gibt den ersten Index der hinzugefügten ASeries in der NSeries zurück.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


Fügt die [Series](../../com.aspose.cells/series)-Sammlung zu einem Diagramm hinzu.

**Remarks**


Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie einen Doppelpunkt, um sie zu trennen. Zum Beispiel, $C$2:$C$5.

Wenn Daten in nicht zusammenhängenden Zellen festgelegt werden, verwenden Sie ein Komma, um sie zu trennen. Zum Beispiel, ($C$2,$D$5).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | java.lang.String | Gibt die Werte an, aus denen die Datenreihe geplottet wird. |
| isVertical | boolean | Gibt an, ob die Serie aus einem Zellwertbereich zeilenweise oder spaltenweise geplottet werden soll. |
| checkLabels | boolean | Gibt an, ob der Bereich den Namen der Serie enthält. |

**Returns:**
int – Gibt den ersten Index der hinzugefügten ASeries in der NSeries zurück.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


Fügt die [Series](../../com.aspose.cells/series)-Sammlung zu einem Diagramm hinzu.

**Remarks**


Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie einen Doppelpunkt, um sie zu trennen. Zum Beispiel, R[1]C[1]:R[3]C[2].

Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie ein Komma, um sie zu trennen. Zum Beispiel, (R[1]C[1],R[3]C[2]).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | java.lang.String | Gibt die Werte an, aus denen die Datenreihe geplottet wird. |
| isVertical | boolean | Gibt an, ob die Serie aus einem Zellwertbereich zeilenweise oder spaltenweise geplottet werden soll. |

**Returns:**
int – Gibt den ersten Index der hinzugefügten ASeries in der NSeries zurück.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


Monochromatische Palette für Diagrammserien festlegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). Der monochrome Typ. |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


Ändert direkt die Reihenfolge der beiden Serien.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode SeriesCollection.SwapSeries. Diese Methode wird 12 Monate später, seit Juni 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceIndex | int | Der aktuelle Index |
| destIndex | int | Der Zielindex |

### clear() {#clear--}
```
public void clear()
```


Leert die Sammlung

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
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
### get(int index) {#get-int-}
```
public Series get(int index)
```


Liest das [Series](../../com.aspose.cells/series)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


Liest den Bereich der Kategorien-Achsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10") oder eine Wertefolge (z. B. "\{2,6,8,10\}").

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


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


Liest den Bereich der zweiten Kategorien-Achsenwerte. Es kann ein Zellbereich sein (z. B., "d1:e10"), oder eine Wertefolge (z. B.,"\{2,6,8,10\}"). Wirkt nur, wenn einige Serien auf der zweiten Achse geplottet wurden.

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


Ermittelt das [Series](../../com.aspose.cells/series)-Element nach Reihenfolge.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Reihenfolge | int | Die Reihenfolge der Serien. |

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


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Gibt an, ob die Farbe der Punkte variiert.

**Remarks**

Funktioniert nur für Kreisdiagramme oder wenn nur eine Serie vorhanden ist.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
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


Entfernt eine Serie am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


Legt den Bereich der Kategorien-Achsenwerte fest. Es kann ein Zellbereich sein (z. B. "d1:e10") oder eine Wertefolge (z. B. "\{2,6,8,10\}").

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Gibt an, ob die Farbe der Punkte variiert.

**Remarks**

Funktioniert nur für Kreisdiagramme oder wenn nur eine Serie vorhanden ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


Legt den Bereich der zweiten Kategorien-Achsenwerte fest. Es kann ein Zellbereich sein (z. B., "d1:e10"), oder eine Wertefolge (z. B.,"\{2,6,8,10\}"). Wirkt nur, wenn einige Serien auf der zweiten Achse geplottet wurden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


Setzt die Namen aller Serien im Diagramm.

**Remarks**


Wenn der Startindex größer ist als die Anzahl der Serien, wird zurückgekehrt und es wird nichts getan.

Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie einen Doppelpunkt, um sie zu trennen. Zum Beispiel, $C$2:$C$5.

Wenn Daten in zusammenhängenden Zellen gesetzt werden, verwenden Sie ein Komma, um sie zu trennen. Zum Beispiel ($C$2,$D$5).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Index der ersten Serie, deren Namen Sie festlegen möchten. |
| area | java.lang.String | Gibt den Bereich für den Seriennamen an. |
| isVertical | boolean | >Gibt an, ob die Serie aus einem Zellbereich zeilenweise oder spaltenweise geplottet werden soll. |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


Ändert direkt die Reihenfolge der beiden Serien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceIndex | int | Der aktuelle Index |
| destIndex | int | Der Zielindex |

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

