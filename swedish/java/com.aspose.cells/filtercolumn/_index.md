---
title: "FilterColumn"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett filter för en enskild kolumn eller en kolumn i tabellen."
type: docs
url: /sv/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

Representerar ett filter för en enskild kolumn eller en kolumn i tabellen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | Hämtar [ColorFilter](../../com.aspose.cells/colorfilter) för att filtrera data efter färg. |
| [getCustomFilters()](#getCustomFilters--) | Hämtar [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) för att filtrera data efter anpassade kriterier. |
| [getDynamicFilter()](#getDynamicFilter--) | Hämtar [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) för att filtrera med dynamiska kriterier. |
| [getFieldIndex()](#getFieldIndex--) | Hämtar kolumnförskjutningen i intervallet. |
| [getFilter()](#getFilter--) | Hämtar villkoret för filtrering av data. |
| [getFilterType()](#getFilterType--) | Hämtar typen för filtrering av data. |
| [getFilterValues()](#getFilterValues--) | Hämtar [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) för att filtrera data efter etiketter eller datum/tid. |
| [getIconFilter()](#getIconFilter--) | Hämtar [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) för att filtrera data efter ikon. |
| [getMultipleFilters()](#getMultipleFilters--) | Hämtar [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) för att filtrera data efter etiketter eller datum/tid. |
| [getTop10Filter()](#getTop10Filter--) | Hämtar [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) för att filtrera data efter rangordning. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | Anger om AutoFilter‑knappen för den här kolumnen är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | Väljer alla. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | Hämtar [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) för att filtrera data efter anpassade kriterier. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | Anger om AutoFilter‑knappen för den här kolumnen är synlig. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Ställer in kolumnförskjutningen i intervallet. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | Ställer in villkoret för filtrering av data. |
| [setFilterType(int value)](#setFilterType-int-) | Ställer in typen för filtrering av data. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | Hämtar [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) för att filtrera data efter etiketter eller datum/tid. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Hämtar [ColorFilter](../../com.aspose.cells/colorfilter) för att filtrera data efter färg.

**Remarks**

Ställer in [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) som [FilterType.COLOR_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER) först, annars returneras Null.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


Hämtar [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) för att filtrera data efter anpassade kriterier.

**Remarks**

OBS: Denna setter för den här egenskapen är nu föråldrad. Använd istället egenskapen [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) genom att sätta den till [FilterType.CUSTOM_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Denna egenskap kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


Hämtar [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) för att filtrera med dynamiska kriterier.

**Remarks**

Innan du använder den här egenskapen, se till att [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) är [FilterType.DYNAMIC_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER), annars returneras null.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Hämtar kolumnförskjutningen i intervallet.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


Hämtar villkoret för filtrering av data.

**Remarks**

OBS: Detta medlem är nu föråldrad. Använd istället motsvarande egenskap enligt [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). Och för filtertypen [FilterType.MULTIPLE_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), är det returnerade objektet nu [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) istället för [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Hämtar typen för filtrering av data.

Se [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

Det motsvarande filterobjektet kommer att skapas när den här egenskapen sätts och motsvarande egenskap bör användas för att hämta filterobjektet på lämpligt sätt:

| FilterType | Egenskap |
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


Hämtar [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) för att filtrera data efter etiketter eller datum/tid.

**Remarks**

Ställer in [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) som [FilterType.MULTIPLE_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) först, annars returneras Null.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


Hämtar [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) för att filtrera data efter ikon.

**Remarks**

Innan du använder den här egenskapen, se till att [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) är [FilterType.ICON_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER), annars returneras null.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


Hämtar [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) för att filtrera data efter etiketter eller datum/tid.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället FilterColumn.FilterValues-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


Hämtar [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) för att filtrera data efter rangordning.

**Remarks**

Innan du använder denna egenskap, se till att [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) är [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10), annars returneras null.

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


Anger om AutoFilter‑knappen för den här kolumnen är synlig.

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


Väljer alla.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


Hämtar [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) för att filtrera data efter anpassade kriterier.

**Remarks**

OBS: Denna setter för den här egenskapen är nu föråldrad. Använd istället egenskapen [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) genom att sätta den till [FilterType.CUSTOM_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Denna egenskap kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


Anger om AutoFilter‑knappen för den här kolumnen är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Ställer in kolumnförskjutningen i intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


Ställer in villkoret för filtrering av data.

**Remarks**

OBS: Detta medlem är nu föråldrad. Använd istället motsvarande egenskap enligt [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). Och för filtertypen [FilterType.MULTIPLE_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), är det returnerade objektet nu [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) istället för [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


Ställer in typen för filtrering av data.

Se [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

Det motsvarande filterobjektet kommer att skapas när den här egenskapen sätts och motsvarande egenskap bör användas för att hämta filterobjektet på lämpligt sätt:

| FilterType | Egenskap |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


Hämtar [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) för att filtrera data efter etiketter eller datum/tid.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället FilterColumn.FilterValues-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

