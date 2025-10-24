##ErrorCheckType
Represents all error check type.
**Inheritance:**
java.lang.Object
```
public final class ErrorCheckType
```
Represents all error check type.
## Fields
| Field | Description |
| --- | --- |
| [CALC](#CALC) | **Remarks** |
| [CALCULATED_COLUMN](#CALCULATED-COLUMN) | Ignore errors when cells contain a value different from a calculated column formula. |
| [EMPTY_CELL_REF](#EMPTY-CELL-REF) | Ignore errors when formulas refer to empty cells. |
| [EVALUATION_ERROR](#EVALUATION-ERROR) | Ignore errors when cells contain formulas that result in an error. |
| [INCONSIST_FORMULA](#INCONSIST-FORMULA) | Ignore errors when a formula in a region of your worksheet differs from other formulas in the same region. |
| [INCONSIST_RANGE](#INCONSIST-RANGE) | Ignore errors when formulas omit certain cells in a region. |
| [NUMBER_STORED_AS_TEXT](#NUMBER-STORED-AS-TEXT) | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| [TABLE_DATA_VALIDATION](#TABLE-DATA-VALIDATION) | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
| [TEXT_DATE](#TEXT-DATE) | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| [TEXT_NUMBER](#TEXT-NUMBER) | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| [TWO_DIGIT_TEXT_YEAR](#TWO-DIGIT-TEXT-YEAR) | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| [UNLOCKED_FORMULA](#UNLOCKED-FORMULA) | Ignore errors when unlocked cells contain formulas. |
| [UNPROCTED_FORMULA](#UNPROCTED-FORMULA) | Ignore errors when unlocked cells contain formulas. |
| [VALIDATION](#VALIDATION) | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
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
### CALC {#CALC}
```
public static final int CALC
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use ErrorCheckType.EvaluationError enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### CALCULATED_COLUMN {#CALCULATED-COLUMN}
```
public static final int CALCULATED_COLUMN
```
Ignore errors when cells contain a value different from a calculated column formula.
### EMPTY_CELL_REF {#EMPTY-CELL-REF}
```
public static final int EMPTY_CELL_REF
```
Ignore errors when formulas refer to empty cells.
### EVALUATION_ERROR {#EVALUATION-ERROR}
```
public static final int EVALUATION_ERROR
```
Ignore errors when cells contain formulas that result in an error.
### INCONSIST_FORMULA {#INCONSIST-FORMULA}
```
public static final int INCONSIST_FORMULA
```
Ignore errors when a formula in a region of your worksheet differs from other formulas in the same region.
### INCONSIST_RANGE {#INCONSIST-RANGE}
```
public static final int INCONSIST_RANGE
```
Ignore errors when formulas omit certain cells in a region.
### NUMBER_STORED_AS_TEXT {#NUMBER-STORED-AS-TEXT}
```
public static final int NUMBER_STORED_AS_TEXT
```
Ignore errors when numbers are formatted as text or are preceded by an apostrophe
### TABLE_DATA_VALIDATION {#TABLE-DATA-VALIDATION}
```
public static final int TABLE_DATA_VALIDATION
```
Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified.
### TEXT_DATE {#TEXT-DATE}
```
public static final int TEXT_DATE
```
Ignore errors when formulas contain text formatted cells with years represented as 2 digits.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ErrorCheckType.TwoDigitTextYear enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### TEXT_NUMBER {#TEXT-NUMBER}
```
public static final int TEXT_NUMBER
```
Ignore errors when numbers are formatted as text or are preceded by an apostrophe
**Remarks**
NOTE: This member is now obsolete. Instead, please use ErrorCheckType.NumberStoredAsText enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### TWO_DIGIT_TEXT_YEAR {#TWO-DIGIT-TEXT-YEAR}
```
public static final int TWO_DIGIT_TEXT_YEAR
```
Ignore errors when formulas contain text formatted cells with years represented as 2 digits.
### UNLOCKED_FORMULA {#UNLOCKED-FORMULA}
```
public static final int UNLOCKED_FORMULA
```
Ignore errors when unlocked cells contain formulas.
### UNPROCTED_FORMULA {#UNPROCTED-FORMULA}
```
public static final int UNPROCTED_FORMULA
```
Ignore errors when unlocked cells contain formulas.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ErrorCheckType.UnproctedFormula enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```
Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ErrorCheckType.TableDataValidation enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
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
