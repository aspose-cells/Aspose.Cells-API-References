---
title: "ChartPointCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une collection qui contient tous les points d'une série."
type: docs
url: /fr/java/com.aspose.cells/chartpointcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ChartPointCollection implements Iterable
```

Représente une collection qui contient tous les points d'une série.

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
         int chartIndex = worksheet.getCharts().add(ChartType.PIE_EXPLODED, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Show Data Labels 
         chart.getNSeries().get(0).getDataLabels().setShowValue(true);
 
         ChartPointCollection points = chart.getNSeries().get(0).getPoints();
 
         for (int i = 0; i <points.getCount(); i++)
         {
             //Get Data Point
             ChartPoint point = points.get(i);
             //Set Pir Explosion
             point.setExplosion(15);
             //Set Border Color
             point.getBorder().setColor(com.aspose.cells.Color.getRed());
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [clear()](#clear--) | Supprime tous les paramètres des points du graphique. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [ChartPoint](../../com.aspose.cells/chartpoint) à l'index spécifié dans la série. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre de points du graphique. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Renvoie un énumérateur pour l'ensemble de la [ChartPointCollection](../../com.aspose.cells/chartpointcollection). |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime le point à l'index de la série. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Supprime tous les paramètres des points du graphique.

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
### get(int index) {#get-int-}
```
public ChartPoint get(int index)
```


Obtient l'élément [ChartPoint](../../com.aspose.cells/chartpoint) à l'index spécifié dans la série.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index du point de graphique dans la série. |

**Returns:**
[ChartPoint](../../com.aspose.cells/chartpoint) - The ChartPoint object.
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


Obtient le nombre de points du graphique.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Renvoie un énumérateur pour l'ensemble de la [ChartPointCollection](../../com.aspose.cells/chartpointcollection).

**Returns:**
java.util.Iterator -
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


Supprime le point à l'index de la série.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index du point. |

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

