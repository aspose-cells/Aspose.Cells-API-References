---
title: "PivotFormatCondition"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine PivotTable-Formatbedingung in der PivotFormatCondition‑Sammlung dar."
type: docs
url: /de/java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

Stellt eine PivotTable-Formatbedingung in der PivotFormatCondition‑Sammlung dar.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen die Klasse [PivotConditionalFormat](../../com.aspose.cells/pivotconditionalformat). Diese Methode wird 12 Monate nach Dezember 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Example**

```
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Spaltenfeldern hinzu. |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Spaltenfeldern hinzu. |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Datenfeldern hinzu. |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Datenfeldern hinzu. |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Zeilenfeldern hinzu. |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Zeilenfeldern hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Liefert Bedingungen für das bedingte Format der Pivot-Tabelle . |
| [getRuleType()](#getRuleType--) | Liefert den Regeltyp für das bedingte Format der Pivot-Tabelle . |
| [getScopeType()](#getScopeType--) | Ermittelt den Gültigkeitsbereichstyp für das Pivot-Tabellen-Bedingte Format. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | Legt die bedingten Bereiche des PivotFormatCondition‑Objekts fest. |
| [setRuleType(int value)](#setRuleType-int-) | Legt den Regeltyp für das Pivot-Tabellen-Bedingte Format fest. |
| [setScopeType(int value)](#setScopeType-int-) | Legt den Gültigkeitsbereichstyp für das Pivot-Tabellen-Bedingte Format fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Spaltenfeldern hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | Das PivotField in den Spaltenfeldern. |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Spaltenfeldern hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldName | java.lang.String | Der Name von PivotField. |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Datenfeldern hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | Das PivotField in den Datenfeldern. |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Datenfeldern hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldName | java.lang.String | Der Name von PivotField. |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Zeilenfeldern hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | Das PivotField in den Zeilenfeldern. |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


Fügt eine PivotTable‑Bedingungsformatbegrenzung in den Zeilenfeldern hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldName | java.lang.String | Der Name von PivotField. |

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
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Liefert Bedingungen für das bedingte Format der Pivot-Tabelle .

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Liefert den Regeltyp für das bedingte Format der Pivot-Tabelle .

Siehe [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Ermittelt den Gültigkeitsbereichstyp für das Pivot-Tabellen-Bedingte Format.

Siehe [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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


Legt die bedingten Bereiche des PivotFormatCondition‑Objekts fest.

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Legt den Regeltyp für das Pivot-Tabellen-Bedingte Format fest.

Siehe [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Legt den Gültigkeitsbereichstyp für das Pivot-Tabellen-Bedingte Format fest.

Siehe [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

