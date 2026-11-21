---
title: "PictureCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/picturecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PictureCollection extends CollectionBase
```

Encapsula una colección de objetos [Picture](../../com.aspose.cells/picture).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get PictureCollection
         PictureCollection pictures = workbook.getWorksheets().get(0).getPictures();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#add-int-int-int-int-java.io.InputStream-) | Añade una imagen a la colección. |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Añade una imagen a la colección. |
| [add(int topRow, int leftColumn, InputStream stream)](#add-int-int-java.io.InputStream-) | Añade una imagen a la colección. |
| [add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#add-int-int-java.io.InputStream-int-int-) | Añade una imagen a la colección. |
| [add(int topRow, int leftColumn, String fileName)](#add-int-int-java.lang.String-) | Añade una imagen a la colección. |
| [add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Añade una imagen a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [camera(int row, int column, String range)](#camera-int-int-java.lang.String-) | Toma una foto del rango. |
| [clear()](#clear--) | Borrar todas las imágenes. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [Picture](../../com.aspose.cells/picture) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Eliminar formas en el índice específico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#add-int-int-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Añade una imagen a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| bottomRow | int | Índice de fila inferior derecha |
| rightColumn | int | Índice de columna inferior derecha |
| stream | java.io.InputStream | Objeto de flujo que contiene los datos de la imagen. |

**Returns:**
int - índice del objeto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)
```


Añade una imagen a la colección.

**Example**

```
         //add a picture
         pictures.add(1, 1, 5, 5, "image.jpg");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| bottomRow | int | Índice de fila inferior derecha |
| rightColumn | int | Índice de columna inferior derecha |
| fileName | java.lang.String | Nombre de archivo de imagen. |

**Returns:**
int - índice del objeto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, InputStream stream) {#add-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, InputStream stream)
```


Añade una imagen a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| stream | java.io.InputStream | Objeto de flujo que contiene los datos de la imagen. |

**Returns:**
int - índice del objeto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#add-int-int-java.io.InputStream-int-int-}
```
public int add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Añade una imagen a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| stream | java.io.InputStream | Objeto de flujo que contiene los datos de la imagen. |
| widthScale | int | Escala del ancho de la imagen, en porcentaje. |
| heightScale | int | Escala de la altura de la imagen, en porcentaje. |

**Returns:**
int - índice del objeto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, String fileName)
```


Añade una imagen a la colección.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| fileName | java.lang.String | Nombre de archivo de imagen. |

**Returns:**
int - índice del objeto [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)
```


Añade una imagen a la colección.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg", 50, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| fileName | java.lang.String | Nombre de archivo de imagen. |
| widthScale | int | Escala del ancho de la imagen, en porcentaje. |
| heightScale | int | Escala de la altura de la imagen, en porcentaje. |

**Returns:**
int - índice del objeto [Picture](../../com.aspose.cells/picture).
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
### camera(int row, int column, String range) {#camera-int-int-java.lang.String-}
```
public int camera(int row, int column, String range)
```


Toma una foto del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | El índice de fila de esta imagen. |
| columna | int | El índice de columna de esta imagen. |
| rango | java.lang.String | El área que requiere fotografía. |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Borrar todas las imágenes.

**Example**

```
         //clear
         pictures.clear();
```

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
public Picture get(int index)
```


Obtiene el elemento [Picture](../../com.aspose.cells/picture) en el índice especificado.

**Example**

```
         //get picture collection
         //PictureCollection pictures = workbook.Worksheets[0].Pictures;
         //add a picture
         int index = pictures.add(1, 1, "image.png");
         //get the picture
         Picture pic = pictures.get(index);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - The element at the specified index.
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


Eliminar formas en el índice específico.

**Example**

```
         //add a picture
         int index2 = pictures.add(1, 1, "image.png");
         //delete
         pictures.removeAt(index2);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

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

