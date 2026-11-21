---
title: "DefaultStyleSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Configuración de los valores predeterminados de las propiedades de estilo de los libros de trabajo."
type: docs
url: /es/java/com.aspose.cells/defaultstylesettings/
---

**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```

Configuraciones para los valores predeterminados de las propiedades de estilo del libro de trabajo.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | Indica si la propiedad de formato numérico es preferible cuando el estilo define tanto un número incorporado como un patrón personalizado. |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | Obtiene el nombre de fuente predeterminado para el libro de trabajo |
| [getFontSize()](#getFontSize--) | Obtiene el tamaño de fuente estándar predeterminado para el libro de trabajo. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Obtiene el valor predeterminado para la alineación horizontal |
| [getVerticalAlignment()](#getVerticalAlignment--) | Obtiene el valor predeterminado para la alineación vertical |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | Indica si la propiedad de formato numérico es preferible cuando el estilo define tanto un número incorporado como un patrón personalizado. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Establece el nombre de fuente predeterminado para el libro de trabajo |
| [setFontSize(double value)](#setFontSize-double-) | Establece el tamaño de fuente estándar predeterminado para el libro de trabajo. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Establece el valor predeterminado para la alineación horizontal |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Establece el valor predeterminado para la alineación vertical |
| [toString()](#toString--) |  |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```


Indica si la propiedad de formato numérico es preferible cuando el estilo define tanto un número incorporado como un patrón personalizado. El valor predeterminado es false, lo que significa que, por defecto, se utilizará el patrón personalizado para formatear los valores siempre que no esté vacío para un estilo.

**Remarks**

Al cargar un libro de trabajo desde un archivo de plantilla existente, puede que tanto el número incorporado como el patrón personalizado estén definidos para un estilo. Esta propiedad determina si debemos usar el número incorporado o el patrón personalizado al formatear los valores con el estilo.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```


Obtiene el nombre de fuente predeterminado para el libro de trabajo

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Obtiene el tamaño de fuente estándar predeterminado para el libro de trabajo.

**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Obtiene el valor predeterminado para la alineación horizontal

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Obtiene el valor predeterminado para la alineación vertical

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
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




### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```


Indica si la propiedad de formato numérico es preferible cuando el estilo define tanto un número incorporado como un patrón personalizado. El valor predeterminado es false, lo que significa que, por defecto, se utilizará el patrón personalizado para formatear los valores siempre que no esté vacío para un estilo.

**Remarks**

Al cargar un libro de trabajo desde un archivo de plantilla existente, puede que tanto el número incorporado como el patrón personalizado estén definidos para un estilo. Esta propiedad determina si debemos usar el número incorporado o el patrón personalizado al formatear los valores con el estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Establece el nombre de fuente predeterminado para el libro de trabajo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```


Establece el tamaño de fuente estándar predeterminado para el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Establece el valor predeterminado para la alineación horizontal

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Establece el valor predeterminado para la alineación vertical

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

