---
title: "FormatCondition"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Bedingung für die bedingte Formatierung dar."
type: docs
url: /de/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

Stellt die Bedingung für die bedingte Formatierung dar.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | Erhalte die "AboveAverage"‑Instanz der bedingten Formatierung. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | Erhalte die "ColorScale"‑Instanz der bedingten Formatierung. |
| [getDataBar()](#getDataBar--) | Erhalte die "DataBar"‑Instanz der bedingten Formatierung. |
| [getFormula1()](#getFormula1--) | Ermittelt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Ruft den Wert oder Ausdruck ab, der mit dieser Formatbedingung verknüpft ist. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | Ruft die Formel der bedingten Formatierung der Zelle ab. |
| [getFormula2()](#getFormula2--) | Ermittelt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Ruft den Wert oder Ausdruck ab, der mit dieser Formatbedingung verknüpft ist. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | Ruft die Formel der bedingten Formatierung der Zelle ab. |
| [getIconSet()](#getIconSet--) | Holt die "IconSet"-Instanz der bedingten Formatierung. |
| [getOperator()](#getOperator--) | Ruft den Operator-Typ der bedingten Formatierung ab. |
| [getPriority()](#getPriority--) | Die Priorität dieser Regel für bedingte Formatierung. |
| [getStopIfTrue()](#getStopIfTrue--) | True, keine Regeln mit niedrigerer Priorität dürfen über diese Regel angewendet werden, wenn diese Regel zu true evaluiert. |
| [getStyle()](#getStyle--) | Ruft den Stil von bedingt formatierten Zellbereichen ab oder legt ihn fest. |
| [getText()](#getText--) | Der Textwert in einer "text contains"-Bedingten-Formatierungsregel. |
| [getTimePeriod()](#getTimePeriod--) | Der anwendbare Zeitraum in einer "date occurrin"-Bedingten-Formatierungsregel. |
| [getTop10()](#getTop10--) | Holt die "Top10"-Instanz der bedingten Formatierung. |
| [getType()](#getType--) | Ermittelt, ob der Typ der bedingten Formatierung. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| [setOperator(int value)](#setOperator-int-) | Setzt den Operator-Typ der bedingten Formatierung. |
| [setPriority(int value)](#setPriority-int-) | Die Priorität dieser Regel für bedingte Formatierung. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | True, keine Regeln mit niedrigerer Priorität dürfen über diese Regel angewendet werden, wenn diese Regel zu true evaluiert. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Ruft den Stil von bedingt formatierten Zellbereichen ab oder legt ihn fest. |
| [setText(String value)](#setText-java.lang.String-) | Der Textwert in einer "text contains"-Bedingten-Formatierungsregel. |
| [setTimePeriod(int value)](#setTimePeriod-int-) | Der anwendbare Zeitraum in einer "date occurrin"-Bedingten-Formatierungsregel. |
| [setType(int value)](#setType-int-) | Setzt, ob der Typ der bedingten Formatierung. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


Holt die "AboveAverage"-Instanz der bedingten Formatierung. Die Regel der Standardinstanz hebt Zellen hervor, die über dem Durchschnitt aller Werte im Bereich liegen. Nur gültig für Typ = AboveAverage.

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


Holt die "ColorScale"-Instanz der bedingten Formatierung. Die Standardinstanz ist ein "grün-gelb-rot" 3ColorScale. Nur gültig für Typ = ColorScale.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


Holt die "DataBar"-Instanz der bedingten Formatierung. Die Farbe der Standardinstanz ist blau. Nur gültig für Typ = DataBar.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Ermittelt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist.

**Remarks**

Bitte fügen Sie alle Bereiche hinzu, bevor Sie die Formel festlegen. Beim Festlegen der Formel für diese Bedingung wird ein Eingabewert, der mit '=' beginnt, als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer sie im Format: "=\\"=...\\"" als Formel eingeben.

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Ruft den Wert oder Ausdruck ab, der mit dieser Formatbedingung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab.

**Remarks**

Die angegebene Zelle muss von dieser bedingten Formatierung enthalten sein, sonst wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
java.lang.String - Der Wert oder Ausdruck, der mit der bedingten Formatierung der Zelle verknüpft ist.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


Ruft die Formel der bedingten Formatierung der Zelle ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
java.lang.String - Die Formel.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Ermittelt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist.

**Remarks**

Bitte fügen Sie alle Bereiche hinzu, bevor Sie die Formel festlegen. Beim Festlegen der Formel für diese Bedingung wird ein Eingabewert, der mit '=' beginnt, als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer sie im Format: "=\\"=...\\"" als Formel eingeben.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Ruft den Wert oder Ausdruck ab, der mit dieser Formatbedingung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab.

**Remarks**

Die angegebene Zelle muss von dieser bedingten Formatierung enthalten sein, sonst wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
java.lang.String - Der Wert oder Ausdruck, der mit der bedingten Formatierung der Zelle verknüpft ist.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


Ruft die Formel der bedingten Formatierung der Zelle ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
java.lang.String - Die Formel.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


Holt die "IconSet"-Instanz der bedingten Formatierung. Der IconSetType der Standardinstanz ist TrafficLights31. Nur gültig für Typ = IconSet.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


Ruft den Operator-Typ der bedingten Formatierung ab.

Siehe [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


Die Priorität dieser bedingten Formatierungsregel. Dieser Wert wird verwendet, um zu bestimmen, welches Format ausgewertet und gerendert werden soll. Niedrigere numerische Werte haben höhere Priorität als höhere numerische Werte, wobei '1' die höchste Priorität ist.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


Wahr, es dürfen keine Regeln mit niedrigerer Priorität über diese Regel angewendet werden, wenn diese Regel zu wahr evaluiert wird. Gilt nur für Excel 2007;

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ruft den Stil von bedingt formatierten Zellbereichen ab oder legt ihn fest.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


Der Textwert in einer "text contains"-Bedingten-Formatierungsregel. Gültig nur für type = containsText, notContainsText, beginsWith und endsWith. Der Standardwert ist null.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


Der anwendbare Zeitraum in einer "date occurrin"-Bedingten-Formatierungsregel. Gültig nur, wenn type timePeriod ist. Der Standardwert ist TimePeriodType.Today.

Siehe [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


Rufen Sie die "Top10"-Instanz der bedingten Formatierung ab. Die Regel der Standardinstanz hebt Zellen hervor, deren Werte in die Top‑10‑Kategorie fallen. Gültig nur, wenn type Top10 ist.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


Ermittelt, ob der Typ der bedingten Formatierung.

Siehe [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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


Setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist.

**Remarks**

Bitte fügen Sie alle Bereiche hinzu, bevor Sie die Formel festlegen. Beim Festlegen der Formel für diese Bedingung wird ein Eingabewert, der mit '=' beginnt, als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer sie im Format: "=\\"=...\\"" als Formel eingeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. Beginnt der Eingabewert mit '=', wird er als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer sie im Format \"=\\\"=...\\\"\" als Formel eingeben. |
| isR1C1 | boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist.

**Remarks**

Bitte fügen Sie alle Bereiche hinzu, bevor Sie die Formel festlegen. Beim Festlegen der Formel für diese Bedingung wird ein Eingabewert, der mit '=' beginnt, als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer sie im Format: "=\\"=...\\"" als Formel eingeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. Beginnt der Eingabewert mit '=', wird er als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer sie im Format \"=\\\"=...\\\"\" als Formel eingeben. |
| isR1C1 | boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula1 | java.lang.String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. Beginnt der Eingabewert mit '=', wird er als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer sie im Format \"=\\\"=...\\\"\" als Formel eingeben. |
| formula2 | java.lang.String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. Das Eingabeformat ist dasselbe wie bei formula1. |
| isR1C1 | boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Setzt den Operator-Typ der bedingten Formatierung.

Siehe [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


Die Priorität dieser bedingten Formatierungsregel. Dieser Wert wird verwendet, um zu bestimmen, welches Format ausgewertet und gerendert werden soll. Niedrigere numerische Werte haben höhere Priorität als höhere numerische Werte, wobei '1' die höchste Priorität ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


Wahr, es dürfen keine Regeln mit niedrigerer Priorität über diese Regel angewendet werden, wenn diese Regel zu wahr evaluiert wird. Gilt nur für Excel 2007;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Ruft den Stil von bedingt formatierten Zellbereichen ab oder legt ihn fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Der Textwert in einer "text contains"-Bedingten-Formatierungsregel. Gültig nur für type = containsText, notContainsText, beginsWith und endsWith. Der Standardwert ist null.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


Der anwendbare Zeitraum in einer "date occurrin"-Bedingten-Formatierungsregel. Gültig nur, wenn type timePeriod ist. Der Standardwert ist TimePeriodType.Today.

Siehe [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Setzt, ob der Typ der bedingten Formatierung.

Siehe [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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

