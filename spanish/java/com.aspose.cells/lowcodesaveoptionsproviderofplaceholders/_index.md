---
title: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Implementación para proporcionar opciones de guardado que guardan partes divididas en archivos y la ruta del archivo resultante se define con marcadores de posición."
type: docs
url: /es/java/com.aspose.cells/lowcodesaveoptionsproviderofplaceholders/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```

Implementación para proporcionar opciones de guardado que guardan partes divididas en archivos y la ruta del archivo resultante se define con marcadores de posición.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | Instancia un objeto para proporcionar opciones de guardado según plantillas especificadas. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Libera recursos después de procesar la parte dividida actual. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Si siempre se agrega el índice o nombre de la hoja a la ruta del archivo. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Si siempre se agrega el índice de la parte dividida a la ruta del archivo. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | La plantilla para crear una instancia de opciones de guardado en [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Desplazamiento del índice de la hoja entre el utilizado en la ruta del archivo y su valor real ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | Prefijo para el índice de la hoja de cálculo. |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | Prefijo para el índice de la hoja de cálculo. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Desfase del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Prefijo para el índice de la parte dividida. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Si siempre se agrega el índice o nombre de la hoja a la ruta del archivo. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Si siempre se agrega el índice de la parte dividida a la ruta del archivo. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | La plantilla para crear una instancia de opciones de guardado en [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Desplazamiento del índice de la hoja entre el utilizado en la ruta del archivo y su valor real ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | Prefijo para el índice de la hoja de cálculo. |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | Prefijo para el índice de la hoja de cálculo. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Desfase del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Prefijo para el índice de la parte dividida. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```


Instancia un objeto para proporcionar opciones de guardado según plantillas especificadas.

**Remarks**

Los marcadores de posición compatibles en la plantilla de ruta de archivo:

 *  $\{SheetIndex\}: will be replaced by the sheet index of the split part
 *  $\{SheetName\}: will be replaced by the sheet name of the split part
 *  $\{SplitPartIndex\}: will be replaced by the index of the split part
 *  $\{SheetIndexPrefix\}: will be replaced by
 *  $\{SheetNamePrefix\}: will be replaced by
 *  $\{SplitPartPrefix\}: will be replaced by

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pathTemplate | java.lang.String | La plantilla de la ruta de archivo resultante. |

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


Indica si siempre se debe agregar el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una hoja, el índice y nombre de la hoja y el prefijo correspondiente ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) no se agregarán a la ruta del archivo.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Indica si siempre se debe agregar el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una parte dividida, el índice de la parte y el prefijo correspondiente ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) no se agregarán a la ruta del archivo.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


La plantilla para crear una instancia de opciones de guardado en [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

Si se ha especificado la plantilla, la instancia creada copiará todas sus configuraciones y actualizará el archivo de salida en consecuencia.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Desplazamiento del índice de la hoja entre el utilizado en la ruta del archivo y su valor real ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```


Prefijo para el índice de la hoja de cálculo.

**Remarks**

Si solo hay una hoja de cálculo y [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) es false, entonces este prefijo y el índice (o nombre) de la hoja no se agregarán a la ruta del archivo resultante.

**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```


Prefijo para el índice de la hoja de cálculo.

**Remarks**

Si solo hay una hoja de cálculo y [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) es false, entonces este prefijo y el índice (o nombre) de la hoja no se agregarán a la ruta del archivo resultante.

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

Si solo hay una parte dividida y [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) es false, entonces este prefijo y el índice de la parte dividida (0) no se agregarán a la ruta del archivo resultante.

**Returns:**
java.lang.String
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


Indica si siempre se debe agregar el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una hoja, el índice y nombre de la hoja y el prefijo correspondiente ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) no se agregarán a la ruta del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Indica si siempre se debe agregar el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una parte dividida, el índice de la parte y el prefijo correspondiente ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) no se agregarán a la ruta del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


La plantilla para crear una instancia de opciones de guardado en [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

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

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```


Prefijo para el índice de la hoja de cálculo.

**Remarks**

Si solo hay una hoja de cálculo y [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) es false, entonces este prefijo y el índice (o nombre) de la hoja no se agregarán a la ruta del archivo resultante.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```


Prefijo para el índice de la hoja de cálculo.

**Remarks**

Si solo hay una hoja de cálculo y [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) es false, entonces este prefijo y el índice (o nombre) de la hoja no se agregarán a la ruta del archivo resultante.

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

Si solo hay una parte dividida y [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) es false, entonces este prefijo y el índice de la parte dividida (0) no se agregarán a la ruta del archivo resultante.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

