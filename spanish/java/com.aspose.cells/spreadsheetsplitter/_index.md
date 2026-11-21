---
title: "SpreadsheetSplitter"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Divide el archivo de hoja de cálculo en varias partes."
type: docs
url: /es/java/com.aspose.cells/spreadsheetsplitter/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetSplitter
```

Divide el archivo de hoja de cálculo en varias partes.

**Example**

```
         SpreadsheetSplitter.process("template.xlsx", "split.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeSplitOptions options)](#process-com.aspose.cells.LowCodeSplitOptions-) | Divide el archivo de hoja de cálculo en varias partes. |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Divide el archivo de plantilla dado en varias partes. |
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




### process(LowCodeSplitOptions options) {#process-com.aspose.cells.LowCodeSplitOptions-}
```
public static void process(LowCodeSplitOptions options)
```


Divide el archivo de hoja de cálculo en varias partes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [LowCodeSplitOptions](../../com.aspose.cells/lowcodesplitoptions) | Opciones para dividir la hoja de cálculo |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Divide el archivo de plantilla dado en varias partes.

**Remarks**

Los archivos de salida se crearán a partir del archivo resultante especificado añadiendo el número de secuencia de la hoja y la parte dividida. Por ejemplo, si el archivo de salida especificado es Split.xlsx, los archivos generados serán Split\_0\_0.xlsx, Split\_0\_1.xlsx, ..., Split\_1\_0.xlsx, ...

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | java.lang.String | El archivo de plantilla a dividir |
| resultFile | java.lang.String | El archivo resultante (patrón de nombre) |

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

