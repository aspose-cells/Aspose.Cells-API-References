---
title: "TrendlineCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una colección de todos los objetos para la serie de datos especificada."
type: docs
url: /es/java/com.aspose.cells/trendlinecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TrendlineCollection extends CollectionBase
```

Representa una colección de todos los objetos [Trendline](../../com.aspose.cells/trendline) para la serie de datos especificada.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         worksheet.getCells().get("A1").putValue(50);
         worksheet.getCells().get("A2").putValue(100);
         worksheet.getCells().get("A3").putValue(150);
         worksheet.getCells().get("A4").putValue(200);
         worksheet.getCells().get("B1").putValue(60);
         worksheet.getCells().get("B2").putValue(32);
         worksheet.getCells().get("B3").putValue(50);
         worksheet.getCells().get("B4").putValue(40);
 
         //Adding a chart to the worksheet
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 3, 3, 15, 10);
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:a3", true);
         chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR, "MyTrendLine");
         Trendline line = chart.getNSeries().get(0).getTrendLines().get(0);
         line.setDisplayEquation(true);
         line.setDisplayRSquared(true);
         line.setColor(Color.getRed());
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int type)](#add-int-) | Agrega un objeto [Trendline](../../com.aspose.cells/trendline) a esta colección con el tipo especificado. |
| [add(int type, String name)](#add-int-java.lang.String-) | Agrega un objeto [Trendline](../../com.aspose.cells/trendline) a esta colección con el tipo y nombre especificados. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene un objeto [Trendline](../../com.aspose.cells/trendline) por su índice. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int type) {#add-int-}
```
public int add(int type)
```


Agrega un objeto [Trendline](../../com.aspose.cells/trendline) a esta colección con el tipo especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [TrendlineType](../../com.aspose.cells/trendlinetype). Tipo de línea de tendencia. |

**Returns:**
int - índice del objeto [Trendline](../../com.aspose.cells/trendline).
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


Agrega un objeto [Trendline](../../com.aspose.cells/trendline) a esta colección con el tipo y nombre especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [TrendlineType](../../com.aspose.cells/trendlinetype). Tipo de línea de tendencia. |
| name | java.lang.String | Nombre de la línea de tendencia. |

**Returns:**
int - índice del objeto [Trendline](../../com.aspose.cells/trendline).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### clear() {#clear--}
```
public void clear()
```


Elimina todos los objetos de la instancia de CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Trendline get(int index)
```


Obtiene un objeto [Trendline](../../com.aspose.cells/trendline) por su índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
[Trendline](../../com.aspose.cells/trendline)
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


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
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


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Devuelve un enumerador que recorre la instancia de CollectionBase.

**Returns:**
java.util.Iterator - Un iterador para la instancia de CollectionBase.
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


Elimina el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento a eliminar. |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

