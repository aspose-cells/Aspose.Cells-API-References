---
title: "Unit"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una medida de longitud"
type: docs
url: /es/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

Representa una medida de longitud
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Unit()](#Unit--) | el constructor predeterminado |
| [Unit(double value, int type)](#Unit-double-int-) | Inicializa una nueva instancia de la estructura Unit con el número de punto flotante de doble precisión especificado y UnitType. |
| [Unit(double value)](#Unit-double-) | Inicializa una nueva instancia de la estructura Unit con el número de punto flotante de doble precisión especificado. |
| [Unit(int value)](#Unit-int-) | Inicializa una nueva instancia de la estructura Unit con el entero con signo de 32 bits especificado. |
| [Unit(String value)](#Unit-java.lang.String-) | Inicializa una nueva instancia de la estructura Unit con la longitud especificada. |
## Métodos

| Método | Descripción |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | obtener cadena por el tipo, puede obtener "px" "pt" "%" y similares; |
| [Parse(String s)](#Parse-java.lang.String-) | Convierte la cadena especificada a una Unit. |
| [Percentage(double n)](#Percentage-double-) | Crea una Unit de tipo Percentage a partir del número de punto flotante de doble precisión especificado. |
| [Pixel(int n)](#Pixel-int-) | Crea una Unit de tipo Pixel a partir del entero con signo de 32 bits especificado. |
| [Point(int n)](#Point-int-) | Crea una Unit de tipo Point a partir del entero con signo de 32 bits especificado. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Obtiene el tipo de unidad de la Unit. |
| [getValue()](#getValue--) | Obtiene la longitud de la Unit. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Obtiene un valor que indica si la Unit está vacía. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | obtener la representación en cadena de la unidad. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


el constructor predeterminado

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


Inicializa una nueva instancia de la estructura Unit con el número de punto flotante de doble precisión especificado y UnitType.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |
| type | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


Inicializa una nueva instancia de la estructura Unit con el número de punto flotante de doble precisión especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


Inicializa una nueva instancia de la estructura Unit con el entero con signo de 32 bits especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


Inicializa una nueva instancia de la estructura Unit con la longitud especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


obtener cadena por el tipo, puede obtener "px" "pt" "%" y similares;

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


Convierte la cadena especificada a una Unit.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


Crea una Unit de tipo Percentage a partir del número de punto flotante de doble precisión especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


Crea una Unit de tipo Pixel a partir del entero con signo de 32 bits especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


Crea una Unit de tipo Point a partir del entero con signo de 32 bits especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de unidad de la Unit.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


Obtiene la longitud de la Unit.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Obtiene un valor que indica si la Unit está vacía.

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```


obtener la representación en cadena de la unidad.

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

