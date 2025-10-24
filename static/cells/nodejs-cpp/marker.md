##Marker
Represents the marker in a line chart scatter chart or radar chart.
## Marker class
Represents the marker in a line chart, scatter chart, or radar chart.
```javascript
class Marker;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [border](#border--)| Line | Readonly. Gets the <see cref="Line">border</see>. |
| [area](#area--)| Area | Readonly. Gets the <see cref="Area">area</see>. |
| [markerStyle](#markerStyle--)| ChartMarkerType | Represents the marker style. Applies to line chart, scatter chart, or radar chart. |
| [markerSize](#markerSize--)| number | Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart. |
| [markerSizePx](#markerSizePx--)| number | Represents the marker size in unit of pixels. Applies to line chart, scatter chart, or radar chart. |
| [foregroundColor](#foregroundColor--)| Color | Represents the marker foreground color in a line chart, scatter chart, or radar chart. |
| [foregroundColorSetType](#foregroundColorSetType--)| FormattingType | Gets or sets the marker foreground color set type. |
| [backgroundColor](#backgroundColor--)| Color | Represents the marker background color in a line chart, scatter chart, or radar chart. |
| [backgroundColorSetType](#backgroundColorSetType--)| FormattingType | Gets or sets the marker background color set type. |
## Methods
| Method | Description |
| --- | --- |
| [getBorder()](#getBorder--)| <b>@deprecated.</b> Please use the 'border' property instead. Gets the <see cref="Line">border</see>. |
| [getArea()](#getArea--)| <b>@deprecated.</b> Please use the 'area' property instead. Gets the <see cref="Area">area</see>. |
| [getMarkerStyle()](#getMarkerStyle--)| <b>@deprecated.</b> Please use the 'markerStyle' property instead. Represents the marker style. Applies to line chart, scatter chart, or radar chart. |
| [setMarkerStyle(ChartMarkerType)](#setMarkerStyle-chartmarkertype-)| <b>@deprecated.</b> Please use the 'markerStyle' property instead. Represents the marker style. Applies to line chart, scatter chart, or radar chart. |
| [getMarkerSize()](#getMarkerSize--)| <b>@deprecated.</b> Please use the 'markerSize' property instead. Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart. |
| [setMarkerSize(number)](#setMarkerSize-number-)| <b>@deprecated.</b> Please use the 'markerSize' property instead. Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart. |
| [getMarkerSizePx()](#getMarkerSizePx--)| <b>@deprecated.</b> Please use the 'markerSizePx' property instead. Represents the marker size in unit of pixels. Applies to line chart, scatter chart, or radar chart. |
| [setMarkerSizePx(number)](#setMarkerSizePx-number-)| <b>@deprecated.</b> Please use the 'markerSizePx' property instead. Represents the marker size in unit of pixels. Applies to line chart, scatter chart, or radar chart. |
| [getForegroundColor()](#getForegroundColor--)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Represents the marker foreground color in a line chart, scatter chart, or radar chart. |
| [setForegroundColor(Color)](#setForegroundColor-color-)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Represents the marker foreground color in a line chart, scatter chart, or radar chart. |
| [getForegroundColorSetType()](#getForegroundColorSetType--)| <b>@deprecated.</b> Please use the 'foregroundColorSetType' property instead. Gets or sets the marker foreground color set type. |
| [setForegroundColorSetType(FormattingType)](#setForegroundColorSetType-formattingtype-)| <b>@deprecated.</b> Please use the 'foregroundColorSetType' property instead. Gets or sets the marker foreground color set type. |
| [getBackgroundColor()](#getBackgroundColor--)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Represents the marker background color in a line chart, scatter chart, or radar chart. |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Represents the marker background color in a line chart, scatter chart, or radar chart. |
| [getBackgroundColorSetType()](#getBackgroundColorSetType--)| <b>@deprecated.</b> Please use the 'backgroundColorSetType' property instead. Gets or sets the marker background color set type. |
| [setBackgroundColorSetType(FormattingType)](#setBackgroundColorSetType-formattingtype-)| <b>@deprecated.</b> Please use the 'backgroundColorSetType' property instead. Gets or sets the marker background color set type. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### border {#border--}
Readonly. Gets the <see cref="Line">border</see>.
```javascript
border : Line;
```
### area {#area--}
Readonly. Gets the <see cref="Area">area</see>.
```javascript
area : Area;
```
### markerStyle {#markerStyle--}
Represents the marker style. Applies to line chart, scatter chart, or radar chart.
```javascript
markerStyle : ChartMarkerType;
```
### markerSize {#markerSize--}
Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart.
```javascript
markerSize : number;
```
### markerSizePx {#markerSizePx--}
Represents the marker size in unit of pixels. Applies to line chart, scatter chart, or radar chart.
```javascript
markerSizePx : number;
```
### foregroundColor {#foregroundColor--}
Represents the marker foreground color in a line chart, scatter chart, or radar chart.
```javascript
foregroundColor : Color;
```
### foregroundColorSetType {#foregroundColorSetType--}
Gets or sets the marker foreground color set type.
```javascript
foregroundColorSetType : FormattingType;
```
### backgroundColor {#backgroundColor--}
Represents the marker background color in a line chart, scatter chart, or radar chart.
```javascript
backgroundColor : Color;
```
### backgroundColorSetType {#backgroundColorSetType--}
Gets or sets the marker background color set type.
```javascript
backgroundColorSetType : FormattingType;
```
### getBorder() {#getBorder--}
```javascript
getBorder() : Line;
```
**Returns**
[Line](../line/)
### getArea() {#getArea--}
```javascript
getArea() : Area;
```
**Returns**
[Area](../area/)
### getMarkerStyle() {#getMarkerStyle--}
```javascript
getMarkerStyle() : ChartMarkerType;
```
**Returns**
[ChartMarkerType](../chartmarkertype/)
### setMarkerStyle(ChartMarkerType) {#setMarkerStyle-chartmarkertype-}
```javascript
setMarkerStyle(value: ChartMarkerType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartMarkerType](../chartmarkertype/) | The value to set. |
### getMarkerSize() {#getMarkerSize--}
```javascript
getMarkerSize() : number;
```
### setMarkerSize(number) {#setMarkerSize-number-}
```javascript
setMarkerSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getMarkerSizePx() {#getMarkerSizePx--}
```javascript
getMarkerSizePx() : number;
```
### setMarkerSizePx(number) {#setMarkerSizePx-number-}
```javascript
setMarkerSizePx(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getForegroundColor() {#getForegroundColor--}
```javascript
getForegroundColor() : Color;
```
**Returns**
[Color](../color/)
### setForegroundColor(Color) {#setForegroundColor-color-}
```javascript
setForegroundColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getForegroundColorSetType() {#getForegroundColorSetType--}
```javascript
getForegroundColorSetType() : FormattingType;
```
**Returns**
[FormattingType](../formattingtype/)
### setForegroundColorSetType(FormattingType) {#setForegroundColorSetType-formattingtype-}
```javascript
setForegroundColorSetType(value: FormattingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |
### getBackgroundColor() {#getBackgroundColor--}
```javascript
getBackgroundColor() : Color;
```
**Returns**
[Color](../color/)
### setBackgroundColor(Color) {#setBackgroundColor-color-}
```javascript
setBackgroundColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getBackgroundColorSetType() {#getBackgroundColorSetType--}
```javascript
getBackgroundColorSetType() : FormattingType;
```
**Returns**
[FormattingType](../formattingtype/)
### setBackgroundColorSetType(FormattingType) {#setBackgroundColorSetType-formattingtype-}
```javascript
setBackgroundColorSetType(value: FormattingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
