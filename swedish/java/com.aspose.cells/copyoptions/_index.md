---
title: "CopyOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar kopieringsalternativen."
type: docs
url: /sv/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

Representerar kopieringsalternativen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | CopyOptions konstruktör. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Indikerar om kolumnbredden kopieras i enheter av tecken. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | Om formeln inte är giltig för dest destination, kopiera bara värden. |
| [getCopyNames()](#getCopyNames--) | Indikerar om namnen kopieras. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Indikerar om intervall ska utökas när intervallet kopieras till intilliggande intervall. |
| [getKeepMacros()](#getKeepMacros--) | Anger om makron ska behållas; |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | När du kopierar intervallet i samma fil och diagrammet refererar till källbladet betyder False att den kopierade diagrammets datakälla inte kommer att ändras. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | I MS Excel, när du kopierar formler som refererar till andra kalkylblad medan du kopierar ett kalkylblad till ett annat, bör de kopierade formlerna referera till källarboken. |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | Anger om målbladet ska refereras till om det refererade bladet inte kopieras. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | Indikerar om kolumnbredden kopieras i enheter av tecken. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | Om formeln inte är giltig för dest destination, kopiera bara värden. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | Indikerar om namnen kopieras. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | Indikerar om intervall ska utökas när intervallet kopieras till intilliggande intervall. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | Anger om makron ska behållas; |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | När du kopierar intervallet i samma fil och diagrammet refererar till källbladet betyder False att den kopierade diagrammets datakälla inte kommer att ändras. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | I MS Excel, när du kopierar formler som refererar till andra kalkylblad medan du kopierar ett kalkylblad till ett annat, bör de kopierade formlerna referera till källarboken. |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | Anger om målbladet ska refereras till om det refererade bladet inte kopieras. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


CopyOptions konstruktör.

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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


Indikerar om kolumnbredden kopieras i enheter av tecken.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


Om formeln inte är giltig för dest destination, kopiera bara värden.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


Indikerar om namnen kopieras.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


Indikerar om intervall ska utökas när intervallet kopieras till intilliggande intervall.

**Remarks**

Om det är true, utökas endast intervallet för hyperlänken, utan att lägga till en ny hyperlänk när hyperlänkar kopieras till intilliggande rader.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


Anger om makron ska behållas;

**Remarks**

Endast för kopiering av arbetsbok.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


När du kopierar intervallet i samma fil och diagrammet refererar till källbladet betyder False att den kopierade diagrammets datakälla inte ändras. True betyder att den kopierade diagrammets datakälla refererar till destinationsbladet.

**Remarks**

Standardvärdet är false, det fungerar som MS Excel. Till exempel: om du kopierar ett diagram med datakällan "sheet1!A1:B10" från kalkylbladet "sheet1" till ett annat kalkylblad "sheet2", kommer datakällan att ändras till "sheet2!A1:B10"

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


I MS Excel, när du kopierar formler som refererar till andra kalkylblad medan du kopierar ett kalkylblad till ett annat, bör de kopierade formlerna referera till källarboken. Men i vissa situationer kan användaren behöva att de kopierade formlerna refererar till kalkylblad med samma namn i samma arbetsbok, till exempel när dessa kalkylblad har kopierats innan denna kopieringsoperation, då bör denna egenskap hållas som true.

**Remarks**

Standardvärdet är true.

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


Anger om målbladet ska refereras till om det refererade bladet inte kopieras.

**Remarks**

Fungerar endast när intervallet eller kalkylbladet kopieras från en annan arbetsbok.

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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


Indikerar om kolumnbredden kopieras i enheter av tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


Om formeln inte är giltig för dest destination, kopiera bara värden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


Indikerar om namnen kopieras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


Indikerar om intervall ska utökas när intervallet kopieras till intilliggande intervall.

**Remarks**

Om det är true, utökas endast intervallet för hyperlänken, utan att lägga till en ny hyperlänk när hyperlänkar kopieras till intilliggande rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


Anger om makron ska behållas;

**Remarks**

Endast för kopiering av arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


När du kopierar intervallet i samma fil och diagrammet refererar till källbladet betyder False att den kopierade diagrammets datakälla inte ändras. True betyder att den kopierade diagrammets datakälla refererar till destinationsbladet.

**Remarks**

Standardvärdet är false, det fungerar som MS Excel. Till exempel: om du kopierar ett diagram med datakällan "sheet1!A1:B10" från kalkylbladet "sheet1" till ett annat kalkylblad "sheet2", kommer datakällan att ändras till "sheet2!A1:B10"

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


I MS Excel, när du kopierar formler som refererar till andra kalkylblad medan du kopierar ett kalkylblad till ett annat, bör de kopierade formlerna referera till källarboken. Men i vissa situationer kan användaren behöva att de kopierade formlerna refererar till kalkylblad med samma namn i samma arbetsbok, till exempel när dessa kalkylblad har kopierats innan denna kopieringsoperation, då bör denna egenskap hållas som true.

**Remarks**

Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


Anger om målbladet ska refereras till om det refererade bladet inte kopieras.

**Remarks**

Fungerar endast när intervallet eller kalkylbladet kopieras från en annan arbetsbok.

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

