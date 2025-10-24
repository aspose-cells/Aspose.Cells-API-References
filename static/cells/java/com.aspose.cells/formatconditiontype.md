##FormatConditionType
Conditional format rule type.
**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```
Conditional format rule type.
## Fields
| Field | Description |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | This conditional formatting rule highlights cells that are above or below the average for all values in the range. |
| [BEGINS_WITH](#BEGINS-WITH) | This conditional formatting rule highlights cells in the range that begin with the given text. |
| [CELL_VALUE](#CELL-VALUE) | This conditional formatting rule compares a cell value to a formula calculated result, using an operator. |
| [COLOR_SCALE](#COLOR-SCALE) | This conditional formatting rule creates a gradated color scale on the cells. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | This conditional formatting rule highlights cells that are completely blank. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | This conditional formatting rule highlights cells with formula errors. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | This conditional formatting rule highlights cells containing given text. |
| [DATA_BAR](#DATA-BAR) | This conditional formatting rule displays a gradated data bar in the range of cells. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | This conditional formatting rule highlights duplicated values. |
| [ENDS_WITH](#ENDS-WITH) | This conditional formatting rule highlights cells ending with given text. |
| [EXPRESSION](#EXPRESSION) | This conditional formatting rule contains a formula to evaluate. |
| [ICON_SET](#ICON-SET) | This conditional formatting rule applies icons to cells according to their values. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | This conditional formatting rule highlights cells that are not blank. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | This conditional formatting rule highlights cells without formula errors. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | This conditional formatting rule highlights cells that do not contain given text. |
| [TIME_PERIOD](#TIME-PERIOD) | This conditional formatting rule highlights cells containing dates in the specified time period. |
| [TOP_10](#TOP-10) | This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | This conditional formatting rule highlights unique values in the range. |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```
This conditional formatting rule highlights cells that are above or below the average for all values in the range.
### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```
This conditional formatting rule highlights cells in the range that begin with the given text. Equivalent to using the LEFT() sheet function and comparing values.
### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```
This conditional formatting rule compares a cell value to a formula calculated result, using an operator.
### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```
This conditional formatting rule creates a gradated color scale on the cells.
### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```
This conditional formatting rule highlights cells that are completely blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank.
### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```
This conditional formatting rule highlights cells with formula errors. Equivalent to using ISERROR() sheet function to determine if there is a formula error.
### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```
This conditional formatting rule highlights cells containing given text. Equivalent to using the SEARCH() sheet function to determine whether the cell contains the text.
### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```
This conditional formatting rule displays a gradated data bar in the range of cells.
### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```
This conditional formatting rule highlights duplicated values.
### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```
This conditional formatting rule highlights cells ending with given text. Equivalent to using the RIGHT() sheet function and comparing values.
### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```
This conditional formatting rule contains a formula to evaluate. When the formula result is true, the cell is highlighted.
### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```
This conditional formatting rule applies icons to cells according to their values.
### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```
This conditional formatting rule highlights cells that are not blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank.
### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```
This conditional formatting rule highlights cells without formula errors. Equivalent to using ISERROR() sheet function to determine if there is a formula error.
### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```
This conditional formatting rule highlights cells that do not contain given text. Equivalent of using SEARCH() sheet function to determine whether the cell contains the text or not.
### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```
This conditional formatting rule highlights cells containing dates in the specified time period. The underlying value of the cell is evaluated, therefore the cell does not need to be formatted as a date to be evaluated. For example, with a cell containing the value 38913 the conditional format shall be applied if the rule requires a value of 7/14/2006.
### TOP_10 {#TOP-10}
```
public static final int TOP_10
```
This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.
### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```
This conditional formatting rule highlights unique values in the range.
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
