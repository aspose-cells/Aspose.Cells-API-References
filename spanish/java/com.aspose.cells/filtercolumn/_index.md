---
title: "FilterColumn"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un filtro para una sola columna o una columna en la tabla."
type: docs
url: /es/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

Representa un filtro para una sola columna o una columna en la tabla.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | Obtiene [ColorFilter](../../com.aspose.cells/colorfilter) para filtrar datos por color. |
| [getCustomFilters()](#getCustomFilters--) | Obtiene [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) para filtrar datos por criterios personalizados. |
| [getDynamicFilter()](#getDynamicFilter--) | Obtiene [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) para filtrar con criterios dinámicos. |
| [getFieldIndex()](#getFieldIndex--) | Obtiene el desplazamiento de columna en el rango. |
| [getFilter()](#getFilter--) | Obtiene la condición del filtrado de datos. |
| [getFilterType()](#getFilterType--) | Obtiene el tipo del filtrado de datos. |
| [getFilterValues()](#getFilterValues--) | Obtiene [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) para filtrar datos por etiquetas o fecha y hora. |
| [getIconFilter()](#getIconFilter--) | Obtiene [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) para filtrar datos por ícono. |
| [getMultipleFilters()](#getMultipleFilters--) | Obtiene [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) para filtrar datos por etiquetas o fecha y hora. |
| [getTop10Filter()](#getTop10Filter--) | Obtiene [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) para filtrar datos por rango de los datos. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | Indica si el botón AutoFilter para esta columna es visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | Selecciona todo. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | Obtiene [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) para filtrar datos por criterios personalizados. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | Indica si el botón AutoFilter para esta columna es visible. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Establece el desplazamiento de columna en el rango. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | Establece la condición del filtrado de datos. |
| [setFilterType(int value)](#setFilterType-int-) | Establece el tipo del filtrado de datos. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | Obtiene [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) para filtrar datos por etiquetas o fecha y hora. |
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
### getColorFilter() {#getColorFilter--}
```
public ColorFilter getColorFilter()
```


Obtiene [ColorFilter](../../com.aspose.cells/colorfilter) para filtrar datos por color.

**Remarks**

Establece [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) como [FilterType.COLOR\_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER) primero, de lo contrario se devolverá Null.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


Obtiene [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) para filtrar datos por criterios personalizados.

**Remarks**

NOTA: Este setter de esta propiedad está ahora obsoleto. En su lugar, por favor use la propiedad [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) configurándola como [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Esta propiedad será eliminada 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


Obtiene [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) para filtrar con criterios dinámicos.

**Remarks**

Antes de usar esta propiedad, por favor asegúrese de que [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) sea [FilterType.DYNAMIC\_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER), de lo contrario se devolverá null.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Obtiene el desplazamiento de columna en el rango.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


Obtiene la condición del filtrado de datos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad correspondiente según [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). Y para el tipo de filtro [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), el objeto devuelto ahora es [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) en lugar de [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Esta propiedad será eliminada 12 meses después, a partir de octubre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Obtiene el tipo del filtrado de datos.

Ver [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

El objeto de filtro correspondiente se creará cuando se establezca esta propiedad y la propiedad correspondiente debe usarse para obtener el objeto de filtro de manera adecuada:

| FilterType | Propiedad |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Returns:**
int
### getFilterValues() {#getFilterValues--}
```
public FilterValueCollection getFilterValues()
```


Obtiene [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) para filtrar datos por etiquetas o fecha y hora.

**Remarks**

Establece [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) como [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) primero, de lo contrario se devolverá Null.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


Obtiene [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) para filtrar datos por ícono.

**Remarks**

Antes de usar esta propiedad, asegúrese de que [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) sea [FilterType.ICON\_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER), de lo contrario se devolverá null.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


Obtiene [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) para filtrar datos por etiquetas o fecha y hora.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FilterColumn.FilterValues. Esta propiedad será eliminada 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


Obtiene [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) para filtrar datos por rango de los datos.

**Remarks**

Antes de usar esta propiedad, asegúrese de que [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) sea [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10), de lo contrario se devolverá null.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDropdownVisible() {#isDropdownVisible--}
```
public boolean isDropdownVisible()
```


Indica si el botón AutoFilter para esta columna es visible.

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




### selectAll() {#selectAll--}
```
public void selectAll()
```


Selecciona todo.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


Obtiene [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) para filtrar datos por criterios personalizados.

**Remarks**

NOTA: Este setter de esta propiedad está ahora obsoleto. En su lugar, por favor use la propiedad [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) configurándola como [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Esta propiedad será eliminada 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


Indica si el botón AutoFilter para esta columna es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Establece el desplazamiento de columna en el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


Establece la condición del filtrado de datos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad correspondiente según [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). Y para el tipo de filtro [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), el objeto devuelto ahora es [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) en lugar de [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Esta propiedad será eliminada 12 meses después, a partir de octubre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


Establece el tipo del filtrado de datos.

Ver [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

El objeto de filtro correspondiente se creará cuando se establezca esta propiedad y la propiedad correspondiente debe usarse para obtener el objeto de filtro de manera adecuada:

| FilterType | Propiedad |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


Obtiene [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) para filtrar datos por etiquetas o fecha y hora.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FilterColumn.FilterValues. Esta propiedad será eliminada 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) |  |

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

