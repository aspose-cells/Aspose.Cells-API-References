---
title: "ColumnCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Colección de los objetos que representan la configuración individual de columnas en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/columncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ColumnCollection extends CollectionBase
```

Colección de los objetos [Column](../../com.aspose.cells/column) que representan la configuración individual de columnas en una hoja de cálculo. El objeto Column solo representa configuraciones como el ancho de columna, estilos, etc., para toda la columna, y no tiene nada que ver con si existen celdas no vacías (datos) o no en la columna correspondiente. Y el "Count" de esta colección solo representa la cantidad de objetos Column que se han instanciado en esta colección, sin relación con la existencia de celdas no vacías (datos) en la hoja de cálculo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Add new Style to Workbook
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setForegroundColor(Color.getBlue());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.SOLID);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Change the default width of first ten columns
         for (int i = 0; i ? i++)
         {
             worksheet.getCells().getColumns().get(i).setWidth(20);
         }
 
         //Get the Column with non default formatting
         ColumnCollection columns = worksheet.getCells().getColumns();
 
         for (Column column : (Iterable<Column>) columns)
         {
             //Apply Style to first ten Columns
             column.applyStyle(style, styleFlag);
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int columnIndex)](#get-int-) | Obtiene un objeto [Column](../../com.aspose.cells/column) por índice de columna. |
| [getByIndex(int index)](#getByIndex-int-) | Obtiene el objeto de columna por el índice. |
| [getClass()](#getClass--) |  |
| [getColumnByIndex(int index)](#getColumnByIndex-int-) | Obtiene el objeto [Column](../../com.aspose.cells/column) por la posición en la lista. |
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
### get(int columnIndex) {#get-int-}
```
public Column get(int columnIndex)
```


Obtiene un objeto [Column](../../com.aspose.cells/column) por el índice de columna. El objeto Column del índice de columna dado se instanciará si no existe previamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int |  |

**Returns:**
[Column](../../com.aspose.cells/column)
### getByIndex(int index) {#getByIndex-int-}
```
public Column getByIndex(int index)
```


Obtiene el objeto de columna por el índice.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Columns.GetColumnByIndex(). Esta propiedad será eliminada 12 meses después desde junio de 2010. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnByIndex(int index) {#getColumnByIndex-int-}
```
public Column getColumnByIndex(int index)
```


Obtiene el objeto [Column](../../com.aspose.cells/column) por la posición en la lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición en la lista. |

**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
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

