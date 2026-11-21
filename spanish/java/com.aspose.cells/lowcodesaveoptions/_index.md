---
title: "LowCodeSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opciones para guardar resultados generados de forma low code."
type: docs
url: /es/java/com.aspose.cells/lowcodesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class LowCodeSaveOptions
```

Opciones para guardar resultados generados de forma low code.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LowCodeSaveOptions()](#LowCodeSaveOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Obtiene el archivo (con ruta si es necesario) para guardar los datos generados. |
| [getOutputStream()](#getOutputStream--) | Obtiene el Stream para escribir los datos generados. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de guardado para la salida. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Establece el archivo (con ruta si es necesario) para guardar los datos generados. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Establece el Stream para escribir los datos generados. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Establece el formato de guardado para la salida. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptions() {#LowCodeSaveOptions--}
```
public LowCodeSaveOptions()
```


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
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


Obtiene el archivo (con ruta si es necesario) para guardar los datos generados. Cuando se establece esta propiedad con un valor distinto de null o cadena vacía, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) será ignorado.

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


Obtiene el Stream para escribir los datos generados. Cuando se establece esta propiedad con un valor distinto de null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) será ignorado.

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtiene el formato de guardado para la salida. Generalmente, para procesos específicos en modo low‑code, solo se permiten algunos formatos específicos. Por favor, especifique el formato correcto para el proceso correspondiente, de lo contrario se pueden producir resultados inesperados o incluso una excepción.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

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




### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


Establece el archivo (con ruta si es necesario) para guardar los datos generados. Cuando se establece esta propiedad con un valor distinto de null o cadena vacía, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) será ignorado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


Establece el Stream para escribir los datos generados. Cuando se establece esta propiedad con un valor distinto de null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) será ignorado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Establece el formato de guardado para la salida. Generalmente, para procesos específicos en modo low‑code, solo se permiten algunos formatos específicos. Por favor, especifique el formato correcto para el proceso correspondiente, de lo contrario se pueden producir resultados inesperados o incluso una excepción.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

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

