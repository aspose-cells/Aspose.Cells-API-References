---
title: "LookInType"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar typ för 'look in'."
type: docs
url: /sv/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

Representerar typ för 'look in'.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [COMMENTS](#COMMENTS) | Hittar objekt endast från cellens kommentar. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | Hitta objekt endast från cellens formaterade värde([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [FORMULAS](#FORMULAS) | Hittar det sökta objektet från formeln([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) om cellen är en formel, annars hittas det från cellens ursprungliga värde (samma som [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)). |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | Ignorerar celler som inte är en formel. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | Hitta objektet endast från cellens ursprungliga värde. |
| [VALUES](#VALUES) | Hittar objektet från cellens ursprungliga värde([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) och det formaterade värdet([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | Ignorerar celler som är en formel. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


Hittar objektet endast från cellens kommentar. Ignorerar de celler som saknar kommentar.

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


Hitta objekt endast från cellens formaterade värde([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


Hittar det sökta objektet från formeln([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) om cellen är en formel, annars hittas det från cellens ursprungliga värde (samma som [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)).

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


Ignorerar celler som inte är en formel. För de celler som är en formel, hittas det sökta objektet från formeln([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)).

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


Hitta objektet endast från cellens ursprungliga värde.

### VALUES {#VALUES}
```
public static final int VALUES
```


Hittar objektet från cellens ursprungliga värde([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) och det formaterade värdet([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


Ignorerar celler som är en formel. För de celler som inte är en formel är det samma som [VALUES](../../com.aspose.cells/lookintype\#VALUES).

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

