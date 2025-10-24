##ShapePathPoint
Specify position coordinates or angle markers.
**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```
Specify position coordinates or angle markers. Position coordinates represent the coordinates of a path in a coordinate space (e.g. X/Y). Angle markers indicate angular changes in a path (e.g. the start and swing angles of an arc).
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Specifies the value type of the current object. |
| [getX()](#getX--) | Gets x coordinate for this position coordinate. |
| [getXAngle()](#getXAngle--) | When the object is an angle marker, get or set the first angle in degrees. |
| [getXPixel()](#getXPixel--) | When the object is a position coordinate, get or set the x coordinate in pixels. |
| [getY()](#getY--) | Gets y coordinate for this position coordinate. |
| [getYAngle()](#getYAngle--) | When the object is an angle marker, get or set the second angle in degrees. |
| [getYPixel()](#getYPixel--) | When the object is a position coordinate, get or set the y coordinate in pixels. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | Sets x coordinate for this position coordinate. |
| [setXAngle(int value)](#setXAngle-int-) | When the object is an angle marker, get or set the first angle in degrees. |
| [setXPixel(int value)](#setXPixel-int-) | When the object is a position coordinate, get or set the x coordinate in pixels. |
| [setY(int value)](#setY-int-) | Gets y coordinate for this position coordinate. |
| [setYAngle(int value)](#setYAngle-int-) | When the object is an angle marker, get or set the second angle in degrees. |
| [setYPixel(int value)](#setYPixel-int-) | When the object is a position coordinate, get or set the y coordinate in pixels. |
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
Specifies the value type of the current object.
See [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype).
**Returns:**
int
### getX() {#getX--}
```
public int getX()
```
Gets x coordinate for this position coordinate. Unit EMUs.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```
When the object is an angle marker, get or set the first angle in degrees.
**Remarks**
If this angle is the starting angle of an arc. This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path.
**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```
When the object is a position coordinate, get or set the x coordinate in pixels.
**Returns:**
int
### getY() {#getY--}
```
public int getY()
```
Gets y coordinate for this position coordinate. Unit EMUs.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```
When the object is an angle marker, get or set the second angle in degrees.
**Remarks**
If this angle is the swing angle of an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.
**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```
When the object is a position coordinate, get or set the y coordinate in pixels.
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
### setX(int value) {#setX-int-}
```
public void setX(int value)
```
Sets x coordinate for this position coordinate. Unit EMUs.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```
When the object is an angle marker, get or set the first angle in degrees.
**Remarks**
If this angle is the starting angle of an arc. This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```
When the object is a position coordinate, get or set the x coordinate in pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setY(int value) {#setY-int-}
```
public void setY(int value)
```
Gets y coordinate for this position coordinate. Unit EMUs.
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```
When the object is an angle marker, get or set the second angle in degrees.
**Remarks**
If this angle is the swing angle of an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```
When the object is a position coordinate, get or set the y coordinate in pixels.
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
