---
title: "GridWorksheetCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

Encapsula una colección de objetos [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
## Métodos

| Método | Descripción |
| --- | --- |
| [add()](#add--) | Agrega una hoja de cálculo a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | Agrega una hoja de cálculo a la colección. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente. |
| [calculateFormula()](#calculateFormula--) | Calcula el resultado de las fórmulas. |
| [clear()](#clear--) | Borra todas las hojas de cálculo. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [GridWorksheet](../../com.aspose.gridweb/gridworksheet) en el índice especificado. |
| [get(String sheetName)](#get-java.lang.String-) | Obtiene el elemento [GridWorksheet](../../com.aspose.gridweb/gridworksheet) con el nombre especificado. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el tamaño del enumerador |
| [getDefaultFontName()](#getDefaultFontName--) | Obtiene el nombre de fuente predeterminado del control. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | Obtiene la colección de todos los objetos Name en la hoja de cálculo. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Obtiene el separador decimal para formatear/analizar valores numéricos. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | Insertar una hoja de cálculo. |
| [iterator()](#iterator--) | Obtiene el enumerador de filas |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en un índice especificado. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Elimina el elemento con un nombre especificado. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Establece el nombre de fuente predeterminado del control. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Establece el separador decimal para formatear/analizar valores numéricos. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | Establece la visibilidad de la hoja. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Intercambia las dos hojas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Agrega una hoja de cálculo a la colección.

**Returns:**
int - índice del objeto [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


Agrega una hoja de cálculo a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | Nombre de la hoja de cálculo |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | Índice de la hoja de cálculo origen. |

**Returns:**
int - índice del objeto [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | Nombre de la hoja de cálculo origen. |

**Returns:**
int - índice del objeto [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcula el resultado de las fórmulas.

### clear() {#clear--}
```
public void clear()
```


Borra todas las hojas de cálculo.

**Remarks**

Un libro de trabajo debe contener una hoja de cálculo.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
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
### get(int index) {#get-int-}
```
public GridWorksheet get(int index)
```


Obtiene el elemento [GridWorksheet](../../com.aspose.gridweb/gridworksheet) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


Obtiene el elemento [GridWorksheet](../../com.aspose.gridweb/gridworksheet) con el nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | El nombre de la hoja de cálculo. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo.

**Remarks**

El índice de la hoja comienza en cero.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el tamaño del enumerador

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Obtiene el nombre de fuente predeterminado del control.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


Obtiene la colección de todos los objetos Name en la hoja de cálculo.

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Obtiene el separador decimal para formatear/analizar valores numéricos. El predeterminado es el separador decimal de la región actual.

**Returns:**
char
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


Insertar una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de la hoja |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene el enumerador de filas

**Returns:**
java.util.Iterator - El enumerador de filas
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el elemento en un índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El valor del índice del elemento a eliminar. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Elimina el elemento con un nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del elemento a eliminar. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo.

**Remarks**

El índice de la hoja comienza en cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Establece el nombre de fuente predeterminado del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Establece el separador decimal para formatear/analizar valores numéricos. El predeterminado es el separador decimal de la región actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


Establece la visibilidad de la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | Nombre de la hoja de cálculo origen. |
| isVisible | boolean | Si la hoja de cálculo es visible |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Intercambia las dos hojas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex1 | int | La primera hoja de cálculo. |
| sheetIndex2 | int | La segunda hoja de cálculo. |

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

