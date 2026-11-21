---
title: "PivotFormatCondition"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett PivotTable-formatvillkor i PivotFormatCondition-samlingen."
type: docs
url: /sv/java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

Representerar ett PivotTable-formatvillkor i PivotFormatCondition-samlingen.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället klassen [PivotConditionalFormat](../../com.aspose.cells/pivotconditionalformat). Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | Lägger till en villkorlig formatgräns för PivotTable i kolumnfälten. |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | Lägger till en villkorlig formatgräns för PivotTable i kolumnfälten. |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | Lägger till en villkorlig formatgräns för PivotTable i datafälten. |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | Lägger till en villkorlig formatgräns för PivotTable i datafälten. |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | Lägger till en villkorlig formatgräns för PivotTable i radfälten. |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | Lägger till en villkorlig formatgräns för PivotTable i radfälten. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Hämta villkor för pivottabellens villkorliga format. |
| [getRuleType()](#getRuleType--) | Hämtar regeltyp för pivottabellens villkorliga format. |
| [getScopeType()](#getScopeType--) | Hämtar omfångstyp för pivottabellens villkorliga format. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | Ställer in villkorliga områden för PivotFormatCondition-objektet. |
| [setRuleType(int value)](#setRuleType-int-) | Anger regeltyp för pivottabellens villkorliga format. |
| [setScopeType(int value)](#setScopeType-int-) | Anger omfångstyp för pivottabellens villkorliga format. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


Lägger till en villkorlig formatgräns för PivotTable i kolumnfälten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField i kolumnfälten. |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


Lägger till en villkorlig formatgräns för PivotTable i kolumnfälten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldName | java.lang.String | Namnet på PivotField. |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


Lägger till en villkorlig formatgräns för PivotTable i datafälten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField i datafälten. |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


Lägger till en villkorlig formatgräns för PivotTable i datafälten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldName | java.lang.String | Namnet på PivotField. |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


Lägger till en villkorlig formatgräns för PivotTable i radfälten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField i radfälten. |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


Lägger till en villkorlig formatgräns för PivotTable i radfälten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldName | java.lang.String | Namnet på PivotField. |

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
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Hämta villkor för pivottabellens villkorliga format.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Hämtar regeltyp för pivottabellens villkorliga format.

Se [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Hämtar omfångstyp för pivottabellens villkorliga format.

Se [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Returns:**
int
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




### setConditionalAreas() {#setConditionalAreas--}
```
public void setConditionalAreas()
```


Ställer in villkorliga områden för PivotFormatCondition-objektet.

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Anger regeltyp för pivottabellens villkorliga format.

Se [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Anger omfångstyp för pivottabellens villkorliga format.

Se [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

