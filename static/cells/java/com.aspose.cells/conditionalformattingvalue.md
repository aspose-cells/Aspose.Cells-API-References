##ConditionalFormattingValue
Describes the values of the interpolation points in a gradient scale dataBar or iconSet.
**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```
Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Gets the type of this conditional formatting value object. |
| [getValue()](#getValue--) | Gets the value of this conditional formatting value object. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | Gets the Greater Than Or Equal flag. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | Sets the Greater Than Or Equal flag. |
| [setType(int value)](#setType-int-) | Sets the type of this conditional formatting value object. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Sets the value of this conditional formatting value object. |
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
### getType() {#getType--}
```
public int getType()
```
Gets the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null.
See [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).
**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```
Gets the value of this conditional formatting value object. It should be used in conjunction with Type.
**Remarks**
If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.
**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```
Gets the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.
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
### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```
Sets the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setType(int value) {#setType-int-}
```
public void setType(int value)
```
Sets the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null.
See [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```
Sets the value of this conditional formatting value object. It should be used in conjunction with Type.
**Remarks**
If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
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
