---
title: "CustomDocumentPropertyCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Una colección de propiedades de documento personalizadas."
type: docs
url: /es/java/com.aspose.cells/customdocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class CustomDocumentPropertyCollection extends DocumentPropertyCollection
```

Una colección de propiedades de documento personalizadas.

**Remarks**

Cada objeto representa una propiedad personalizada de un documento contenedor.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         CustomDocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Boolean**. |
| [add(String name, DateTime value)](#add-java.lang.String-com.aspose.cells.DateTime-) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.DateTime**. |
| [add(String name, double value)](#add-java.lang.String-double-) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Float**. |
| [add(String name, int value)](#add-java.lang.String-int-) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Number**. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.String**. |
| [addLinkToContent(String name, String source)](#addLinkToContent-java.lang.String-java.lang.String-) | Crea una nueva propiedad de documento personalizada que enlaza con contenido. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [contains(String name)](#contains-java.lang.String-) | Devuelve true si una propiedad con el nombre especificado existe en la colección. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Devuelve un objeto [DocumentProperty](../../com.aspose.cells/documentproperty) por índice. |
| [get(String name)](#get-java.lang.String-) | Devuelve un objeto [DocumentProperty](../../com.aspose.cells/documentproperty) por el nombre de la propiedad. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Obtiene el índice de una propiedad por nombre. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Elimina una propiedad con el nombre especificado de la colección. |
| [removeAt(int index)](#removeAt-int-) | Elimina una propiedad en el índice especificado. |
| [toString()](#toString--) |  |
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--) | Actualiza los valores de todas las propiedades personalizadas que están vinculadas al contenido (utiliza el valor de celda del rango vinculado para actualizar el valor de la propiedad personalizada). |
| [updateLinkedRange()](#updateLinkedRange--) | Actualiza todos los rangos que están vinculados a propiedades personalizadas (utiliza el valor de la propiedad de documento personalizada para actualizar el valor de celda del rango vinculado). |
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
### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public DocumentProperty add(String name, boolean value)
```


Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Boolean**.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| valor | boolean | El valor de la propiedad. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, DateTime value) {#add-java.lang.String-com.aspose.cells.DateTime-}
```
public DocumentProperty add(String name, DateTime value)
```


Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.DateTime**.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| value | [DateTime](../../com.aspose.cells/datetime) | El valor de la propiedad. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public DocumentProperty add(String name, double value)
```


Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Float**.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| valor | double | El valor de la propiedad. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, int value) {#add-java.lang.String-int-}
```
public DocumentProperty add(String name, int value)
```


Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Number**.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| valor | int | El valor de la propiedad. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public DocumentProperty add(String name, String value)
```


Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.String**.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| valor | java.lang.String | El valor de la propiedad. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### addLinkToContent(String name, String source) {#addLinkToContent-java.lang.String-java.lang.String-}
```
public DocumentProperty addLinkToContent(String name, String source)
```


Crea una nueva propiedad de documento personalizada que enlaza con contenido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| origen | java.lang.String | El origen de la propiedad. Debe ser el nombre del rango con nombre. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Devuelve true si una propiedad con el nombre especificado existe en la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas. |

**Returns:**
boolean - True si la propiedad existe en la colección; false de lo contrario.
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
public DocumentProperty get(int index)
```


Devuelve un objeto [DocumentProperty](../../com.aspose.cells/documentproperty) por índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | Índice basado en cero del [DocumentProperty](../../com.aspose.cells/documentproperty) a recuperar. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Devuelve un objeto [DocumentProperty](../../com.aspose.cells/documentproperty) por el nombre de la propiedad.

**Remarks**

Devuelve null si no se encuentra una propiedad con el nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas a recuperar. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Obtiene el índice de una propiedad por nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas. |

**Returns:**
int - El índice basado en cero. Valor negativo si no se encuentra.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Elimina una propiedad con el nombre especificado de la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina una propiedad en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
```
public void updateLinkedPropertyValue()
```


Actualiza los valores de todas las propiedades personalizadas que están vinculadas al contenido (utiliza el valor de celda del rango vinculado para actualizar el valor de la propiedad personalizada).

### updateLinkedRange() {#updateLinkedRange--}
```
public void updateLinkedRange()
```


Actualiza todos los rangos que están vinculados a propiedades personalizadas (utiliza el valor de la propiedad de documento personalizada para actualizar el valor de celda del rango vinculado).

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

