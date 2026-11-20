---
title: "PivotFieldGroupOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Optionen für die Gruppierungseinstellungen des Pivot-Feldes."
type: docs
url: /de/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

Optionen für die Gruppierungseinstellungen des Pivot-Feldes.

**Example**

```
         // Load the sample workbook
         Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
         // Access the second worksheet and its pivot table
         PivotTable pt = wb.getWorksheets().get(1).getPivotTables().get(0);
         // Group the first row field (a date field) by months and quarters
         PivotFieldGroupOptions options = new PivotFieldGroupOptions();
         options.setStartDate(new DateTime(2008, 1, 1));
         options.setEndDate(new DateTime(2008, 9, 5));
         options.setGroupTypes(new /*PivotGroupByType*/int[] { PivotGroupByType.MONTHS, PivotGroupByType.QUARTERS });
         pt.getRowFields().get(0).group(options);
         // Calculate the pivot table data and save the output file
         pt.calculateData();
         wb.save("outputGroupPivotFieldsInPivotTable.xlsx");
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | Ruft diskrete Gruppenelemente ab. |
| [getEndDate()](#getEndDate--) | Ruft den Endwert des Gruppierungsbereichs ab. |
| [getEndNumber()](#getEndNumber--) | Ruft den Endwert des Gruppierungsbereichs ab. |
| [getGroupType()](#getGroupType--) | Ruft den Gruppierungstyp für das Pivot‑Feld ab. |
| [getGroupTypes()](#getGroupTypes--) | Ruft den Gruppierungstyp für das Pivot‑Feld ab. |
| [getInterval()](#getInterval--) | Ruft die Intervallgröße für jede Gruppe ab. |
| [getNewPivotField()](#getNewPivotField--) | Ruft einen Wert ab, der angibt, ob nach der Gruppierung neue Pivot‑Felder erstellt werden sollen. |
| [getStartDate()](#getStartDate--) | Ruft den Startwert des Gruppierungsbereichs ab. |
| [getStartNumber()](#getStartNumber--) | Ruft den Startwert des Gruppierungsbereichs ab. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | Ruft einen Wert ab, der angibt, ob der Endwert automatisch bestimmt wird. |
| [isAutoStart()](#isAutoStart--) | Ruft einen Wert ab, der angibt, ob der Startwert automatisch bestimmt wird. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | Setzt einen Wert, der angibt, ob der Endwert automatisch bestimmt wird. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | Setzt einen Wert, der angibt, ob der Startwert automatisch bestimmt wird. |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | Setzt diskrete Gruppenelemente. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | Setzt den Endwert des Gruppierungsbereichs. |
| [setEndNumber(double value)](#setEndNumber-double-) | Setzt den Endwert des Gruppierungsbereichs. |
| [setGroupType(int value)](#setGroupType-int-) | Setzt den Gruppierungstyp für das Pivot‑Feld. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | Setzt den Gruppierungstyp für das Pivot‑Feld. |
| [setInterval(double value)](#setInterval-double-) | Setzt die Intervallgröße für jede Gruppe. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | Setzt einen Wert, der angibt, ob nach der Gruppierung neue Pivot‑Felder erstellt werden sollen. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Setzt den Startwert des Gruppierungsbereichs. |
| [setStartNumber(double value)](#setStartNumber-double-) | Setzt den Startwert des Gruppierungsbereichs. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupOptions() {#PivotFieldGroupOptions--}
```
public PivotFieldGroupOptions()
```


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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


Ruft diskrete Gruppenelemente ab.

**Remarks**

Wenn diese Eigenschaft gesetzt ist,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


Ruft den Endwert des Gruppierungsbereichs ab.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


Ruft den Endwert des Gruppierungsbereichs ab.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


Ruft den Gruppierungstyp für das Pivot‑Feld ab. Nur für die Gruppierung von Datums‑Uhrzeit‑Pivot‑Feldern.

Siehe [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Example**

```
         //init
         PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
         // Group by year and month together
         /*PivotGroupByType*/int pivotGroupByType = pivotFieldGroupOptions.getGroupType();
         pivotGroupByType = PivotGroupByType.YEARS | PivotGroupByType.MONTHS;
         pivotFieldGroupOptions.setGroupType(pivotGroupByType);
