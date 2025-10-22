##RenderingWatermark
Watermark for rendering.
**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```
Watermark for rendering.
## Constructors
| Constructor | Description |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | Creates instance of text watermark. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | Creates instance of image watermark. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Gets font of the watermark. |
| [getHAlignment()](#getHAlignment--) | Gets horizontal alignment of the watermark to the page. |
| [getImage()](#getImage--) | Gets image of the watermark. |
| [getOffsetX()](#getOffsetX--) | Gets offset value to [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | Gets offset value to [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | Gets opacity of the watermark in range [0, 1]. |
| [getRotation()](#getRotation--) | Gets roation of the watermark in degrees. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | Gets scale relative to target page in percent. |
| [getText()](#getText--) | Gets text of the watermark. |
| [getVAlignment()](#getVAlignment--) | Gets vertical alignment of the watermark to the page. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | Indicates whether the watermark is placed behind page contents. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | Indicates whether the watermark is placed behind page contents. |
| [setHAlignment(int value)](#setHAlignment-int-) | Sets horizontal alignment of the watermark to the page. |
| [setOffsetX(float value)](#setOffsetX-float-) | Sets offset value to [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | Sets offset value to [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | Sets opacity of the watermark in range [0, 1]. |
| [setRotation(float value)](#setRotation-float-) | Sets roation of the watermark in degrees. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | Sets scale relative to target page in percent. |
| [setVAlignment(int value)](#setVAlignment-int-) | Sets vertical alignment of the watermark to the page. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```
Creates instance of text watermark.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | watermark text |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | watermark font |
### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```
Creates instance of image watermark.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageData | byte[] |  |
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
### getFont() {#getFont--}
```
public RenderingFont getFont()
```
Gets font of the watermark.
**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```
Gets horizontal alignment of the watermark to the page.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Remarks**
Only Left, Center, Right is valid. Default is Left.
**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```
Gets image of the watermark.
**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```
Gets offset value to [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)
**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```
Gets offset value to [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)
**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```
Gets opacity of the watermark in range [0, 1].
**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```
Gets roation of the watermark in degrees.
**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```
Gets scale relative to target page in percent.
**Returns:**
int
### getText() {#getText--}
```
public String getText()
```
Gets text of the watermark.
**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```
Gets vertical alignment of the watermark to the page.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Remarks**
Only Top, Center, Bottom is valid. Default is Top.
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isBackground() {#isBackground--}
```
public boolean isBackground()
```
Indicates whether the watermark is placed behind page contents.
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
### setBackground(boolean value) {#setBackground-boolean-}
```
public void setBackground(boolean value)
```
Indicates whether the watermark is placed behind page contents.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```
Sets horizontal alignment of the watermark to the page.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Remarks**
Only Left, Center, Right is valid. Default is Left.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```
Sets offset value to [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |
### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```
Sets offset value to [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |
### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```
Sets opacity of the watermark in range [0, 1].
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |
### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```
Sets roation of the watermark in degrees.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |
### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```
Sets scale relative to target page in percent.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```
Sets vertical alignment of the watermark to the page.
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Remarks**
Only Top, Center, Bottom is valid. Default is Top.
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
