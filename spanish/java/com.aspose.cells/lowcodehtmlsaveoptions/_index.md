---
title: "LowCodeHtmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opciones para guardar HTML de forma low code."
type: docs
url: /es/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

Opciones para guardar HTML de forma low code.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | Las opciones generales para guardar HTML. |
| [getOutputFile()](#getOutputFile--) | Obtiene el archivo (con ruta si es necesario) para guardar los datos generados. |
| [getOutputStream()](#getOutputStream--) | Obtiene el Stream para escribir los datos generados. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de la hoja de cálculo. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | Las opciones generales para guardar HTML. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Establece el archivo (con ruta si es necesario) para guardar los datos generados. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Establece el Stream para escribir los datos generados. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Establece el formato de la hoja de cálculo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeHtmlSaveOptions() {#LowCodeHtmlSaveOptions--}
```
public LowCodeHtmlSaveOptions()
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
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


Las opciones generales para guardar HTML.

**Remarks**

Cuando se especifica una instancia de [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions), el método [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) será sobrescrito (si se había especificado antes).

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
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


Obtiene el formato de la hoja de cálculo.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Al cambiar esta propiedad, el formato de guardado especificado por [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) será ignorado (si se había especificado antes).

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




### setHtmlOptions(HtmlSaveOptions value) {#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-}
```
public void setHtmlOptions(HtmlSaveOptions value)
```


Las opciones generales para guardar HTML.

**Remarks**

Cuando se especifica una instancia de [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions), el método [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) será sobrescrito (si se había especificado antes).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

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


Establece el formato de la hoja de cálculo.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Al cambiar esta propiedad, el formato de guardado especificado por [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) será ignorado (si se había especificado antes).

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

