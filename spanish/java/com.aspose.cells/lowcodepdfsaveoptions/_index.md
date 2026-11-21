---
title: "LowCodePdfSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opciones para guardar PDF de forma low code."
type: docs
url: /es/java/com.aspose.cells/lowcodepdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodePdfSaveOptions extends LowCodeSaveOptions
```

Opciones para guardar PDF de forma low code.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LowCodePdfSaveOptions()](#LowCodePdfSaveOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Obtiene el archivo (con ruta si es necesario) para guardar los datos generados. |
| [getOutputStream()](#getOutputStream--) | Obtiene el Stream para escribir los datos generados. |
| [getPdfOptions()](#getPdfOptions--) | Las opciones para guardar el archivo Pdf. |
| [getSaveFormat()](#getSaveFormat--) | El formato de guardado para la salida. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Establece el archivo (con ruta si es necesario) para guardar los datos generados. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Establece el Stream para escribir los datos generados. |
| [setPdfOptions(PdfSaveOptions value)](#setPdfOptions-com.aspose.cells.PdfSaveOptions-) | Las opciones para guardar el archivo Pdf. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | El formato de guardado para la salida. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodePdfSaveOptions() {#LowCodePdfSaveOptions--}
```
public LowCodePdfSaveOptions()
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
### getPdfOptions() {#getPdfOptions--}
```
public PdfSaveOptions getPdfOptions()
```


Las opciones para guardar el archivo Pdf.

**Returns:**
[PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions)
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


El formato de guardado para la salida. Para convertir a pdf, solo puede ser [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF).

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

### setPdfOptions(PdfSaveOptions value) {#setPdfOptions-com.aspose.cells.PdfSaveOptions-}
```
public void setPdfOptions(PdfSaveOptions value)
```


Las opciones para guardar el archivo Pdf.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions) |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


El formato de guardado para la salida. Para convertir a pdf, solo puede ser [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF).

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

