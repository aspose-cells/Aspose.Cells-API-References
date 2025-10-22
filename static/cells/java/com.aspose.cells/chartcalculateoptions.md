##ChartCalculateOptions
Represents the options for calculating chart.
**Inheritance:**
java.lang.Object
```
public class ChartCalculateOptions
```
Represents the options for calculating chart.
## Constructors
| Constructor | Description |
| --- | --- |
| [ChartCalculateOptions()](#ChartCalculateOptions--) | Creates the options for calculating chart. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getUpdateAllPoints()](#getUpdateAllPoints--) | Whether update all data points when performing the chart calculation. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setUpdateAllPoints(boolean value)](#setUpdateAllPoints-boolean-) | Whether update all data points when performing the chart calculation. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ChartCalculateOptions() {#ChartCalculateOptions--}
```
public ChartCalculateOptions()
```
Creates the options for calculating chart.
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
### getUpdateAllPoints() {#getUpdateAllPoints--}
```
public boolean getUpdateAllPoints()
```
Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.
**Returns:**
boolean
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
### setUpdateAllPoints(boolean value) {#setUpdateAllPoints-boolean-}
```
public void setUpdateAllPoints(boolean value)
```
Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
