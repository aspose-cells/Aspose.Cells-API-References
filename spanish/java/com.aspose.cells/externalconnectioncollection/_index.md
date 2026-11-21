---
title: "ExternalConnectionCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica la colección"
type: docs
url: /es/java/com.aspose.cells/externalconnectioncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ExternalConnectionCollection extends CollectionBase
```

Especifica la colección [ExternalConnection](../../com.aspose.cells/externalconnection)

**Example**

```
         Workbook wb = new Workbook("connection.xlsx");
         ExternalConnectionCollection dataConns = wb.getDataConnections();
         ExternalConnection dataConn = null;
         for (int i = 0; i <dataConns.getCount(); i++)
         {
             dataConn = dataConns.get(i);
             //get external connection id
             System.out.println(dataConn.getConnectionId());
         }
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [ExternalConnection](../../com.aspose.cells/externalconnection) en el índice especificado. |
| [get(String connectionName)](#get-java.lang.String-) | Obtiene el elemento [ExternalConnection](../../com.aspose.cells/externalconnection) con el nombre especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [getExternalConnectionById(int connId)](#getExternalConnectionById-int-) | Obtiene el elemento [ExternalConnection](../../com.aspose.cells/externalconnection) con el id especificado. |
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
### get(int index) {#get-int-}
```
public ExternalConnection get(int index)
```


Obtiene el elemento [ExternalConnection](../../com.aspose.cells/externalconnection) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection) - The element at the specified index.
### get(String connectionName) {#get-java.lang.String-}
```
public ExternalConnection get(String connectionName)
```


Obtiene el elemento [ExternalConnection](../../com.aspose.cells/externalconnection) con el nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| connectionName | java.lang.String | el nombre de la conexión de datos |

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection) - The element with the specified name.
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
### getExternalConnectionById(int connId) {#getExternalConnectionById-int-}
```
public ExternalConnection getExternalConnectionById(int connId)
```


Obtiene el elemento [ExternalConnection](../../com.aspose.cells/externalconnection) con el id especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| connId | int | id de conexión externa |

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection) - The element with the specified id.
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

