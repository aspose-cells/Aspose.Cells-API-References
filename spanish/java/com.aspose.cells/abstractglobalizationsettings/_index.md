---
title: "AbstractGlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración de globalización."
type: docs
url: /es/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

Representa la configuración de globalización.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Compara dos valores de cadena según ciertas reglas de ordenación. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Transforma la cadena en un objeto comparable según ciertas reglas de ordenación. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractGlobalizationSettings() {#AbstractGlobalizationSettings--}
```
public AbstractGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Compara dos valores de cadena según ciertas reglas de ordenación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| v1 | java.lang.String | la primera cadena |
| v2 | java.lang.String | la segunda cadena |
| ignoreCase | boolean | si se ignora mayúsculas y minúsculas al comparar valores |

**Returns:**
int - Entero que indica la relación léxica entre los dos comparandos
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
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Transforma la cadena en un objeto comparable según ciertas reglas de ordenación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| v | java.lang.String | El valor de cadena necesita compararse con otros. |
| ignoreCase | boolean | si se ignora mayúsculas y minúsculas al comparar valores |

**Returns:**
java.lang.Comparable - El objeto puede usarse para comparar o ordenar valores de cadena
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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

