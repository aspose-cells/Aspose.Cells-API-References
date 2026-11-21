---
title: "DeleteBlankOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar inställningen för att ta bort tomma celler/rader/kolumner."
type: docs
url: /sv/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

Representerar inställningen för att ta bort tomma celler/rader/kolumner.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | Indikerar om ritningsrelaterade objekt såsom bild, form, diagram... kommer att behandlas som tomma. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | Om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | Indikerar om en cell ska betraktas som tom när dess värde är en tom sträng. |
| [getEndIndex()](#getEndIndex--) | Anger slutrad-/kolumnindex (inklusive) för området som ska kontrolleras och radera tomma rader/kolumner. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | Hämtar övervakaren för att spåra ändringar som orsakas av raderingen. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | Indikerar hur sammanslagna celler ska behandlas när tomma rader/kolumner tas bort. |
| [getStartIndex()](#getStartIndex--) | Anger startrad-/kolumnindex för området som ska kontrolleras och radera tom rad/kolumn. |
| [getUpdateReference()](#getUpdateReference--) | Indikerar om referenser i andra kalkylblad ska uppdateras. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | Indikerar om ritningsrelaterade objekt såsom bild, form, diagram... kommer att behandlas som tomma. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | Om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | Indikerar om en cell ska betraktas som tom när dess värde är en tom sträng. |
| [setEndIndex(int value)](#setEndIndex-int-) | Anger slutrad-/kolumnindex (inklusive) för området som ska kontrolleras och radera tomma rader/kolumner. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | Ställer in övervakaren för att spåra ändringar som orsakas av raderingen. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | Indikerar hur sammanslagna celler ska behandlas när tomma rader/kolumner tas bort. |
| [setStartIndex(int value)](#setStartIndex-int-) | Anger startrad-/kolumnindex för området som ska kontrolleras och radera tom rad/kolumn. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indikerar om referenser i andra kalkylblad ska uppdateras. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
```


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
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


Anger om ritningsrelaterade objekt såsom bild, form, diagram... ska betraktas som tomma. Standardvärdet är true.

**Remarks**

När egenskapen sätts till false kommer alla rader/kolumner som täcks av ritningsobjekt inte att betraktas som tomma och kommer inte att tas bort.

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


Om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. Standardvärdet är false.

**Remarks**

Generellt bör användaren säkerställa att formlerna har beräknats innan raderingsoperationen när denna egenskap är true. Annars kommer alla ny skapade formler via vanliga API:er såsom [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) att betraktas som tomma och kan tas bort eftersom deras beräknade resultat är null innan beräkning.

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


Anger om en cell ska betraktas som tom när dess värde är en tom sträng. Standardvärdet är true.

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


Anger slutrad-/kolumnindex (inklusive) för intervallet som ska kontrolleras och radera tomma rader/kolumner. Standardvärdet är -1 och -1 betyder det maximala intervallet för alla objekt (celler, ritningar, ...) som måste kontrolleras.

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


Hämtar övervakaren för att spåra ändringar som orsakas av raderingen.

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


Indikerar hur sammanslagna celler ska behandlas när tomma rader/kolumner tas bort.

Se [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

För [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY) kommer alla celler i den att betraktas som tomma förutom den icke-tomma övre vänstra cellen. Det är standardvärdet för denna egenskap.

För [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE) kommer alla celler i den att betraktas som icke-tomma.

För [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT) kommer alla celler utanför innehållsvisningsområdet att betraktas som tomma.



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Anger startrad-/kolumnindex för området som ska kontrolleras och radera tom rad/kolumn.

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Indikerar om referenser i andra kalkylblad ska uppdateras.

**Remarks**

Från och med version 26.7 sätter vi standardvärdet för denna egenskap till true.

**Returns:**
boolean
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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


Anger om ritningsrelaterade objekt såsom bild, form, diagram... ska betraktas som tomma. Standardvärdet är true.

**Remarks**

När egenskapen sätts till false kommer alla rader/kolumner som täcks av ritningsobjekt inte att betraktas som tomma och kommer inte att tas bort.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


Om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. Standardvärdet är false.

**Remarks**

Generellt bör användaren säkerställa att formlerna har beräknats innan raderingsoperationen när denna egenskap är true. Annars kommer alla ny skapade formler via vanliga API:er såsom [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) att betraktas som tomma och kan tas bort eftersom deras beräknade resultat är null innan beräkning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


Anger om en cell ska betraktas som tom när dess värde är en tom sträng. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


Anger slutrad-/kolumnindex (inklusive) för intervallet som ska kontrolleras och radera tomma rader/kolumner. Standardvärdet är -1 och -1 betyder det maximala intervallet för alla objekt (celler, ritningar, ...) som måste kontrolleras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


Ställer in övervakaren för att spåra ändringar som orsakas av raderingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


Indikerar hur sammanslagna celler ska behandlas när tomma rader/kolumner tas bort.

Se [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

För [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY) kommer alla celler i den att betraktas som tomma förutom den icke-tomma övre vänstra cellen. Det är standardvärdet för denna egenskap.

För [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE) kommer alla celler i den att betraktas som icke-tomma.

För [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT) kommer alla celler utanför innehållsvisningsområdet att betraktas som tomma.



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


Anger startrad-/kolumnindex för området som ska kontrolleras och radera tom rad/kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Indikerar om referenser i andra kalkylblad ska uppdateras.

**Remarks**

Från och med version 26.7 sätter vi standardvärdet för denna egenskap till true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

