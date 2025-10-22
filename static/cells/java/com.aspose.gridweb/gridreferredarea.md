##GridReferredArea
Represents a referred objcet by the formula.
**Inheritance:**
java.lang.Object
```
public class GridReferredArea
```
Represents a referred objcet by the formula.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | The end column of the area. |
| [getEndRow()](#getEndRow--) | The end row of the area. |
| [getExternalFileName()](#getExternalFileName--) | this.KeepedRels = source.KeepedRels; |
| [getSheetName()](#getSheetName--) | Indicates which sheet this is in |
| [getStartColumn()](#getStartColumn--) | The start column of the area. |
| [getStartRow()](#getStartRow--) | The start row of the area. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Gets cell value with given offset from the top-left of this area. |
| [getValues()](#getValues--) | Gets cell values in this area. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Indicates whether this is an area. |
| [isExternalLink()](#isExternalLink--) | Indicates whether this is an external link. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
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
this.KeepedRels = source.KeepedRels;
**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```
Indicates which sheet this is in
**Returns:**
java.lang.String
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
### getValues() {#getValues--}
```
public Object getValues()
```
Gets cell values in this area.
**Returns:**
java.lang.Object - If this area is invalid, "\#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one array for all values in this area.
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
