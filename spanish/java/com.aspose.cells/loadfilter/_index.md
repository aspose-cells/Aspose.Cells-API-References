---
title: "LoadFilter"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el filtro que proporciona opciones para cargar datos al cargar el libro de trabajo desde una plantilla."
type: docs
url: /es/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

Representa el filtro que proporciona opciones para cargar datos al cargar el libro de trabajo desde una plantilla.

**Remarks**

El usuario puede especificar las opciones de filtro o implementar su propio LoadFilter para especificar cómo cargar los datos.

**Example**

El siguiente ejemplo muestra cómo determinar las opciones de filtro según las propiedades de la hoja de cálculo.

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | Construye un LoadFilter con las opciones de filtro predeterminadas LoadDataFilterOptions.All. |
| [LoadFilter(int opts)](#LoadFilter-int-) | Construye un LoadFilter con las opciones de filtro proporcionadas. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | Las opciones de filtro para indicar qué datos deben cargarse. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | Especifica las hojas (índices) y el orden que se cargarán. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | Las opciones de filtro para indicar qué datos deben cargarse. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Prepara las opciones de filtro antes de cargar la hoja de cálculo dada. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


Construye un LoadFilter con las opciones de filtro predeterminadas LoadDataFilterOptions.All.

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


Construye un LoadFilter con las opciones de filtro proporcionadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). las opciones de filtro predeterminadas |

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
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


Las opciones de filtro para indicar qué datos deben cargarse.

Ver [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


Especifica las hojas (índices) y el orden que se cargarán. El valor predeterminado es null, lo que indica cargar todas las hojas en el orden predeterminado del archivo de plantilla. Si no es null y el índice de alguna hoja no está en la matriz devuelta, entonces esa hoja no se cargará.

**Returns:**
int[]
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




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


Las opciones de filtro para indicar qué datos deben cargarse.

Ver [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


Prepara las opciones de filtro antes de cargar la hoja de cálculo dada. La implementación de LoadFilter del usuario puede cambiar aquí los LoadDataFilterOptions para indicar cómo cargar los datos de esta hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | La hoja de cálculo a cargar. Sólo se pueden usar unas pocas propiedades del objeto de hoja de cálculo dado aquí porque la mayoría de los datos y propiedades no se han cargado. Las propiedades disponibles son: Name, Index, VisibilityType |

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

