---
title: "GridValidationCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

Inkapslar en samling av [GridValidation](../../com.aspose.gridweb/gridvalidation) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add()](#add--) | Lägg till en [GridValidation](../../com.aspose.gridweb/gridvalidation) i samlingen. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | Lägger till en datavalidering i samlingen. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | Lägg till en [GridValidation](../../com.aspose.gridweb/gridvalidation) i samlingen. |
| [add(int row, int column)](#add-int-int-) | Lägg till en [GridValidation](../../com.aspose.gridweb/gridvalidation) i samlingen. Valideringen tillämpas på den specificerade cellen. |
| [add(String cellname)](#add-java.lang.String-) | Lägg till en [GridValidation](../../com.aspose.gridweb/gridvalidation) i samlingen. Valideringen tillämpas på den specificerade cellen. |
| [clear()](#clear--) | Rensar alla valideringar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [GridValidation](../../com.aspose.gridweb/gridvalidation)-elementet på det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar storleken på enumeratorn |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Hämtar valideringen som tillämpas på den angivna cellen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Ta bort valideringen på det angivna indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


Lägg till en [GridValidation](../../com.aspose.gridweb/gridvalidation) i samlingen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden GridValidationCollection.Add(row,col). Denna egenskap kommer att tas bort 12 månader senare sedan JANUARY 2015. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


Lägger till en datavalidering i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Området innehåller denna validering. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


Lägg till en [GridValidation](../../com.aspose.gridweb/gridvalidation) i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | Ett valideringsobjekt. |

**Returns:**
int - [GridValidation](../../com.aspose.gridweb/gridvalidation) objektindex.
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


Lägg till en [GridValidation](../../com.aspose.gridweb/gridvalidation) i samlingen. Valideringen tillämpas på den specificerade cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


Lägg till en [GridValidation](../../com.aspose.gridweb/gridvalidation) i samlingen. Valideringen tillämpas på den specificerade cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellname | java.lang.String | namnet på cellen. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


Rensar alla valideringar.

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
### get(int index) {#get-int-}
```
public GridValidation get(int index)
```


Hämtar [GridValidation](../../com.aspose.gridweb/gridvalidation)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
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


Hämtar storleken på enumeratorn

**Returns:**
int
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


Hämtar valideringen som tillämpas på den angivna cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Ta bort valideringen på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

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

