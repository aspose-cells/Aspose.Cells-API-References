---
title: "ImageConverter"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Convertidor para convertir archivos de plantilla a imágenes."
type: docs
url: /es/java/com.aspose.cells/imageconverter/
---

**Inheritance:**
java.lang.Object
```
public class ImageConverter
```

Convertidor para convertir archivos de plantilla a imágenes.

**Example**

```
         ImageConverter.process("template.xlsx", "res.png");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | Convierte el archivo de plantilla a imágenes |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Convierte el archivo de plantilla a imágenes |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Convierte el archivo de plantilla a imágenes. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```


Convierte el archivo de plantilla a imágenes

**Remarks**

Al convertir a una imagen de formato que admite varias páginas (como tiff), el [LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) o [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) especificado se utilizará directamente para la imagen resultante.

Para otros tipos de imagen, si las opciones de guardado han especificado un Stream como salida, entonces todas las imágenes resultantes se guardarán en el mismo Stream. De lo contrario, los archivos de salida se crearán a partir del archivo de salida especificado en las opciones de guardado añadiendo el número de secuencia de la hoja y la parte dividida. Por ejemplo, si el archivo de salida especificado es Image.png, los archivos de imagen generados serán Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Opciones para entrada y carga |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Opciones para salida y guardado |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)
```


Convierte el archivo de plantilla a imágenes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Opciones para entrada y carga |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Opciones para guardar. Su salida ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) o [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) no tiene efecto porque todas las salidas serán especificadas por el parámetro "provider". |
| provider | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) | Proveedor de opciones de guardado para guardar las imágenes generadas |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Convierte el archivo de plantilla a imágenes.

**Remarks**

Los archivos de salida se crearán a partir del archivo de resultado especificado añadiendo el número de secuencia de la hoja y la parte dividida. Por ejemplo, si el archivo de salida especificado es Image.png, los archivos de imagen generados serán Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | java.lang.String | El archivo de plantilla que se convertirá a imágenes. |
| resultFile | java.lang.String | El archivo resultante (patrón de nombre) para las imágenes generadas. |

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

