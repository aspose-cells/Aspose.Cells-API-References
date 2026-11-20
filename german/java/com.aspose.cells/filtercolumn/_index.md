---
title: "FilterColumn"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen Filter für eine einzelne Spalte oder eine Spalte in der Tabelle dar."
type: docs
url: /de/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

Stellt einen Filter für eine einzelne Spalte oder eine Spalte in der Tabelle dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | Ruft [ColorFilter](../../com.aspose.cells/colorfilter) zum Filtern von Daten nach Farbe ab. |
| [getCustomFilters()](#getCustomFilters--) | Ruft [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) zum Filtern von Daten nach benutzerdefinierten Kriterien ab. |
| [getDynamicFilter()](#getDynamicFilter--) | Ruft [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) zum Filtern mit dynamischen Kriterien ab. |
| [getFieldIndex()](#getFieldIndex--) | Ruft den Spaltenversatz im Bereich ab. |
| [getFilter()](#getFilter--) | Ruft die Bedingung für das Filtern von Daten ab. |
| [getFilterType()](#getFilterType--) | Ruft den Typ für das Filtern von Daten ab. |
| [getFilterValues()](#getFilterValues--) | Ruft [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) zum Filtern von Daten nach Beschriftungen oder Datum/Uhrzeit ab. |
| [getIconFilter()](#getIconFilter--) | Ruft [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) zum Filtern von Daten nach Symbol ab. |
| [getMultipleFilters()](#getMultipleFilters--) | Ruft [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) zum Filtern von Daten nach Beschriftungen oder Datum/Uhrzeit ab. |
| [getTop10Filter()](#getTop10Filter--) | Ruft [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) zum Filtern von Daten nach Rang ab. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | Wählt alles aus. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | Ruft [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) zum Filtern von Daten nach benutzerdefinierten Kriterien ab. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Legt den Spaltenversatz im Bereich fest. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | Setzt die Bedingung für das Filtern von Daten. |
| [setFilterType(int value)](#setFilterType-int-) | Legt den Typ der Datenfilterung fest. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | Ruft [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) zum Filtern von Daten nach Beschriftungen oder Datum/Uhrzeit ab. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Ruft [ColorFilter](../../com.aspose.cells/colorfilter) zum Filtern von Daten nach Farbe ab.

**Remarks**

Setzt [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) zuerst als [FilterType.COLOR\_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER), andernfalls wird Null zurückgegeben.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


Ruft [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) zum Filtern von Daten nach benutzerdefinierten Kriterien ab.

**Remarks**

HINWEIS: Dieser Setter dieser Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) und setzen sie auf [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


Ruft [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) zum Filtern mit dynamischen Kriterien ab.

**Remarks**

Bevor Sie diese Eigenschaft verwenden, stellen Sie bitte sicher, dass [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) [FilterType.DYNAMIC\_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER) ist, andernfalls wird null zurückgegeben.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Ruft den Spaltenversatz im Bereich ab.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


Ruft die Bedingung für das Filtern von Daten ab.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen bitte die entsprechende Eigenschaft gemäß [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). Und für den Filtertyp [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) ist das zurückgegebene Objekt jetzt [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) anstelle von [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Diese Eigenschaft wird 12 Monate später, seit Oktober 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Ruft den Typ für das Filtern von Daten ab.

Siehe [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

Das entsprechende Filterobjekt wird erstellt, wenn diese Eigenschaft gesetzt wird, und die entsprechende Eigenschaft sollte verwendet werden, um das Filterobjekt entsprechend abzurufen:

| FilterType | Property |
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


Ruft [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) zum Filtern von Daten nach Beschriftungen oder Datum/Uhrzeit ab.

**Remarks**

Setzt [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) zuerst als [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS), andernfalls wird Null zurückgegeben.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


Ruft [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) zum Filtern von Daten nach Symbol ab.

**Remarks**

Bevor Sie diese Eigenschaft verwenden, stellen Sie bitte sicher, dass [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) [FilterType.ICON\_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER) ist, andernfalls wird null zurückgegeben.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


Ruft [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) zum Filtern von Daten nach Beschriftungen oder Datum/Uhrzeit ab.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen bitte die Eigenschaft FilterColumn.FilterValues. Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


Ruft [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) zum Filtern von Daten nach Rang ab.

**Remarks**

Bevor Sie diese Eigenschaft verwenden, stellen Sie bitte sicher, dass [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10) ist, sonst wird null zurückgegeben.

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


Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist.

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


Wählt alles aus.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


Ruft [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) zum Filtern von Daten nach benutzerdefinierten Kriterien ab.

**Remarks**

HINWEIS: Dieser Setter dieser Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) und setzen sie auf [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Legt den Spaltenversatz im Bereich fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


Setzt die Bedingung für das Filtern von Daten.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen bitte die entsprechende Eigenschaft gemäß [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). Und für den Filtertyp [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) ist das zurückgegebene Objekt jetzt [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) anstelle von [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). Diese Eigenschaft wird 12 Monate später, seit Oktober 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


Legt den Typ der Datenfilterung fest.

Siehe [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

Das entsprechende Filterobjekt wird erstellt, wenn diese Eigenschaft gesetzt wird, und die entsprechende Eigenschaft sollte verwendet werden, um das Filterobjekt entsprechend abzurufen:

| FilterType | Property |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


Ruft [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) zum Filtern von Daten nach Beschriftungen oder Datum/Uhrzeit ab.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen bitte die Eigenschaft FilterColumn.FilterValues. Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

