##ReferredArea
Represents a referred area by the formula.
**Inheritance:**
java.lang.Object
```
public class ReferredArea
```
Represents a referred area by the formula.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | The end column of the area. |
| [getEndRow()](#getEndRow--) | The end row of the area. |
| [getExternalFileName()](#getExternalFileName--) | Get the external file name if this is an external reference. |
| [getSheetName()](#getSheetName--) | Indicates which sheet this reference is in. |
| [getSheetNames()](#getSheetNames--) | Names of all the worksheets this instance references to. |
| [getStartColumn()](#getStartColumn--) | The start column of the area. |
| [getStartRow()](#getStartRow--) | The start row of the area. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Gets cell value with given offset from the top-left of this area. |
| [getValue(int rowOffset, int colOffset, boolean calculateFormulas)](#getValue-int-int-boolean-) | Gets cell value with given offset from the top-left of this area. |
| [getValues()](#getValues--) | Gets cell values in this area. |
| [getValues(boolean calculateFormulas)](#getValues-boolean-) | Gets cell values in this area. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Indicates whether this is an area. |
| [isEntireColumn()](#isEntireColumn--) | Indicates whether this area contains all rows(entire column). |
| [isEntireRow()](#isEntireRow--) | Indicates whether this area contains all columns(entire row). |
| [isExternalLink()](#isExternalLink--) | Indicates whether this is an external link. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Returns the reference address of this area. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```
The end column of the area.
**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```
The end row of the area.
**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```
Get the external file name if this is an external reference.
**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```
Indicates which sheet this reference is in.
**Remarks**
If it references to multiple worksheets, the returned value is just like the range expression in the formula. For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".
**Returns:**
java.lang.String
### getSheetNames() {#getSheetNames--}
```
public String[] getSheetNames()
```
Names of all the worksheets this instance references to.
**Returns:**
java.lang.String[]
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```
The start column of the area.
**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```
The start row of the area.
**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```
Gets cell value with given offset from the top-left of this area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | row offset from the start row of this area |
| colOffset | int | column offset from the start row of this area |
**Returns:**
java.lang.Object - "\#REF!" if this area is invalid; "\#N/A" if given offset out of this area; Otherwise return the cell value at given position.
### getValue(int rowOffset, int colOffset, boolean calculateFormulas) {#getValue-int-int-boolean-}
```
public Object getValue(int rowOffset, int colOffset, boolean calculateFormulas)
```
Gets cell value with given offset from the top-left of this area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | row offset from the start row of this area |
| colOffset | int | column offset from the start row of this area |
| calculateFormulas | boolean | Whether calculate it recursively if the specified reference is formula |
**Returns:**
java.lang.Object - "\#REF!" if this area is invalid; "\#N/A" if given offset out of this area; Otherwise return the cell value at given position.
### getValues() {#getValues--}
```
public Object getValues()
```
Gets cell values in this area.
**Returns:**
java.lang.Object - If this area is invalid, "\#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.
### getValues(boolean calculateFormulas) {#getValues-boolean-}
```
public Object getValues(boolean calculateFormulas)
```
Gets cell values in this area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculateFormulas | boolean | In this range, if there are some formulas that have not been calculated, this flag denotes whether those formulas should be calculated recursively |
**Returns:**
java.lang.Object - If this area is invalid, "\#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```
Indicates whether this is an area.
**Remarks**
If this is not an area, only StartRow and StartColumn effect.
**Returns:**
boolean
### isEntireColumn() {#isEntireColumn--}
```
public boolean isEntireColumn()
```
Indicates whether this area contains all rows(entire column).
**Returns:**
boolean
### isEntireRow() {#isEntireRow--}
```
public boolean isEntireRow()
```
Indicates whether this area contains all columns(entire row).
**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```
Indicates whether this is an external link.
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
### toString() {#toString--}
```
public String toString()
```
Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3".
**Returns:**
java.lang.String - the reference address of this area.
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
