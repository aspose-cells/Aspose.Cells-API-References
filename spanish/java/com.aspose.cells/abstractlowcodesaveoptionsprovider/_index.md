---
title: "AbstractLowCodeSaveOptionsProvider"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Implementación para proporcionar múltiples opciones de guardado para procesos que requieren múltiples salidas."
type: docs
url: /es/java/com.aspose.cells/abstractlowcodesaveoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeSaveOptionsProvider
```

Implementación para proporcionar múltiples opciones de guardado para procesos que requieren múltiples salidas. Por ejemplo, la característica [SpreadsheetSplitter](../../com.aspose.cells/spreadsheetsplitter) requiere varios destinos para guardar los archivos divididos.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider()](#AbstractLowCodeSaveOptionsProvider--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Libera recursos después de procesar la parte dividida actual. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeSaveOptionsProvider() {#AbstractLowCodeSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider()
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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Libera recursos después de procesar la parte dividida actual.

**Remarks**

Por defecto, este método simplemente cierra directamente el flujo especificado por [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) (si las opciones de guardado especificaron un Stream como destino). El usuario puede sobrescribir este método para controlar cómo liberar recursos según sus requisitos y la implementación de [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | las opciones de guardado utilizadas para la parte dividida actual. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public abstract LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual. Devolver null indica omitir la parte dada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
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

