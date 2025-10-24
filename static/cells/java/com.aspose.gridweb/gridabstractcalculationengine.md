##GridAbstractCalculationEngine
Represents users custom calculation engine to extend the default calculation engine of Aspose.Cells.
**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```
Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.
**Example**
```
class MyEngine extends GridAbstractCalculationEngine
{
public /*override*/ void calculate(GridCalculationData data)
{
String funcName = data.getFunctionName().toUpperCase();
if ("MYFUNC".equals(funcName))
{
//do calculation for MYFUNC here
int count = data.getParamCount();
Object res = null;
for (int i = 0; i <count; i++)
{
Object pv = data.getParamValue(i);
if (pv instanceof GridReferredArea)
{
GridReferredArea ra = (GridReferredArea)pv;
pv = ra.getValue(0, 0);
}
//process the parameter here
//res = ...;
}
data.setCalculatedValue(res);
}
}
}
```
## Constructors
| Constructor | Description |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## Methods
| Method | Description |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridweb.GridCalculationData-) | Calculates one function with given data. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridAbstractCalculationEngine() {#GridAbstractCalculationEngine--}
```
public GridAbstractCalculationEngine()
```
### calculate(GridCalculationData data) {#calculate-com.aspose.gridweb.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```
Calculates one function with given data.
**Remarks**
User should set the calculated value for given data for all functions(including excel native functions) that he wants to calculate by himself in this implementation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridweb/gridcalculationdata) | the required data to calculate function such as function name, parameters, ...etc. |
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
