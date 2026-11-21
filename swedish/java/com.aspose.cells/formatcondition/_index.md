---
title: "FormatCondition"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar villkorsformateringsvillkor."
type: docs
url: /sv/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

Representerar villkorsformateringsvillkor.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
 
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
 
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
 
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         //Saving the Excel file
         workbook.save("output.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | Hämta den villkorliga formateringens "AboveAverage"-instans. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | Hämta den villkorliga formateringens "ColorScale"-instans. |
| [getDataBar()](#getDataBar--) | Hämta den villkorliga formateringens "DataBar"-instans. |
| [getFormula1()](#getFormula1--) | Hämtar värdet eller uttrycket som är associerat med villkorlig formatering. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Hämtar värdet eller uttrycket som är associerat med detta formatvillkor. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Hämtar värdet eller uttrycket för cellens villkorliga formatering. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | Hämtar formeln för cellens villkorliga formatering. |
| [getFormula2()](#getFormula2--) | Hämtar värdet eller uttrycket som är associerat med villkorlig formatering. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Hämtar värdet eller uttrycket som är associerat med detta formatvillkor. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Hämtar värdet eller uttrycket för cellens villkorliga formatering. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | Hämtar formeln för cellens villkorliga formatering. |
| [getIconSet()](#getIconSet--) | Hämta den villkorliga formateringens "IconSet"-instans. |
| [getOperator()](#getOperator--) | Hämtar den villkorliga formatoperatorns typ. |
| [getPriority()](#getPriority--) | Prioriteten för detta villkorliga formateringsregel. |
| [getStopIfTrue()](#getStopIfTrue--) | Sant, inga regler med lägre prioritet får tillämpas över denna regel när regeln utvärderas till sant. |
| [getStyle()](#getStyle--) | Hämtar eller anger stil för villkorligt formaterade cellområden. |
| [getText()](#getText--) | Textvärdet i en "text contains"-villkorlig formateringsregel. |
| [getTimePeriod()](#getTimePeriod--) | Den tillämpliga tidsperioden i en "date occurrin"-villkorlig formateringsregel. |
| [getTop10()](#getTop10--) | Hämta den villkorliga formateringens "Top10"-instans. |
| [getType()](#getType--) | Hämtar om den villkorliga formattypen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Anger värdet eller uttrycket som är associerat med villkorlig formatering. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Anger värdet eller uttrycket som är associerat med detta formatvillkor. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Anger värdet eller uttrycket som är associerat med villkorlig formatering. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Anger värdet eller uttrycket som är associerat med detta formatvillkor. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | Anger värdet eller uttrycket som är associerat med detta formatvillkor. |
| [setOperator(int value)](#setOperator-int-) | Anger den villkorliga formatoperatorns typ. |
| [setPriority(int value)](#setPriority-int-) | Prioriteten för detta villkorliga formateringsregel. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | Sant, inga regler med lägre prioritet får tillämpas över denna regel när regeln utvärderas till sant. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Hämtar eller anger stil för villkorligt formaterade cellområden. |
| [setText(String value)](#setText-java.lang.String-) | Textvärdet i en "text contains"-villkorlig formateringsregel. |
| [setTimePeriod(int value)](#setTimePeriod-int-) | Den tillämpliga tidsperioden i en "date occurrin"-villkorlig formateringsregel. |
| [setType(int value)](#setType-int-) | Anger om den villkorsstyrda formattypen. |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


Hämta den villkorsstyrda formateringens "AboveAverage"-instans. Standardinstansens regel markerar celler som ligger över genomsnittet för alla värden i intervallet. Giltig endast för typ = AboveAverage.

**Returns:**
[AboveAverage](../../com.aspose.cells/aboveaverage) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorScale() {#getColorScale--}
```
public ColorScale getColorScale()
```


Hämta den villkorsstyrda formateringens "ColorScale"-instans. Standardinstansen är en "grön-gul-röd" 3ColorScale. Giltig endast för typ = ColorScale.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


Hämta den villkorsstyrda formateringens "DataBar"-instans. Standardinstansens färg är blå. Giltig endast för typ = DataBar.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Hämtar värdet eller uttrycket som är associerat med villkorlig formatering.

**Remarks**

Lägg till alla områden innan du anger formel. För att ange formel för detta villkor, om inmatningsvärdet börjar med '=', kommer det att behandlas som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\\"=...\\"".

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Hämtar värdet eller uttrycket som är associerat med detta formatvillkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - Värdet eller uttrycket som är associerat med detta formatvillkor.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Hämtar värdet eller uttrycket för cellens villkorliga formatering.

**Remarks**

Den angivna cellen måste ingå i denna villkorsstyrda formatering, annars returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
java.lang.String - Värdet eller uttrycket som är associerat med cellens villkorsstyrda formatering.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


Hämtar formeln för cellens villkorliga formatering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
java.lang.String - Formeln.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Hämtar värdet eller uttrycket som är associerat med villkorlig formatering.

**Remarks**

Lägg till alla områden innan du anger formel. För att ange formel för detta villkor, om inmatningsvärdet börjar med '=', kommer det att behandlas som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\\"=...\\"".

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Hämtar värdet eller uttrycket som är associerat med detta formatvillkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - Värdet eller uttrycket som är associerat med detta formatvillkor.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Hämtar värdet eller uttrycket för cellens villkorliga formatering.

**Remarks**

Den angivna cellen måste ingå i denna villkorsstyrda formatering, annars returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
java.lang.String - Värdet eller uttrycket som är associerat med cellens villkorsstyrda formatering.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


Hämtar formeln för cellens villkorliga formatering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
java.lang.String - Formeln.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


Hämta den villkorsstyrda formateringens "IconSet"-instans. Standardinstansens IconSetType är TrafficLights31. Giltig endast för typ = IconSet.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


Hämtar den villkorliga formatoperatorns typ.

Se [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


Prioriteten för denna villkorsstyrda formateringsregel. Detta värde används för att avgöra vilken formatering som ska utvärderas och renderas. Lägre numeriska värden har högre prioritet än högre numeriska värden, där '1' är den högsta prioriteten.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


Sant, inga regler med lägre prioritet får tillämpas över denna regel när den utvärderas till sant. Gäller endast för Excel 2007;

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Hämtar eller anger stil för villkorligt formaterade cellområden.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


Textvärdet i en "text contains"-regel för villkorsstyrd formatering. Giltig endast för typ = containsText, notContainsText, beginsWith och endsWith. Standardvärdet är null.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


Den tillämpliga tidsperioden i en "date occurrin"-regel för villkorsstyrd formatering. Giltig endast för typ = timePeriod. Standardvärdet är TimePeriodType.Today.

Se [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


Hämta den villkorsstyrda formateringens "Top10"-instans. Standardinstansens regel markerar celler vars värden faller inom de 10 bästa. Giltig endast för typ = Top10.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


Hämtar om den villkorliga formattypen.

Se [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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




### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Anger värdet eller uttrycket som är associerat med villkorlig formatering.

**Remarks**

Lägg till alla områden innan du anger formel. För att ange formel för detta villkor, om inmatningsvärdet börjar med '=', kommer det att behandlas som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\\"=...\\"".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Anger värdet eller uttrycket som är associerat med detta formatvillkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Värdet eller uttrycket som är associerat med detta formatvillkor. Om inmatningsvärdet börjar med '=', behandlas det som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\\"=...\\"". |
| isR1C1 | boolean | Om formeln är en R1C1-formel. |
| isLocal | boolean | Om formeln är lokalanpassad. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Anger värdet eller uttrycket som är associerat med villkorlig formatering.

**Remarks**

Lägg till alla områden innan du anger formel. För att ange formel för detta villkor, om inmatningsvärdet börjar med '=', kommer det att behandlas som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\\"=...\\"".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Anger värdet eller uttrycket som är associerat med detta formatvillkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Värdet eller uttrycket som är associerat med detta formatvillkor. Om inmatningsvärdet börjar med '=', behandlas det som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\\"=...\\"". |
| isR1C1 | boolean | Om formeln är en R1C1-formel. |
| isLocal | boolean | Om formeln är lokalanpassad. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


Anger värdet eller uttrycket som är associerat med detta formatvillkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula1 | java.lang.String | Värdet eller uttrycket som är associerat med detta formatvillkor. Om inmatningsvärdet börjar med '=', behandlas det som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\\"=...\\"". |
| formula2 | java.lang.String | Värdet eller uttrycket som är associerat med detta formatvillkor. Indataformatet är samma som formula1. |
| isR1C1 | boolean | Om formeln är en R1C1-formel. |
| isLocal | boolean | Om formeln är lokalanpassad. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Anger den villkorliga formatoperatorns typ.

Se [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


Prioriteten för denna villkorsstyrda formateringsregel. Detta värde används för att avgöra vilken formatering som ska utvärderas och renderas. Lägre numeriska värden har högre prioritet än högre numeriska värden, där '1' är den högsta prioriteten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


Sant, inga regler med lägre prioritet får tillämpas över denna regel när den utvärderas till sant. Gäller endast för Excel 2007;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Hämtar eller anger stil för villkorligt formaterade cellområden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Textvärdet i en "text contains"-regel för villkorsstyrd formatering. Giltig endast för typ = containsText, notContainsText, beginsWith och endsWith. Standardvärdet är null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


Den tillämpliga tidsperioden i en "date occurrin"-regel för villkorsstyrd formatering. Giltig endast för typ = timePeriod. Standardvärdet är TimePeriodType.Today.

Se [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Anger om den villkorsstyrda formattypen.

Se [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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

