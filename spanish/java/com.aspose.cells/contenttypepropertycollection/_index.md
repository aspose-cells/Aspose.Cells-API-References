---
title: "ContentTypePropertyCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Una colección de objetos que representan información adicional."
type: docs
url: /es/java/com.aspose.cells/contenttypepropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ContentTypePropertyCollection extends CollectionBase
```

Una colección de objetos [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) que representan información adicional.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Add a new property.
          workbook.getContentTypeProperties().add("Admin", "Aspose", "text");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Agrega información de la propiedad de tipo de contenido. |
| [add(String name, String value, String type)](#add-java.lang.String-java.lang.String-java.lang.String-) | Agrega información de la propiedad de tipo de contenido. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene la propiedad de tipo de contenido por el índice específico. |
| [get(String name)](#get-java.lang.String-) | Obtiene la propiedad de tipo de contenido por el nombre de la propiedad. |
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
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public int add(String name, String value)
```


Agrega información de la propiedad de tipo de contenido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad de tipo de contenido. |
| valor | java.lang.String | El valor de la propiedad de tipo de contenido. |

**Returns:**
int
### add(String name, String value, String type) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String name, String value, String type)
```


Agrega información de la propiedad de tipo de contenido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad de tipo de contenido. |
| valor | java.lang.String | El valor de la propiedad de tipo de contenido. |
| type | java.lang.String | El tipo de la propiedad de tipo de contenido. |

**Returns:**
int
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
public ContentTypeProperty get(int index)
```


Obtiene la propiedad de tipo de contenido por el índice específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice. |

**Returns:**
[ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) - The content type property
### get(String name) {#get-java.lang.String-}
```
public ContentTypeProperty get(String name)
```


Obtiene la propiedad de tipo de contenido por el nombre de la propiedad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |

**Returns:**
[ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) - The content type property
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

