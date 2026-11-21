---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Implementación para proporcionar opciones de guardado que guardan partes divididas en archivos y la ruta del archivo resultante se nombra, pudiendo contener directorios SheetIndex o SheetName SplitPartIndex."
type: docs
url: /es/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

Implementación para proporcionar opciones de guardado que guardan partes divididas en archivos y la ruta del archivo resultante se nombra como (puede contener directorios): [getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(o SheetName)+[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Libera recursos después de procesar la parte dividida actual. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Si siempre se agrega el índice o nombre de la hoja a la ruta del archivo. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Si siempre se agrega el índice de la parte dividida a la ruta del archivo. |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | Parte de encabezado (antes del contenido añadido de la hoja y la parte dividida) de la ruta del archivo. |
| [getPathTail()](#getPathTail--) | Parte final (después de los números de secuencia) de la ruta del archivo. |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | La plantilla para crear una instancia de opciones de guardado en [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Desplazamiento del índice de la hoja entre el utilizado en la ruta del archivo y su valor real ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetPrefix()](#getSheetPrefix--) | Prefijo para el índice de la hoja de cálculo. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Desfase del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Prefijo para el índice de la parte dividida. |
| [getUseSheetName()](#getUseSheetName--) | Indica si construye la ruta del archivo con el nombre de la hoja en lugar del índice de la hoja. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Si siempre se agrega el índice o nombre de la hoja a la ruta del archivo. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Si siempre se agrega el índice de la parte dividida a la ruta del archivo. |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | Parte de encabezado (antes del contenido añadido de la hoja y la parte dividida) de la ruta del archivo. |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | Parte final (después de los números de secuencia) de la ruta del archivo. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | La plantilla para crear una instancia de opciones de guardado en [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Desplazamiento del índice de la hoja entre el utilizado en la ruta del archivo y su valor real ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | Prefijo para el índice de la hoja de cálculo. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Desfase del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Prefijo para el índice de la parte dividida. |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | Indica si construye la ruta del archivo con el nombre de la hoja en lugar del índice de la hoja. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
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

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


Indica si siempre se agrega el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, es decir, cuando hay solo una hoja, el índice (o nombre) de la hoja y el prefijo correspondiente no se agregarán a la ruta del archivo.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Indica si siempre se agrega el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, es decir, cuando hay solo una parte dividida, el índice de la parte dividida y el prefijo correspondiente no se agregarán a la ruta del archivo.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


Parte de encabezado (antes del contenido añadido de la hoja y la parte dividida) de la ruta del archivo.

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


Parte final (después de los números de secuencia) de la ruta del archivo. Debe incluir la extensión del nombre del archivo.

**Returns:**
java.lang.String
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


La plantilla para crear una instancia de opciones de guardado en [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Si se ha especificado la plantilla, la instancia creada copiará todas sus configuraciones y actualizará el archivo de salida en consecuencia.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Desplazamiento del índice de la hoja entre el utilizado en la ruta del archivo y su valor real ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Solo tiene efecto cuando [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) es false.

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


Prefijo para el índice de la hoja de cálculo.

**Remarks**

Si solo hay una hoja de cálculo y [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) es false, entonces este prefijo y el índice (o nombre) de la hoja no se agregarán a la ruta de archivo resultante.

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


Desfase del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


Prefijo para el índice de la parte dividida.

**Remarks**

Si solo hay una parte dividida y [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) es false, entonces este prefijo y el índice de la parte dividida (0) no se agregarán a la ruta de archivo resultante.

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


Indica si construye la ruta del archivo con el nombre de la hoja en lugar del índice de la hoja. El valor predeterminado es false.

**Remarks**

El nombre de la hoja nunca se volverá a generar automáticamente. Por lo tanto, cuando se establezca en true, asegúrese de que no haya ningún nombre de hoja especial que pueda causar una ruta o nombre de archivo no válido.

**Returns:**
boolean
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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


Indica si siempre se agrega el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, es decir, cuando hay solo una hoja, el índice (o nombre) de la hoja y el prefijo correspondiente no se agregarán a la ruta del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Indica si siempre se agrega el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, es decir, cuando hay solo una parte dividida, el índice de la parte dividida y el prefijo correspondiente no se agregarán a la ruta del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


Parte de encabezado (antes del contenido añadido de la hoja y la parte dividida) de la ruta del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


Parte final (después de los números de secuencia) de la ruta del archivo. Debe incluir la extensión del nombre del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


La plantilla para crear una instancia de opciones de guardado en [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Si se ha especificado la plantilla, la instancia creada copiará todas sus configuraciones y actualizará el archivo de salida en consecuencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


Desplazamiento del índice de la hoja entre el utilizado en la ruta del archivo y su valor real ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Solo tiene efecto cuando [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


Prefijo para el índice de la hoja de cálculo.

**Remarks**

Si solo hay una hoja de cálculo y [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) es false, entonces este prefijo y el índice (o nombre) de la hoja no se agregarán a la ruta de archivo resultante.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


Desfase del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


Prefijo para el índice de la parte dividida.

**Remarks**

Si solo hay una parte dividida y [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) es false, entonces este prefijo y el índice de la parte dividida (0) no se agregarán a la ruta de archivo resultante.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


Indica si construye la ruta del archivo con el nombre de la hoja en lugar del índice de la hoja. El valor predeterminado es false.

**Remarks**

El nombre de la hoja nunca se volverá a generar automáticamente. Por lo tanto, cuando se establezca en true, asegúrese de que no haya ningún nombre de hoja especial que pueda causar una ruta o nombre de archivo no válido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

