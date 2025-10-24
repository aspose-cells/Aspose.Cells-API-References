##GridPivotField
Represents a field in a PivotTable report.
**Inheritance:**
java.lang.Object
```
public class GridPivotField
```
Represents a field in a PivotTable report.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayName()](#getDisplayName--) | Represents the PivotField display name. |
| [getFunction()](#getFunction--) | Represents the function used to summarize the PivotTable data field. |
| [getPosition()](#getPosition--) | Represents the PivotField index in the PivotFields. |
| [hashCode()](#hashCode--) |  |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Sets whether the specific PivotItem in a data field is hidden. |
| [hideItemByName(String name, boolean isHidden)](#hideItemByName-java.lang.String-boolean-) | Sets whether the specific PivotItem in a data field is hidden. |
| [hideItemByValue(String value, boolean isHidden)](#hideItemByValue-java.lang.String-boolean-) | Sets whether the specific PivotItem in a data field is hidden. |
| [isAscendSort()](#isAscendSort--) | Indicates whether the specified PivotTable field is autosorted ascending. |
| [isAutoSort()](#isAutoSort--) | Indicates whether the specified PivotTable field is automatically sorted. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Indicates whether the specified PivotTable field is autosorted ascending. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Indicates whether the specified PivotTable field is automatically sorted. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Represents the PivotField display name. |
| [setFunction(int value)](#setFunction-int-) | Represents the function used to summarize the PivotTable data field. |
| [setPosition(int value)](#setPosition-int-) | Represents the PivotField index in the PivotFields. |
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
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```
Represents the PivotField display name.
**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```
Represents the function used to summarize the PivotTable data field.
See [GridPivotFieldFunction](../../com.aspose.gridweb/gridpivotfieldfunction).
**Returns:**
int
### getPosition() {#getPosition--}
```
public int getPosition()
```
Represents the PivotField index in the PivotFields.
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```
Sets whether the specific PivotItem in a data field is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |
### hideItemByName(String name, boolean isHidden) {#hideItemByName-java.lang.String-boolean-}
```
public void hideItemByName(String name, boolean isHidden)
```
Sets whether the specific PivotItem in a data field is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |
### hideItemByValue(String value, boolean isHidden) {#hideItemByValue-java.lang.String-boolean-}
```
public void hideItemByValue(String value, boolean isHidden)
```
Sets whether the specific PivotItem in a data field is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the value of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```
Indicates whether the specified PivotTable field is autosorted ascending.
**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```
Indicates whether the specified PivotTable field is automatically sorted.
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
### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```
Indicates whether the specified PivotTable field is autosorted ascending.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```
Indicates whether the specified PivotTable field is automatically sorted.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```
Represents the PivotField display name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```
Represents the function used to summarize the PivotTable data field.
See [GridPivotFieldFunction](../../com.aspose.gridweb/gridpivotfieldfunction).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```
Represents the PivotField index in the PivotFields.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
