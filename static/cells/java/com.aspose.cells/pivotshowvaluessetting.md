##PivotShowValuesSetting
Represents the settings about showing values as when the ShowDataAs calculation is in use.
**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```
Represents the settings about showing values as when the ShowDataAs calculation is in use.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. |
| [getCalculationType()](#getCalculationType--) | Represents how to show values of a data field in the pivot report. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. |
| [setCalculationType(int value)](#setCalculationType-int-) | Represents how to show values of a data field in the pivot report. |
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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```
Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.
**Returns:**
int
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```
Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields.
**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```
Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.
See [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).
**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```
Represents how to show values of a data field in the pivot report.
See [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).
**Returns:**
int
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
### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```
Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```
Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```
Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.
See [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```
Represents how to show values of a data field in the pivot report.
See [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).
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
