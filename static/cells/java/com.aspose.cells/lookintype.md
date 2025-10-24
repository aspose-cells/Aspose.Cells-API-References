##LookInType
Represents look in type.
**Inheritance:**
java.lang.Object
```
public final class LookInType
```
Represents look in type.
## Fields
| Field | Description |
| --- | --- |
| [COMMENTS](#COMMENTS) | Finds object from cell's comment only. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | Find object from cell's formatted value([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) only. |
| [FORMULAS](#FORMULAS) | Finds the searched object from formula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) if the cell is formula, otherwise finds from cell's original value(same with [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)). |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | Ignores cells that are not formula. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | Find object from cell's original value only. |
| [VALUES](#VALUES) | Finds object from cell's original value([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) and formatted value([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | Ignores cells that are formula. |
## Methods
| Method | Description |
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
Finds object from cell's comment only. Ignores those cells that have no comment.
### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```
Find object from cell's formatted value([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) only.
### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```
Finds the searched object from formula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) if the cell is formula, otherwise finds from cell's original value(same with [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)).
### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```
Ignores cells that are not formula. For those cells that are formula, finds the searched object from formula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)).
### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```
Find object from cell's original value only.
### VALUES {#VALUES}
```
public static final int VALUES
```
Finds object from cell's original value([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) and formatted value([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).
### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```
Ignores cells that are formula. For those cells that are not formula, it is same with [VALUES](../../com.aspose.cells/lookintype\#VALUES).
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
