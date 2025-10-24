##ActiveXControlBase
Represents the ActiveX control.
**Inheritance:**
java.lang.Object
```
public abstract class ActiveXControlBase
```
Represents the ActiveX control.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Gets the ole color of the background. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Gets the binary data of the control. |
| [getForeOleColor()](#getForeOleColor--) | Gets the ole color of the foreground. |
| [getHeight()](#getHeight--) | Gets the height of the control in unit of points. |
| [getLinkedCell()](#getLinkedCell--) | Gets the linked cell. |
| [getListFillRange()](#getListFillRange--) | Gets the list fill range. |
| [getMouseIcon()](#getMouseIcon--) | Gets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getMousePointer--) | Gets the type of icon displayed as the mouse pointer for the control. |
| [getShadow()](#getShadow--) | Indicates whether to show a shadow. |
| [getType()](#getType--) | Gets the type of the ActiveX control. |
| [getWidth()](#getWidth--) | Gets the width of the control in unit of points. |
| [getWorkbook()](#getWorkbook--) | Gets the [Workbook](../../com.aspose.cells/workbook) object. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Indicates whether this control is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Sets the ole color of the background. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Sets the ole color of the foreground. |
| [setHeight(double value)](#setHeight-double-) | Sets the height of the control in unit of points. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Sets the linked cell. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Sets the list fill range. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Sets a custom icon to display as the mouse pointer for the control. |
| [setMousePointer(int value)](#setMousePointer-int-) | Sets the type of icon displayed as the mouse pointer for the control. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indicates whether to show a shadow. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indicates whether this control is visible. |
| [setWidth(double value)](#setWidth-double-) | Sets the width of the control in unit of points. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```
Gets the ole color of the background.
**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```
Gets the binary data of the control.
**Returns:**
byte[]
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```
Gets the ole color of the foreground.
**Remarks**
Not applies to Image control.
**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```
Gets the height of the control in unit of points.
**Returns:**
double
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```
Gets the linked cell.
**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```
Gets the list fill range.
**Returns:**
java.lang.String
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```
Gets a custom icon to display as the mouse pointer for the control.
**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```
Gets the type of icon displayed as the mouse pointer for the control.
See [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).
**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```
Indicates whether to show a shadow.
**Returns:**
boolean
### getType() {#getType--}
```
public abstract int getType()
```
Gets the type of the ActiveX control.
See [ControlType](../../com.aspose.cells/controltype).
**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```
Gets the width of the control in unit of points.
**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```
Gets the [Workbook](../../com.aspose.cells/workbook) object.
**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```
Indicates whether this control is visible.
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
### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```
Sets the ole color of the background.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```
Sets the ole color of the foreground.
**Remarks**
Not applies to Image control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```
Sets the height of the control in unit of points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```
Sets the linked cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```
Sets the list fill range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```
Sets a custom icon to display as the mouse pointer for the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |
### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```
Sets the type of icon displayed as the mouse pointer for the control.
See [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```
Indicates whether to show a shadow.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```
Indicates whether this control is visible.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```
Sets the width of the control in unit of points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
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
