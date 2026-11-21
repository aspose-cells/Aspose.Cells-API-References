---
title: "ConditionalFormattingValue"
second_title: "Aspose.Cells för Java API-referens"
description: "Beskriver värdena för interpolationspunkterna i en gradientskala dataBar eller iconSet."
type: docs
url: /sv/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

Beskriver värdena för interpolationspunkterna i en gradientskala, dataBar eller iconSet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Hämtar typen för detta villkorsformateringsvärdeobjekt. |
| [getValue()](#getValue--) | Hämtar värdet för detta villkorsformateringsvärdeobjekt. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | Hämtar flaggan för Större än eller lika med. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | Ställer in flaggan för Större än eller lika med. |
| [setType(int value)](#setType-int-) | Ställer in typen för detta villkorsformateringsvärdeobjekt. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Ställer in värdet för detta villkorsformateringsvärdeobjekt. |
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
### getType() {#getType--}
```
public int getType()
```


Hämtar typen för detta villkorsformateringsvärdeobjekt. Att sätta typen till FormatConditionValueType.Min eller FormatConditionValueType.Max kommer automatiskt att sätta \"Value\" till null.

Se [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Hämtar värdet för detta villkorsformateringsvärdeobjekt. Det bör användas tillsammans med Type.

**Remarks**

Om värdet är en sträng och börjar med \"=\", kommer det att bearbetas som en formel, annars behandlar vi det som ett enkelt värde.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


Hämtar flaggan för Större än eller lika med. Använd endast för icon sets, bestämmer om detta tröskelvärde använder operatorn större än eller lika med. 'false' indikerar att 'större än' används istället för 'större än eller lika med'. Standardvärdet är true.

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


Ställer in flaggan för Större än eller lika med. Använd endast för icon sets, bestämmer om detta tröskelvärde använder operatorn större än eller lika med. 'false' indikerar att 'större än' används istället för 'större än eller lika med'. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Ställer in typen för detta villkorsformateringsvärdeobjekt. Att sätta typen till FormatConditionValueType.Min eller FormatConditionValueType.Max kommer automatiskt att sätta \"Value\" till null.

Se [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Ställer in värdet för detta villkorsformateringsvärdeobjekt. Det bör användas i kombination med Type.

**Remarks**

Om värdet är en sträng och börjar med \"=\", kommer det att bearbetas som en formel, annars behandlar vi det som ett enkelt värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

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

