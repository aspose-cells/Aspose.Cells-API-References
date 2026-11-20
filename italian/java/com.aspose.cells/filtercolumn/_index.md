---
title: "FilterColumn"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un filtro per una singola colonna o una colonna nella tabella."
type: docs
url: /it/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

Rappresenta un filtro per una singola colonna o una colonna nella tabella.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | Ottiene [ColorFilter](../../com.aspose.cells/colorfilter) per filtrare i dati per colore. |
| [getCustomFilters()](#getCustomFilters--) | Ottiene [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) per filtrare i dati per criteri personalizzati. |
| [getDynamicFilter()](#getDynamicFilter--) | Ottiene [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) per filtrare con criteri dinamici. |
| [getFieldIndex()](#getFieldIndex--) | Ottiene l'offset di colonna nell'intervallo. |
| [getFilter()](#getFilter--) | Ottiene la condizione del filtraggio dei dati. |
| [getFilterType()](#getFilterType--) | Ottiene il tipo di filtraggio dei dati. |
| [getFilterValues()](#getFilterValues--) | Ottiene [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) per filtrare i dati per etichette o data/ora. |
| [getIconFilter()](#getIconFilter--) | Ottiene [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) per filtrare i dati per icona. |
| [getMultipleFilters()](#getMultipleFilters--) | Ottiene [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) per filtrare i dati per etichette o data/ora. |
| [getTop10Filter()](#getTop10Filter--) | Ottiene [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) per filtrare i dati in base al rango dei dati. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | Indica se il pulsante AutoFilter per questa colonna è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | Seleziona tutto. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | Ottiene [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) per filtrare i dati per criteri personalizzati. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | Indica se il pulsante AutoFilter per questa colonna è visibile. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Imposta lo spostamento della colonna nell'intervallo. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | Imposta la condizione del filtraggio dei dati. |
| [setFilterType(int value)](#setFilterType-int-) | Imposta il tipo di filtraggio dei dati. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | Ottiene [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) per filtrare i dati per etichette o data/ora. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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


Ottiene [ColorFilter](../../com.aspose.cells/colorfilter) per filtrare i dati per colore.

**Remarks**

Imposta [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) come [FilterType.COLOR\_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER) per primo, altrimenti verrà restituito Null.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


Ottiene [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) per filtrare i dati per criteri personalizzati.

**Remarks**

NOTA: Questo setter di questa proprietà è ora obsoleto. Invece, si prega di utilizzare la proprietà [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) impostandola come [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Questa proprietà sarà rimossa tra 12 mesi a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


Ottiene [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) per filtrare con criteri dinamici.

**Remarks**

Prima di utilizzare questa proprietà, assicurati che [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) sia [FilterType.DYNAMIC\_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER), altrimenti verrà restituito null.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Ottiene l'offset di colonna nell'intervallo.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


Ottiene la condizione del filtraggio dei dati.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà corrispondente secondo [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). E per il tipo di filtro [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), l'oggetto restituito è ora [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) invece di [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Ottiene il tipo di filtraggio dei dati.

Vedi [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

L'oggetto filtro corrispondente verrà creato quando questa proprietà è impostata e la proprietà corrispondente dovrebbe essere usata per ottenere l'oggetto filtro di conseguenza:

| FilterType | Proprietà |
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


Ottiene [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) per filtrare i dati per etichette o data/ora.

**Remarks**

Imposta [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) come [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) per primo, altrimenti verrà restituito Null.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


Ottiene [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) per filtrare i dati per icona.

**Remarks**

Prima di utilizzare questa proprietà, assicurati che [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) sia [FilterType.ICON\_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER), altrimenti verrà restituito null.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


Ottiene [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) per filtrare i dati per etichette o data/ora.

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, utilizza la proprietà FilterColumn.FilterValues. Questa proprietà sarà rimossa tra 12 mesi a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


Ottiene [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) per filtrare i dati in base al rango dei dati.

**Remarks**

Prima di utilizzare questa proprietà, assicurati che [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) sia [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10), altrimenti verrà restituito null.

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


Indica se il pulsante AutoFilter per questa colonna è visibile.

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


Seleziona tutto.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


Ottiene [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) per filtrare i dati per criteri personalizzati.

**Remarks**

NOTA: Questo setter di questa proprietà è ora obsoleto. Invece, si prega di utilizzare la proprietà [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) impostandola come [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Questa proprietà sarà rimossa tra 12 mesi a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


Indica se il pulsante AutoFilter per questa colonna è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Imposta lo spostamento della colonna nell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


Imposta la condizione del filtraggio dei dati.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà corrispondente secondo [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). E per il tipo di filtro [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), l'oggetto restituito è ora [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) invece di [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


Imposta il tipo di filtraggio dei dati.

Vedi [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

L'oggetto filtro corrispondente verrà creato quando questa proprietà è impostata e la proprietà corrispondente dovrebbe essere usata per ottenere l'oggetto filtro di conseguenza:

| FilterType | Proprietà |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


Ottiene [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) per filtrare i dati per etichette o data/ora.

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, utilizza la proprietà FilterColumn.FilterValues. Questa proprietà sarà rimossa tra 12 mesi a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

