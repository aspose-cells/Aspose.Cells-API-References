##GridShape
Represents a shape object.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```
Represents a shape object.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | Gets the Buffer of object. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | Gets the Sets ID for the Shape. |
| [getLeft()](#getLeft--) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [getLeftToCorner()](#getLeftToCorner--) | Represents the horizontal offset of shape from worksheet left board, in unit of pixels. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Gets mso drawing type. |
| [getName()](#getName--) | Gets the name of the shape. |
| [getText()](#getText--) | Represents the string in this TextBox object. |
| [getTop()](#getTop--) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [getTopToCorner()](#getTopToCorner--) | Represents the vertical offset of shape from worksheet top board, in unit of pixels. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Represents upper left corner column index. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Represents upper left corner row index. |
| [getZOrderPosition()](#getZOrderPosition--) | Returns the position of a shape in the z-order. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Creates the image and saves it to a stream in the specified png format. |
| [setID(String value)](#setID-java.lang.String-) | Gets the Sets ID for the Shape. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Represents the horizontal offset of shape from worksheet left board, in unit of pixels. |
| [setText(String value)](#setText-java.lang.String-) | Represents the string in this TextBox object. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Represents the vertical offset of shape from worksheet top board, in unit of pixels. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Returns the position of a shape in the z-order. |
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
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```
Gets the Buffer of object.
**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getID() {#getID--}
```
public String getID()
```
Gets the Sets ID for the Shape.
**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```
Represents the horizontal offset of shape from its left column, in unit of pixels.
**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```
Represents the horizontal offset of shape from worksheet left board, in unit of pixels.
**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```
Gets mso drawing type.
See [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).
**Returns:**
int
### getName() {#getName--}
```
public String getName()
```
Gets the name of the shape.
**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```
Represents the string in this TextBox object.
**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```
Represents the vertical offset of shape from its top row, in unit of pixels.
**Remarks**
If the shape is in the chart, represents the vertical offset of shape from its top border.
**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```
Represents the vertical offset of shape from worksheet top board, in unit of pixels.
**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```
Represents upper left corner column index.
**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```
Represents upper left corner row index.
**Remarks**
If the shape is in the shape or in the group , UpperLeftRow will be ignored.
**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```
Returns the position of a shape in the z-order.
**Returns:**
int
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
### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```
Creates the image and saves it to a stream in the specified png format.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.io.InputStream |  |
### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```
Gets the Sets ID for the Shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```
Represents the horizontal offset of shape from worksheet left board, in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```
Represents the string in this TextBox object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```
Represents the vertical offset of shape from worksheet top board, in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```
Returns the position of a shape in the z-order.
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
