---
title: "AbstractLowCodeLoadOptionsProvider"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Implementación para proporcionar múltiples opciones de carga para procesos que utilizan múltiples entradas, como archivos de plantilla."
type: docs
url: /es/java/com.aspose.cells/abstractlowcodeloadoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```

Implementación para proporcionar múltiples opciones de carga para procesos que utilizan múltiples entradas (como archivos de plantilla).

**Remarks**

Por ejemplo, la característica [SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) requiere varios archivos de plantilla para combinar.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | Libera recursos después de procesar la parte actual de la entrada. |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | Obtiene las opciones de carga desde las que cargar los datos de la parte procesada actualmente. |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | Comprueba si hay más entrada. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeLoadOptionsProvider() {#AbstractLowCodeLoadOptionsProvider--}
```
public AbstractLowCodeLoadOptionsProvider()
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
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```


Libera recursos después de procesar la parte actual de la entrada.

**Remarks**

Por defecto, este método simplemente cierra el flujo especificado por el [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) directamente (si las opciones de carga especificaron un Stream como origen). El usuario puede sobrescribir este método para controlar cómo liberar los recursos según sus requisitos y la implementación de [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | las opciones de carga utilizadas para la parte dividida actualmente. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrent() {#getCurrent--}
```
public abstract LowCodeLoadOptions getCurrent()
```


Obtiene las opciones de carga desde las que cargar los datos de la parte procesada actualmente.

**Returns:**
[LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### moveNext() {#moveNext--}
```
public abstract boolean moveNext()
```


Comprueba si hay más entrada.

**Returns:**
boolean
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

