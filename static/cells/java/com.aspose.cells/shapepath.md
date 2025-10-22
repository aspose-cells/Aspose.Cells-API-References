##ShapePath
Represents a creation path consisting of a series of moves lines and curves that when combined will form a geometric shape.
**Inheritance:**
java.lang.Object
```
public class ShapePath
```
Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.
## Constructors
| Constructor | Description |
| --- | --- |
| [ShapePath()](#ShapePath--) | Initializes a new instance of the [ShapePath](../../com.aspose.cells/shapepath) class. |
## Methods
| Method | Description |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | Appends an elliptical arc to the current figure. |
| [close()](#close--) | Closes the current figure and starts a new figure. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | Appends a cubic B\\u8305zier curve to the current figure. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Gets the height of this path in unit of pixels. |
| [getPathSegementList()](#getPathSegementList--) | Gets [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) list |
| [getWidthPixel()](#getWidthPixel--) | Gets the width of this path in unit of pixels. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | Appends a line segment to the current figure. |
| [moveTo(float x, float y)](#moveTo-float-float-) | Starts a new figure from the specified point without closing the current figure. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Gets the height of this path in unit of pixels. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Gets the width of this path in unit of pixels. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```
Initializes a new instance of the [ShapePath](../../com.aspose.cells/shapepath) class.
### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```
Appends an elliptical arc to the current figure. The starting point is the end point of the current figure.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| wR | float | The half-width of the rectangular area of \\u9225\\u5b27\\u20ac\\u5aa1he ellipse that draws the arc(Unit: Pixel). |
| hR | float | The half-height of the rectangular area of \\u9225\\u5b27\\u20ac\\u5aa1he ellipse that draws the arc(Unit: Pixel). |
| stAng | float | The starting angle of the arc, measured in degrees clockwise from the x-axis(Unit: Degree). This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path. |
| swAng | float | The swing angle for an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.(Unit: Degree) |
### close() {#close--}
```
public void close()
```
Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point.
### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```
Appends a cubic B\\u8305zier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ctrX1 | float | The x-coordinate of the first control point for the curve(Unit: Pixel). |
| ctrY1 | float | The y-coordinate of the first control point for the curve(Unit: Pixel). |
| ctrX2 | float | The x-coordinate of the second control point for the curve(Unit: Pixel). |
| ctrY2 | float | The y-coordinate of the second control point for the curve(Unit: Pixel). |
| endX | float | The x-coordinate of the endpoint of the curve(Unit: Pixel). |
| endY | float | The y-coordinate of the endpoint of the curve(Unit: Pixel). |
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
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```
Gets the height of this path in unit of pixels.
**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```
Gets [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) list
**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```
Gets the width of this path in unit of pixels.
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### lineTo(float x, float y) {#lineTo-float-float-}
```
public void lineTo(float x, float y)
```
Appends a line segment to the current figure. The starting point is the end point of the current figure.Unit: Pixel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| x | float | The x-coordinate of the endpoint of the line segment(Unit: Pixel). |
| y | float | The y-coordinate of the endpoint of the line segment(Unit: Pixel). |
### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```
Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit: Pixel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| x | float | The x-coordinate of the starting point of the figure(Unit: Pixel). |
| y | float | The y-coordinate of the starting point of the figure(Unit: Pixel). |
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```
Gets the height of this path in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```
Gets the width of this path in unit of pixels.
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
