---
title: "SeriesCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

Encapsula una colección de objetos [Series](../../com.aspose.cells/series).

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
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | Agrega la colección de [Series](../../com.aspose.cells/series) a un gráfico. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | Agrega la colección de [Series](../../com.aspose.cells/series) a un gráfico. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | Agrega la colección de [Series](../../com.aspose.cells/series) a un gráfico. |
| [changeColors(int type)](#changeColors-int-) | Establece una paleta monocromática para las series del gráfico. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | Cambia directamente el orden de las dos series. |
| [clear()](#clear--) | Limpia la colección |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [Series](../../com.aspose.cells/series) en el índice especificado. |
| [getCategoryData()](#getCategoryData--) | Obtiene el rango de valores del eje de categoría. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [getSecondCategoryData()](#getSecondCategoryData--) | Obtiene el rango de valores del segundo eje de categoría. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | Obtiene el elemento [Series](../../com.aspose.cells/series) por orden. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [isColorVaried()](#isColorVaried--) | Representa si el color de los puntos varía. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina una serie en el índice específico. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | Establece el rango de valores del eje de categoría. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Representa si el color de los puntos varía. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | Establece el rango de valores del segundo eje de categoría. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | Establece los nombres de todas las series en el gráfico. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | Cambia directamente el orden de las dos series. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


Agrega la colección de [Series](../../com.aspose.cells/series) a un gráfico.

**Remarks**


Si se establecen datos en celdas contiguas, use dos puntos para separarlas. Por ejemplo, $C$2:$C$5.

Si se establecen datos en celdas no contiguas, use coma para separarlas. Por ejemplo: ($C$2,$D$5).

Este método solo procesa simplemente como rango de datos. Si desea comprobar de forma inteligente el método ChartCollection.Add().


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataArea | java.lang.String | Especifica los valores desde los cuales trazar la serie de datos |
| isVertical | boolean | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. Si es verdadero, [Series](../../com.aspose.cells/series) se añadirá columna por columna |

**Returns:**
int - Devuelve el primer índice de la ASeries añadida en la NSeries.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


Agrega la colección de [Series](../../com.aspose.cells/series) a un gráfico.

**Remarks**


Si se establecen datos en celdas contiguas, use dos puntos para separarlas. Por ejemplo, $C$2:$C$5.

Si se establecen datos en celdas no contiguas, use coma para separarlas. Por ejemplo, ($C$2,$D$5).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | java.lang.String | Especifica los valores desde los cuales trazar la serie de datos |
| isVertical | boolean | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |
| checkLabels | boolean | Indica si el rango contiene el nombre de la serie |

**Returns:**
int - Devuelve el primer índice de la ASeries añadida en la NSeries.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


Agrega la colección de [Series](../../com.aspose.cells/series) a un gráfico.

**Remarks**


Si se establecen datos en celdas contiguas, use dos puntos para separarlas. Por ejemplo, R[1]C[1]:R[3]C[2].

Si se establecen datos en celdas contiguas, use coma para separarlas. Por ejemplo, (R[1]C[1],R[3]C[2]).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | java.lang.String | Especifica los valores desde los cuales trazar la serie de datos |
| isVertical | boolean | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |

**Returns:**
int - Devuelve el primer índice de la ASeries añadida en la NSeries.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


Establece una paleta monocromática para las series del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). El tipo monocromático. |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


Cambia directamente el orden de las dos series.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método SeriesCollection.SwapSeries. Este método será eliminado 12 meses después, a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceIndex | int | El índice actual |
| destIndex | int | El índice de destino |

### clear() {#clear--}
```
public void clear()
```


Limpia la colección

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
public Series get(int index)
```


Obtiene el elemento [Series](../../com.aspose.cells/series) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


Obtiene el rango de valores del eje de categoría. Puede ser un rango de celdas (como "d1:e10") o una secuencia de valores (como "\{2,6,8,10\}").

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


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


Obtiene el rango de valores del segundo eje de categoría. Puede ser un rango de celdas (como "d1:e10"), o una secuencia de valores (como "\{2,6,8,10\}"). Solo tiene efecto cuando algunas series se trazan en el segundo eje.

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


Obtiene el elemento [Series](../../com.aspose.cells/series) por orden.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| order | int | El orden de las series |

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


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Representa si el color de los puntos varía.

**Remarks**

Solo funciona para gráficos de pastel o cuando hay solo una serie.

**Returns:**
boolean
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


Elimina una serie en el índice específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice. |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


Establece el rango de valores del eje de categoría. Puede ser un rango de celdas (como "d1:e10") o una secuencia de valores (como "\{2,6,8,10\}").

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Representa si el color de los puntos varía.

**Remarks**

Solo funciona para gráficos de pastel o cuando hay solo una serie.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


Establece el rango de valores del segundo eje de categoría. Puede ser un rango de celdas (como "d1:e10"), o una secuencia de valores (como "\{2,6,8,10\}"). Solo tiene efecto cuando algunas series se trazan en el segundo eje.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


Establece los nombres de todas las series en el gráfico.

**Remarks**


Si el índice de inicio es mayor que la cantidad de series, devolverá y no hará nada.

Si se establecen datos en celdas contiguas, use dos puntos para separarlas. Por ejemplo, $C$2:$C$5.

Si se establecen datos en celdas contiguas, use una coma para separarlas. Por ejemplo, ($C$2,$D$5).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice de la primera serie cuyo nombre desea establecer. |
| area | java.lang.String | Especifica el área para el nombre de la serie. |
| isVertical | boolean | >Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


Cambia directamente el orden de las dos series.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceIndex | int | El índice actual |
| destIndex | int | El índice de destino |

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

