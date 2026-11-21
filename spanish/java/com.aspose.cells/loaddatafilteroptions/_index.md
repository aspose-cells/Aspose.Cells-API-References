---
title: "LoadDataFilterOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones para filtrar datos al cargar el libro de trabajo desde una plantilla."
type: docs
url: /es/java/com.aspose.cells/loaddatafilteroptions/
---

**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```

Representa las opciones para filtrar datos al cargar el libro de trabajo desde una plantilla.
## Campos

| Campo | Descripción |
| --- | --- |
| [ALL](#ALL) | Cargar todo |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | Cargar configuraciones para el libro de trabajo |
| [CELL_BLANK](#CELL-BLANK) | Cargar celdas cuyo valor está vacío |
| [CELL_BOOL](#CELL-BOOL) | Cargar celdas cuyo valor es booleano |
| [CELL_DATA](#CELL-DATA) | Cargar datos de celdas incluyendo valores, fórmulas y formato |
| [CELL_ERROR](#CELL-ERROR) | Cargar celdas cuyo valor es error |
| [CELL_NUMERIC](#CELL-NUMERIC) | Cargar celdas cuyo valor es numérico(incluyendo fecha y hora) |
| [CELL_STRING](#CELL-STRING) | Cargar celdas cuyo valor es cadena |
| [CELL_VALUE](#CELL-VALUE) | Cargar valor de celdas(todos los tipos de valor) solo |
| [CHART](#CHART) | Cargar gráficos |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Cargar formato condicional |
| [DATA_VALIDATION](#DATA-VALIDATION) | Cargar validaciones de datos |
| [DEFINED_NAMES](#DEFINED-NAMES) | Cargar objetos de nombre definido |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | Cargar propiedades del documento |
| [DRAWING](#DRAWING) | Objetos de dibujo(incluyendo Gráfico, Imagen, OleObject y todos los demás objetos de dibujo) |
| [FORMULA](#FORMULA) | Cargar fórmulas de celdas. |
| [HYPERLINKS](#HYPERLINKS) | Cargar hipervínculos |
| [MERGED_AREA](#MERGED-AREA) | Cargar celdas combinadas |
| [NONE](#NONE) | Cargar nada para los datos de la hoja |
| [OLE_OBJECT](#OLE-OBJECT) | Cargar OleObjects |
| [PICTURE](#PICTURE) | Cargar imágenes |
| [PIVOT_TABLE](#PIVOT-TABLE) | Cargar tablas dinámicas |
| [REVISION](#REVISION) | Cargar registros de revisiones |
| [SETTINGS](#SETTINGS) | Cargar configuraciones para el libro y la hoja de cálculo |
| [SHAPE](#SHAPE) | Cargar formas |
| [SHEET_DATA](#SHEET-DATA) | Cargar todos los datos de la hoja de cálculo, como datos de celdas, configuraciones, objetos, ...etc. |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | Cargar configuraciones para la hoja de cálculo |
| [STRUCTURE](#STRUCTURE) | Cargar estructura del libro |
| [STYLE](#STYLE) | Cargar estilos para el formato de celdas |
| [TABLE](#TABLE) | Cargar tablas |
| [VBA](#VBA) | Cargar proyectos VBA |
| [XML_MAP](#XML-MAP) | Cargar XmlMap |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Cargar todo

### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```


Cargar configuraciones para el libro de trabajo

### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```


Cargar celdas cuyo valor está vacío

### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```


Cargar celdas cuyo valor es booleano

### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```


Cargar datos de celdas incluyendo valores, fórmulas y formato

### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```


Cargar celdas cuyo valor es error

### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```


Cargar celdas cuyo valor es numérico(incluyendo fecha y hora)

### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```


Cargar celdas cuyo valor es cadena

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Cargar valor de celdas(todos los tipos de valor) solo

### CHART {#CHART}
```
public static final int CHART
```


Cargar gráficos

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Cargar formato condicional

### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```


Cargar validaciones de datos

### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```


Cargar objetos de nombre definido

### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```


Cargar propiedades del documento

### DRAWING {#DRAWING}
```
public static final int DRAWING
```


Objetos de dibujo(incluyendo Gráfico, Imagen, OleObject y todos los demás objetos de dibujo)

### FORMULA {#FORMULA}
```
public static final int FORMULA
```


Cargar fórmulas de celdas.

**Remarks**

Generalmente los objetos Name definidos (DefinedNames) también deben cargarse al cargar fórmulas porque pueden ser referenciados por fórmulas. Por lo tanto, la opción Formula o CellData debe funcionar con la opción DefinedNames juntas (Formula\\|DefinedNames o CellData\\|DefinedNames) para la mayoría de los escenarios.

### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```


Cargar hipervínculos

### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```


Cargar celdas combinadas

### NONE {#NONE}
```
public static final int NONE
```


Cargar nada para los datos de la hoja

**Remarks**

NOTA: Este miembro está ahora obsoleto y por favor use Structure en su lugar. Esta propiedad será eliminada 12 meses después desde diciembre de 2017. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```


Cargar OleObjects

### PICTURE {#PICTURE}
```
public static final int PICTURE
```


Cargar imágenes

### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```


Cargar tablas dinámicas

### REVISION {#REVISION}
```
public static final int REVISION
```


Cargar registros de revisiones

### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```


Cargar configuraciones para el libro y la hoja de cálculo

### SHAPE {#SHAPE}
```
public static final int SHAPE
```


Cargar formas

**Remarks**

NOTA: Este miembro está ahora obsoleto y por favor use Drawing en su lugar. Esta propiedad será eliminada 12 meses después desde noviembre de 2019. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```


Cargar todos los datos de la hoja de cálculo, como datos de celdas, configuraciones, objetos, ...etc.

### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```


Cargar configuraciones para la hoja de cálculo

### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```


Cargar estructura del libro

### STYLE {#STYLE}
```
public static final int STYLE
```


Cargar estilos para el formato de celdas

### TABLE {#TABLE}
```
public static final int TABLE
```


Cargar tablas

### VBA {#VBA}
```
public static final int VBA
```


Cargar proyectos VBA

### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```


Cargar XmlMap

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

