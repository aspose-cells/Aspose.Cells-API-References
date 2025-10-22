##LegendEntry
Represents a legend entry in a chart legend.
## LegendEntry class
Represents a legend entry in a chart legend.
```javascript
class LegendEntry;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isDeleted](#isDeleted--)| boolean | Gets and sets whether the legend entry is deleted. |
| [font](#font--)| Font | Readonly. Gets a [Font](../font/) object of the specified ChartFrame object. |
| [isTextNoFill](#isTextNoFill--)| boolean | Gets or sets no fill of the text. |
| [autoScaleFont](#autoScaleFont--)| boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [backgroundMode](#backgroundMode--)| BackgroundMode | Gets and sets the display mode of the background |
## Methods
| Method | Description |
| --- | --- |
| [isDeleted()](#isDeleted--)| <b>@deprecated.</b> Please use the 'isDeleted' property instead. Gets and sets whether the legend entry is deleted. |
| [setIsDeleted(boolean)](#setIsDeleted-boolean-)| <b>@deprecated.</b> Please use the 'isDeleted' property instead. Gets and sets whether the legend entry is deleted. |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Gets a [Font](../font/) object of the specified ChartFrame object. |
| [isTextNoFill()](#isTextNoFill--)| <b>@deprecated.</b> Please use the 'isTextNoFill' property instead. Gets or sets no fill of the text. |
| [setIsTextNoFill(boolean)](#setIsTextNoFill-boolean-)| <b>@deprecated.</b> Please use the 'isTextNoFill' property instead. Gets or sets no fill of the text. |
| [getAutoScaleFont()](#getAutoScaleFont--)| <b>@deprecated.</b> Please use the 'autoScaleFont' property instead. True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| <b>@deprecated.</b> Please use the 'autoScaleFont' property instead. True if the text in the object changes font size when the object size changes. The default value is True. |
| [getBackgroundMode()](#getBackgroundMode--)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### isDeleted {#isDeleted--}
Gets and sets whether the legend entry is deleted.
```javascript
isDeleted : boolean;
```
### font {#font--}
Readonly. Gets a [Font](../font/) object of the specified ChartFrame object.
```javascript
font : Font;
```
### isTextNoFill {#isTextNoFill--}
Gets or sets no fill of the text.
```javascript
isTextNoFill : boolean;
```
### autoScaleFont {#autoScaleFont--}
True if the text in the object changes font size when the object size changes. The default value is True.
```javascript
autoScaleFont : boolean;
```
### backgroundMode {#backgroundMode--}
Gets and sets the display mode of the background
```javascript
backgroundMode : BackgroundMode;
```
### isDeleted() {#isDeleted--}
```javascript
isDeleted() : boolean;
```
### setIsDeleted(boolean) {#setIsDeleted-boolean-}
```javascript
setIsDeleted(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFont() {#getFont--}
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### isTextNoFill() {#isTextNoFill--}
```javascript
isTextNoFill() : boolean;
```
### setIsTextNoFill(boolean) {#setIsTextNoFill-boolean-}
```javascript
setIsTextNoFill(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAutoScaleFont() {#getAutoScaleFont--}
```javascript
getAutoScaleFont() : boolean;
```
### setAutoScaleFont(boolean) {#setAutoScaleFont-boolean-}
```javascript
setAutoScaleFont(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getBackgroundMode() {#getBackgroundMode--}
```javascript
getBackgroundMode() : BackgroundMode;
```
**Returns**
[BackgroundMode](../backgroundmode/)
### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}
```javascript
setBackgroundMode(value: BackgroundMode) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](../backgroundmode/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
