---
title: "VbaModuleCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la lista de"
type: docs
url: /es/java/com.aspose.cells/vbamodulecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaModuleCollection extends CollectionBase
```

Representa la lista de [VbaModule](../../com.aspose.cells/vbamodule)

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject(); 
         // Add a new module.
         vbaProject.getModules().add(VbaModuleType.CLASS, "test");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Worksheet sheet)](#add-com.aspose.cells.Worksheet-) | Agrega módulo para una hoja de cálculo. |
| [add(int type, String name)](#add-int-java.lang.String-) | Agrega módulo. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [addDesignerStorage(String name, byte[] data)](#addDesignerStorage-java.lang.String-byte---) |  |
| [addUserForm(String name, String codes, byte[] designerStorage)](#addUserForm-java.lang.String-java.lang.String-byte---) | Inserta formulario de usuario en el proyecto VBA. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene [VbaModule](../../com.aspose.cells/vbamodule) en la lista por el índice. |
| [get(String name)](#get-java.lang.String-) | Obtiene [VbaModule](../../com.aspose.cells/vbamodule) en la lista por el nombre. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [getDesignerStorage(String name)](#getDesignerStorage-java.lang.String-) | Representa los datos del Diseñador. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Worksheet sheet)](#remove-com.aspose.cells.Worksheet-) | Elimina módulo de una hoja de cálculo. |
| [remove(String name)](#remove-java.lang.String-) | Elimina el módulo por el nombre |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Worksheet sheet) {#add-com.aspose.cells.Worksheet-}
```
public int add(Worksheet sheet)
```


Agrega módulo para una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | La hoja de cálculo |

**Returns:**
int -
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


Agrega módulo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [VbaModuleType](../../com.aspose.cells/vbamoduletype). El tipo de módulo. |
| name | java.lang.String | El nombre del módulo. |

**Returns:**
int -
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
### addDesignerStorage(String name, byte[] data) {#addDesignerStorage-java.lang.String-byte---}
```
public void addDesignerStorage(String name, byte[] data)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |
| datos | byte[] |  |

### addUserForm(String name, String codes, byte[] designerStorage) {#addUserForm-java.lang.String-java.lang.String-byte---}
```
public int addUserForm(String name, String codes, byte[] designerStorage)
```


Inserta formulario de usuario en el proyecto VBA.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del formulario de usuario |
| códigos | java.lang.String | Los códigos del formulario de usuario |
| designerStorage | byte[] | la configuración del diseñador sobre el formulario de usuario |

**Returns:**
int -
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
public VbaModule get(int index)
```


Obtiene [VbaModule](../../com.aspose.cells/vbamodule) en la lista por el índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
### get(String name) {#get-java.lang.String-}
```
public VbaModule get(String name)
```


Obtiene [VbaModule](../../com.aspose.cells/vbamodule) en la lista por el nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del módulo. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
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
### getDesignerStorage(String name) {#getDesignerStorage-java.lang.String-}
```
public byte[] getDesignerStorage(String name)
```


Representa los datos del Diseñador.

**Remarks**

No admitimos analizarlo. Solo para copiar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
byte[]
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




### remove(Worksheet sheet) {#remove-com.aspose.cells.Worksheet-}
```
public void remove(Worksheet sheet)
```


Elimina módulo de una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | La hoja de cálculo |

### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Elimina el módulo por el nombre

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |

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

