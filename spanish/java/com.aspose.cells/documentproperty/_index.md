---
title: "DocumentProperty"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una propiedad de documento personalizada o incorporada."
type: docs
url: /es/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

Representa una propiedad de documento personalizada o incorporada.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         DocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
 
         //Accessng a custom document property by using the property index
         DocumentProperty customProperty1 = customProperties.get(3);
 
         //Accessng a custom document property by using the property name
         DocumentProperty customProperty2 = customProperties.get("Owner");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Devuelve el nombre de la propiedad. |
| [getSource()](#getSource--) | La fuente de contenido vinculada. |
| [getType()](#getType--) | Obtiene el tipo de datos de la propiedad. |
| [getValue()](#getValue--) | Obtiene el valor de la propiedad. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | Devuelve true si esta propiedad no tiene un nombre en el almacenamiento OLE2 y se generó un nombre único solo para la API pública. |
| [isLinkedToContent()](#isLinkedToContent--) | Indica si esta propiedad está vinculada al contenido |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | Establece el valor de la propiedad. |
| [toBool()](#toBool--) | Devuelve el valor de la propiedad como bool. |
| [toDateTime()](#toDateTime--) | Devuelve el valor de la propiedad como DateTime en la zona horaria local. |
| [toDouble()](#toDouble--) | Devuelve el valor de la propiedad como double. |
| [toInt()](#toInt--) | Devuelve el valor de la propiedad como integer. |
| [toString()](#toString--) | Devuelve el valor de la propiedad como una cadena. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Devuelve el nombre de la propiedad.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


La fuente de contenido vinculada.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de datos de la propiedad.

Ver [PropertyType](../../com.aspose.cells/propertytype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene el valor de la propiedad.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGeneratedName() {#isGeneratedName--}
```
public boolean isGeneratedName()
```


Devuelve true si esta propiedad no tiene un nombre en el almacenamiento OLE2 y se generó un nombre único solo para la API pública.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


Indica si esta propiedad está vinculada al contenido

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Establece el valor de la propiedad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


Devuelve el valor de la propiedad como bool.

**Remarks**

Lanza una excepción si el tipo de propiedad no es PropertyType.Boolean.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


Devuelve el valor de la propiedad como DateTime en la zona horaria local.

**Remarks**

Lanza una excepción si el tipo de propiedad no es PropertyType.Date.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


Devuelve el valor de la propiedad como double.

**Remarks**

Lanza una excepción si el tipo de propiedad no es PropertyType.Float.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


Devuelve el valor de la propiedad como integer.

**Remarks**

Lanza una excepción si el tipo de propiedad no es PropertyType.Number.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


Devuelve el valor de la propiedad como una cadena.

**Remarks**

Convierte una propiedad numérica usando Object.ToString(). Convierte una propiedad booleana en "Y" o "N". Convierte una propiedad de fecha en una cadena de fecha corta.

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

