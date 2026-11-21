---
title: "TextBoxCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/textboxcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TextBoxCollection extends CollectionBase
```

Encapsula una colección de objetos [TextBox](../../com.aspose.cells/textbox).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //get collection object
         TextBoxCollection textBoxCollection = workbook.getWorksheets().get(0).getTextBoxes();
         //add a textbox
         textBoxCollection.add(1, 1, 50, 100);
         for(TextBox tbox : (Iterable<TextBox>) textBoxCollection)
         {
             //do what you want
         }
 
         //do your business
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int topRow, int leftColumn, int height, int width)](#add-int-int-int-int-) | Agrega un cuadro de texto a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Borra todos los cuadros de texto. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [TextBox](../../com.aspose.cells/textbox) en el índice especificado. |
| [get(String name)](#get-java.lang.String-) | Obtiene el elemento [TextBox](../../com.aspose.cells/textbox) por el nombre. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina un cuadro de texto del archivo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int height, int width) {#add-int-int-int-int-}
```
public int add(int topRow, int leftColumn, int height, int width)
```


Agrega un cuadro de texto a la colección.

**Example**

```
         //add a TextBox
         int index2 = textBoxCollection.add(1, 1, 50, 100);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| altura | int | Altura de textbox, en unidad de píxel. |
| ancho | int | Ancho de textbox, en unidad de píxel. |

**Returns:**
int - índice del objeto [TextBox](../../com.aspose.cells/textbox).
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


Borra todos los cuadros de texto.

**Example**

```
         //clear all textbox
         textBoxCollection.clear();
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
public TextBox get(int index)
```


Obtiene el elemento [TextBox](../../com.aspose.cells/textbox) en el índice especificado.

**Example**

```
         int index = textBoxCollection.getCount() - 1;
         TextBox txb = textBoxCollection.get(index);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public TextBox get(String name)
```


Obtiene el elemento [TextBox](../../com.aspose.cells/textbox) por el nombre.

**Example**

```
         String txtboxName = "textbox 1"; 
         TextBox txb2 = textBoxCollection.get(txtboxName);
         if(txb2 != null)
         {
             //do what you want
         }
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del cuadro de texto. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
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


Elimina un cuadro de texto del archivo.

**Example**

```
         int index3 = textBoxCollection.getCount() - 1;
         textBoxCollection.removeAt(index3);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del cuadro de texto. |

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