```

**Returns:**
int
### getGroupTypes() {#getGroupTypes--}
```
public int[] getGroupTypes()
```


Ruft den Gruppierungstyp für das Pivot‑Feld ab.

Siehe [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

Die Reihenfolge in dieser Eigenschaft wird ignoriert. Beim Angeben mehrerer Gruppentypen werden Basisgruppenfelder in aufsteigender Reihenfolge eingefügt und das Gruppenfeld im Zeilen/Spalten‑Bereich in absteigender Reihenfolge angezeigt (Jahre \\u922b?Quartale \\u922b?Monate \\u922b?Tage \\u922b?Stunden \\u922b?Minuten \\u922b?Sekunden).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


Ruft die Intervallgröße für jede Gruppe ab.

**Remarks**

Nur für Zahlen‑ und Tagesgruppen.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


Ruft einen Wert ab, der angibt, ob nach der Gruppierung neue Pivot‑Felder erstellt werden sollen.

**Remarks**

Wenn nicht explizit festgelegt, ist der Standardwert für numerische Gruppierung false und für Datums‑Zeit‑Gruppierung true, für diskrete Gruppen ebenfalls true. Funktioniert nur für das erste neue Grupp‑Pivot‑Feld des Basisfelds.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Ruft den Startwert des Gruppierungsbereichs ab.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


Ruft den Startwert des Gruppierungsbereichs ab.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoEnd() {#isAutoEnd--}
```
public boolean isAutoEnd()
```


Ruft einen Wert ab, der angibt, ob der Endwert automatisch bestimmt wird.

**Remarks**

Wenn [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) oder [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) festgelegt ist, wird diese Eigenschaft false sein.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


Ruft einen Wert ab, der angibt, ob der Startwert automatisch bestimmt wird.

**Remarks**

Wenn [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) oder [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) festgelegt ist, wird diese Eigenschaft false sein.

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




### setAutoEnd(boolean value) {#setAutoEnd-boolean-}
```
public void setAutoEnd(boolean value)
```


Setzt einen Wert, der angibt, ob der Endwert automatisch bestimmt wird.

**Remarks**

Wenn [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) oder [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) festgelegt ist, wird diese Eigenschaft false sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


Setzt einen Wert, der angibt, ob der Startwert automatisch bestimmt wird.

**Remarks**

Wenn [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) oder [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) festgelegt ist, wird diese Eigenschaft false sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


Setzt diskrete Gruppenelemente.

**Remarks**

Wenn diese Eigenschaft gesetzt ist,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


Setzt den Endwert des Gruppierungsbereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


Setzt den Endwert des Gruppierungsbereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


Legt den Gruppierungstyp für das Pivot‑Feld fest. Nur für die Gruppierung von Datums‑Zeit‑Pivot‑Feldern.

Siehe [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


Setzt den Gruppierungstyp für das Pivot‑Feld.

Siehe [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

Die Reihenfolge in dieser Eigenschaft wird ignoriert. Beim Angeben mehrerer Gruppentypen werden Basisgruppenfelder in aufsteigender Reihenfolge eingefügt und das Gruppenfeld im Zeilen/Spalten‑Bereich in absteigender Reihenfolge angezeigt (Jahre \\u922b?Quartale \\u922b?Monate \\u922b?Tage \\u922b?Stunden \\u922b?Minuten \\u922b?Sekunden).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


Setzt die Intervallgröße für jede Gruppe.

**Remarks**

Nur für Zahlen‑ und Tagesgruppen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


Setzt einen Wert, der angibt, ob nach der Gruppierung neue Pivot‑Felder erstellt werden sollen.

**Remarks**

Wenn nicht explizit festgelegt, ist der Standardwert für numerische Gruppierung false und für Datums‑Zeit‑Gruppierung true, für diskrete Gruppen ebenfalls true. Funktioniert nur für das erste neue Grupp‑Pivot‑Feld des Basisfelds.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Setzt den Startwert des Gruppierungsbereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


Setzt den Startwert des Gruppierungsbereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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

