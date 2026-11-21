---
title: "LowCodeImageSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opciones para guardar imagen de forma low code."
type: docs
url: /es/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

Opciones para guardar imagen de forma low code.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | Las opciones para renderizar imágenes. |
| [getOutputFile()](#getOutputFile--) | Obtiene el archivo (con ruta si es necesario) para guardar los datos generados. |
| [getOutputStream()](#getOutputStream--) | Obtiene el Stream para escribir los datos generados. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de guardado. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | Proveedor de opciones de guardado para guardar imágenes generadas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | Las opciones para renderizar imágenes. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Establece el archivo (con ruta si es necesario) para guardar los datos generados. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Establece el Stream para escribir los datos generados. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Establece el formato de guardado. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Proveedor de opciones de guardado para guardar imágenes generadas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeImageSaveOptions() {#LowCodeImageSaveOptions--}
```
public LowCodeImageSaveOptions()
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Las opciones para renderizar imágenes.

**Remarks**

Cuando se especifica una instancia de [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions), el [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) será sobrescrito (si se había especificado antes).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
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


Obtiene el formato de guardado.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Si se ha especificado [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--), al establecer esta propiedad también se modificará el valor de [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--).

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


Proveedor de opciones de guardado para guardar imágenes generadas.

**Remarks**

La salida([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) o [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) especificada por esta instancia no tendrá efecto cuando se establezca esta propiedad. En su lugar, la salida de cada imagen generada será especificada por el proveedor.

**Returns:**
[AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
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




### setImageOptions(ImageOrPrintOptions value) {#setImageOptions-com.aspose.cells.ImageOrPrintOptions-}
```
public void setImageOptions(ImageOrPrintOptions value)
```


Las opciones para renderizar imágenes.

**Remarks**

Cuando se especifica una instancia de [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions), el [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) será sobrescrito (si se había especificado antes).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

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


Establece el formato de guardado.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Si se ha especificado [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--), al establecer esta propiedad también se modificará el valor de [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


Proveedor de opciones de guardado para guardar imágenes generadas.

**Remarks**

La salida([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) o [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) especificada por esta instancia no tendrá efecto cuando se establezca esta propiedad. En su lugar, la salida de cada imagen generada será especificada por el proveedor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) |  |

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

