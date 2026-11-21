---
title: "PivotFieldGroupOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Alternativ för gruppering av pivotfält."
type: docs
url: /sv/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

Alternativ för gruppering av pivotfält.

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | Hämtar diskreta gruppobjekt. |
| [getEndDate()](#getEndDate--) | Hämtar slutvärdet för grupperingsintervallet. |
| [getEndNumber()](#getEndNumber--) | Hämtar slutvärdet för grupperingsintervallet. |
| [getGroupType()](#getGroupType--) | Hämtar grupperingstypen för pivottfältet. |
| [getGroupTypes()](#getGroupTypes--) | Hämtar grupperingstypen för pivottfältet. |
| [getInterval()](#getInterval--) | Hämtar intervallstorleken för varje grupp. |
| [getNewPivotField()](#getNewPivotField--) | Hämtar ett värde som indikerar om nya pivottfält ska skapas efter gruppering. |
| [getStartDate()](#getStartDate--) | Hämtar startvärdet för grupperingsintervallet. |
| [getStartNumber()](#getStartNumber--) | Hämtar startvärdet för grupperingsintervallet. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | Hämtar ett värde som indikerar om slutvärdet bestäms automatiskt. |
| [isAutoStart()](#isAutoStart--) | Hämtar ett värde som indikerar om startvärdet bestäms automatiskt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | Ställer in ett värde som indikerar om slutvärdet bestäms automatiskt. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | Ställer in ett värde som indikerar om startvärdet bestäms automatiskt. |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | Ställer in diskreta gruppobjekt. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | Ställer in slutvärdet för grupperingsintervallet. |
| [setEndNumber(double value)](#setEndNumber-double-) | Ställer in slutvärdet för grupperingsintervallet. |
| [setGroupType(int value)](#setGroupType-int-) | Ställer in grupperingstypen för pivottfältet. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | Ställer in grupperingstypen för pivottfältet. |
| [setInterval(double value)](#setInterval-double-) | Ställer in intervallstorleken för varje grupp. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | Ställer in ett värde som indikerar om nya pivottfält ska skapas efter gruppering. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Ställer in startvärdet för grupperingsintervallet. |
| [setStartNumber(double value)](#setStartNumber-double-) | Ställer in startvärdet för grupperingsintervallet. |
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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


Hämtar diskreta gruppobjekt.

**Remarks**

Om denna egenskap är inställd,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


Hämtar slutvärdet för grupperingsintervallet.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


Hämtar slutvärdet för grupperingsintervallet.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


Hämtar grupperingstypen för pivottfältet. Endast för gruppering av datum/tid-pivottfält.

Se [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

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


Hämtar grupperingstypen för pivottfältet.

Se [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

Ordningen i denna egenskap kommer att ignoreras. När du specificerar flera grupptyper kommer basgruppfält att infogas i stigande ordning och visa gruppfält till rad/kolumn‑region i fallande ordning (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


Hämtar intervallstorleken för varje grupp.

**Remarks**

Endast för nummer- och daggrupp.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


Hämtar ett värde som indikerar om nya pivottfält ska skapas efter gruppering.

**Remarks**

Om den inte uttryckligen anges är standardvärdet falskt för numerisk gruppering och sant för datum‑tid gruppering, sant för diskret grupp. Fungerar endast för det första nya grupp‑pivotfältet för basfältet.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Hämtar startvärdet för grupperingsintervallet.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


Hämtar startvärdet för grupperingsintervallet.

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


Hämtar ett värde som indikerar om slutvärdet bestäms automatiskt.

**Remarks**

Om [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) eller [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) är angivet, kommer denna egenskap att vara falsk.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


Hämtar ett värde som indikerar om startvärdet bestäms automatiskt.

**Remarks**

Om [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) eller [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) är angivet, kommer denna egenskap att vara falsk.

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


Ställer in ett värde som indikerar om slutvärdet bestäms automatiskt.

**Remarks**

Om [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) eller [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) är angivet, kommer denna egenskap att vara falsk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


Ställer in ett värde som indikerar om startvärdet bestäms automatiskt.

**Remarks**

Om [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) eller [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) är angivet, kommer denna egenskap att vara falsk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


Ställer in diskreta gruppobjekt.

**Remarks**

Om denna egenskap är inställd,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


Ställer in slutvärdet för grupperingsintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


Ställer in slutvärdet för grupperingsintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


Ställer in grupperingstypen för pivotfältet. Endast för gruppering av datum‑tid pivotfält.

Se [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


Ställer in grupperingstypen för pivottfältet.

Se [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

Ordningen i denna egenskap kommer att ignoreras. När du specificerar flera grupptyper kommer basgruppfält att infogas i stigande ordning och visa gruppfält till rad/kolumn‑region i fallande ordning (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


Ställer in intervallstorleken för varje grupp.

**Remarks**

Endast för nummer- och daggrupp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


Ställer in ett värde som indikerar om nya pivottfält ska skapas efter gruppering.

**Remarks**

Om den inte uttryckligen anges är standardvärdet falskt för numerisk gruppering och sant för datum‑tid gruppering, sant för diskret grupp. Fungerar endast för det första nya grupp‑pivotfältet för basfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Ställer in startvärdet för grupperingsintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


Ställer in startvärdet för grupperingsintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

