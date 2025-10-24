##ChartSplitType
Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.
**Inheritance:**
java.lang.Object
```
public final class ChartSplitType
```
Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.
## Fields
| Field | Description |
| --- | --- |
| [AUTO](#AUTO) | Represents the data points shall be split using the default mechanism for this chart type. |
| [CUSTOM](#CUSTOM) | Represents the data points shall be split between the pie and the second chart according to the Custom Split values. |
| [PERCENT_VALUE](#PERCENT-VALUE) | Represents the data points shall be split between the pie and the second chart by putting the points with percentage less than Split Position percent in the second chart. |
| [POSITION](#POSITION) | Represents the data points shall be split between the pie and the second chart by putting the last Split Position of the data points in the second chart |
| [VALUE](#VALUE) | Represents the data points shall be split between the pie and the second chart by putting the data points with value less than Split Position in the second chart. |
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
### AUTO {#AUTO}
```
public static final int AUTO
```
Represents the data points shall be split using the default mechanism for this chart type.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Series.IsAutoSplit property. This property will be removed 12 months later since September 2023. Aspose apologizes for any inconvenience you may have experienced.
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```
Represents the data points shall be split between the pie and the second chart according to the Custom Split values.
### PERCENT_VALUE {#PERCENT-VALUE}
```
public static final int PERCENT_VALUE
```
Represents the data points shall be split between the pie and the second chart by putting the points with percentage less than Split Position percent in the second chart.
### POSITION {#POSITION}
```
public static final int POSITION
```
Represents the data points shall be split between the pie and the second chart by putting the last Split Position of the data points in the second chart
### VALUE {#VALUE}
```
public static final int VALUE
```
Represents the data points shall be split between the pie and the second chart by putting the data points with value less than Split Position in the second chart.
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
