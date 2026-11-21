---
title: "Namn"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett definierat namn för ett cellområde."
type: docs
url: /sv/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

Representerar ett definierat namn för ett cellområde.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Hämtar kommentaren för namnet. |
| [getFullText()](#getFullText--) | Hämtar hela namntexten för objektet med omfångsinställningen. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | Hämtar en R1C1-referens för [Name](../../com.aspose.cells/name). |
| [getRange()](#getRange--) | Hämtar intervallet om detta namn refererar till ett intervall. |
| [getRange(boolean recalculate)](#getRange-boolean-) | Hämtar intervallet om detta namn refererar till ett intervall |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | Hämtar intervallet om detta namn refererar till ett intervall. |
| [getRanges()](#getRanges--) | Hämtar alla intervall som detta namn refererar till. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | Hämtar alla intervall som detta namn refererar till. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | Hämtar alla referenser som detta namn refererar till. |
| [getRefersTo()](#getRefersTo--) | Returnerar eller anger formeln som namnet är definierat att referera till, inledningsvis med ett lika-tecken. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | Hämta referensen för detta namn. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | Hämta referensen för detta namn baserat på angiven cell. |
| [getSheetIndex()](#getSheetIndex--) | Indikerar att detta namn tillhör Arbetsbok eller Arbetsblad. 0 = Globalt namn, annars index till blad (en-baserat). |
| [getText()](#getText--) | Hämtar namntexten för objektet. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indikerar om detta namn refereras av andra formler. |
| [isVisible()](#isVisible--) | Indikerar om namnet är synligt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | Anger kommentaren för namnet. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | Ställer in en R1C1-referens för [Name](../../com.aspose.cells/name). |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | Returnerar eller anger formeln som namnet är definierat att referera till, inledningsvis med ett lika-tecken. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | Ställ in referensen för detta namn. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Indikerar att detta namn tillhör Arbetsbok eller Arbetsblad. 0 = Globalt namn, annars index till blad (en-baserat). |
| [setText(String value)](#setText-java.lang.String-) | Hämtar namntexten för objektet. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indikerar om namnet är synligt. |
| [toString()](#toString--) | Returnerar en sträng som representerar det aktuella Range-objektet. |
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
### getComment() {#getComment--}
```
public String getComment()
```


Hämtar kommentaren för namnet. Gäller endast för Excel 2007 eller senare versioner.

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


Hämtar hela namntexten för objektet med omfångsinställningen.

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


Hämtar en R1C1-referens för [Name](../../com.aspose.cells/name).

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Hämtar intervallet om detta namn refererar till ett intervall.

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


Hämtar intervallet om detta namn refererar till ett intervall

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omberäkna | boolean | om den ska omberäknas om detta namn redan har beräknats före detta anrop. |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


Hämtar intervallet om detta namn refererar till ett intervall. Om referensen för detta namn inte är absolut kan intervallet vara olika för olika celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Det motsvarande bladindexet. |
| rad | int | Det motsvarande radindexet. |
| kolumn | int | Det motsvarande kolumnindexet |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Hämtar alla intervall som detta namn refererar till.

**Returns:**
com.aspose.cells.Range[] - Alla intervall.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


Hämtar alla intervall som detta namn refererar till.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omberäkna | boolean | om den ska omberäknas om detta namn redan har beräknats före detta anrop. |

**Returns:**
com.aspose.cells.Range[] - Alla intervall.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


Hämtar alla referenser som detta namn refererar till.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omberäkna | boolean | om den ska omberäknas om detta namn redan har beräknats före detta anrop. |

**Returns:**
com.aspose.cells.ReferredArea[] - Alla intervall.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Returnerar eller anger formeln som namnet är definierat att referera till, inledningsvis med ett lika-tecken.

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


Hämta referensen för detta namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om referensen behöver formateras som R1C1. |
| isLocal | boolean | Om referensen behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


Hämta referensen för detta namn baserat på angiven cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om referensen behöver formateras som R1C1. |
| isLocal | boolean | Om referensen behöver formateras enligt lokala inställningar. |
| rad | int | Radindex för cellen. |
| kolumn | int | Kolumnindex för cellen. |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Indikerar att detta namn tillhör Arbetsbok eller Arbetsblad. 0 = Globalt namn, annars index till blad (en-baserat).

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Hämtar namntexten för objektet.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Indikerar om detta namn refereras av andra formler.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indikerar om namnet är synligt.

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




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Ställer in kommentaren för namnet. Gäller endast för Excel 2007 eller senare versioner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


Ställer in en R1C1-referens för [Name](../../com.aspose.cells/name).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


Returnerar eller anger formeln som namnet är definierat att referera till, inledningsvis med ett lika-tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


Ställ in referensen för detta namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| refersTo | java.lang.String | Referensen. |
| isR1C1 | boolean | Om referensen är i R1C1-format. |
| isLocal | boolean | Om referensen är formaterad enligt lokala inställningar. |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


Indikerar att detta namn tillhör Arbetsbok eller Arbetsblad. 0 = Globalt namn, annars index till blad (en-baserat).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Hämtar namntexten för objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indikerar om namnet är synligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar det aktuella Range-objektet.

**Returns:**
java.lang.String -
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

