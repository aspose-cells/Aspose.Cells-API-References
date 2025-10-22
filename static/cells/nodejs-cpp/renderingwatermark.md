##RenderingWatermark
Watermark for rendering.
## RenderingWatermark class
Watermark for rendering.
```javascript
class RenderingWatermark;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Uint8Array)](#constructor-uint8array-)| Creates instance of image watermark. |
| [constructor(string, RenderingFont)](#constructor-string-renderingfont-)| Creates instance of text watermark. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [rotation](#rotation--)| number | Gets or sets roation of the watermark in degrees. |
| [scaleToPagePercent](#scaleToPagePercent--)| number | Gets or sets scale relative to target page in percent. |
| [opacity](#opacity--)| number | Gets or sets opacity of the watermark in range [0, 1]. |
| [isBackground](#isBackground--)| boolean | Indicates whether the watermark is placed behind page contents. |
| [text](#text--)| string | Readonly. Gets text of the watermark. |
| [font](#font--)| RenderingFont | Readonly. Gets font of the watermark. |
| [image](#image--)| Uint8Array | Readonly. Gets image of the watermark. |
| [hAlignment](#hAlignment--)| TextAlignmentType | Gets or sets horizontal alignment of the watermark to the page. |
| [vAlignment](#vAlignment--)| TextAlignmentType | Gets or sets vertical alignment of the watermark to the page. |
| [offsetX](#offsetX--)| number | Gets or sets offset value to [HAlignment](../halignment/) |
| [offsetY](#offsetY--)| number | Gets or sets offset value to [VAlignment](../valignment/) |
## Methods
| Method | Description |
| --- | --- |
| [getRotation()](#getRotation--)| <b>@deprecated.</b> Please use the 'rotation' property instead. Gets or sets roation of the watermark in degrees. |
| [setRotation(number)](#setRotation-number-)| <b>@deprecated.</b> Please use the 'rotation' property instead. Gets or sets roation of the watermark in degrees. |
| [getScaleToPagePercent()](#getScaleToPagePercent--)| <b>@deprecated.</b> Please use the 'scaleToPagePercent' property instead. Gets or sets scale relative to target page in percent. |
| [setScaleToPagePercent(number)](#setScaleToPagePercent-number-)| <b>@deprecated.</b> Please use the 'scaleToPagePercent' property instead. Gets or sets scale relative to target page in percent. |
| [getOpacity()](#getOpacity--)| <b>@deprecated.</b> Please use the 'opacity' property instead. Gets or sets opacity of the watermark in range [0, 1]. |
| [setOpacity(number)](#setOpacity-number-)| <b>@deprecated.</b> Please use the 'opacity' property instead. Gets or sets opacity of the watermark in range [0, 1]. |
| [isBackground()](#isBackground--)| <b>@deprecated.</b> Please use the 'isBackground' property instead. Indicates whether the watermark is placed behind page contents. |
| [setIsBackground(boolean)](#setIsBackground-boolean-)| <b>@deprecated.</b> Please use the 'isBackground' property instead. Indicates whether the watermark is placed behind page contents. |
| [getText()](#getText--)| <b>@deprecated.</b> Please use the 'text' property instead. Gets text of the watermark. |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Gets font of the watermark. |
| [getImage()](#getImage--)| <b>@deprecated.</b> Please use the 'image' property instead. Gets image of the watermark. |
| [getHAlignment()](#getHAlignment--)| <b>@deprecated.</b> Please use the 'hAlignment' property instead. Gets or sets horizontal alignment of the watermark to the page. |
| [setHAlignment(TextAlignmentType)](#setHAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'hAlignment' property instead. Gets or sets horizontal alignment of the watermark to the page. |
| [getVAlignment()](#getVAlignment--)| <b>@deprecated.</b> Please use the 'vAlignment' property instead. Gets or sets vertical alignment of the watermark to the page. |
| [setVAlignment(TextAlignmentType)](#setVAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'vAlignment' property instead. Gets or sets vertical alignment of the watermark to the page. |
| [getOffsetX()](#getOffsetX--)| <b>@deprecated.</b> Please use the 'offsetX' property instead. Gets or sets offset value to [HAlignment](../halignment/) |
| [setOffsetX(number)](#setOffsetX-number-)| <b>@deprecated.</b> Please use the 'offsetX' property instead. Gets or sets offset value to [HAlignment](../halignment/) |
| [getOffsetY()](#getOffsetY--)| <b>@deprecated.</b> Please use the 'offsetY' property instead. Gets or sets offset value to [VAlignment](../valignment/) |
| [setOffsetY(number)](#setOffsetY-number-)| <b>@deprecated.</b> Please use the 'offsetY' property instead. Gets or sets offset value to [VAlignment](../valignment/) |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor(Uint8Array) {#constructor-uint8array-}
Creates instance of image watermark.
```javascript
constructor(imageData: Uint8Array);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageData | number[] |  |
### constructor(string, RenderingFont) {#constructor-string-renderingfont-}
Creates instance of text watermark.
```javascript
constructor(text: string, renderingFont: RenderingFont);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | watermark text |
| renderingFont | [RenderingFont](../renderingfont/) | watermark font |
### rotation {#rotation--}
Gets or sets roation of the watermark in degrees.
```javascript
rotation : number;
```
### scaleToPagePercent {#scaleToPagePercent--}
Gets or sets scale relative to target page in percent.
```javascript
scaleToPagePercent : number;
```
### opacity {#opacity--}
Gets or sets opacity of the watermark in range [0, 1].
```javascript
opacity : number;
```
### isBackground {#isBackground--}
Indicates whether the watermark is placed behind page contents.
```javascript
isBackground : boolean;
```
### text {#text--}
Readonly. Gets text of the watermark.
```javascript
text : string;
```
### font {#font--}
Readonly. Gets font of the watermark.
```javascript
font : RenderingFont;
```
### image {#image--}
Readonly. Gets image of the watermark.
```javascript
image : Uint8Array;
```
### hAlignment {#hAlignment--}
Gets or sets horizontal alignment of the watermark to the page.
```javascript
hAlignment : TextAlignmentType;
```
**Remarks**
Only Left, Center, Right is valid. Default is Left.
### vAlignment {#vAlignment--}
Gets or sets vertical alignment of the watermark to the page.
```javascript
vAlignment : TextAlignmentType;
```
**Remarks**
Only Top, Center, Bottom is valid. Default is Top.
### offsetX {#offsetX--}
Gets or sets offset value to [HAlignment](../halignment/)
```javascript
offsetX : number;
```
### offsetY {#offsetY--}
Gets or sets offset value to [VAlignment](../valignment/)
```javascript
offsetY : number;
```
### getRotation() {#getRotation--}
```javascript
getRotation() : number;
```
### setRotation(number) {#setRotation-number-}
```javascript
setRotation(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getScaleToPagePercent() {#getScaleToPagePercent--}
```javascript
getScaleToPagePercent() : number;
```
### setScaleToPagePercent(number) {#setScaleToPagePercent-number-}
```javascript
setScaleToPagePercent(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getOpacity() {#getOpacity--}
```javascript
getOpacity() : number;
```
### setOpacity(number) {#setOpacity-number-}
```javascript
setOpacity(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isBackground() {#isBackground--}
```javascript
isBackground() : boolean;
```
### setIsBackground(boolean) {#setIsBackground-boolean-}
```javascript
setIsBackground(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getText() {#getText--}
```javascript
getText() : string;
```
### getFont() {#getFont--}
```javascript
getFont() : RenderingFont;
```
**Returns**
[RenderingFont](../renderingfont/)
### getImage() {#getImage--}
```javascript
getImage() : Uint8Array;
```
### getHAlignment() {#getHAlignment--}
```javascript
getHAlignment() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
**Remarks**
Only Left, Center, Right is valid. Default is Left.
### setHAlignment(TextAlignmentType) {#setHAlignment-textalignmenttype-}
```javascript
setHAlignment(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
**Remarks**
Only Left, Center, Right is valid. Default is Left.
### getVAlignment() {#getVAlignment--}
```javascript
getVAlignment() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
**Remarks**
Only Top, Center, Bottom is valid. Default is Top.
### setVAlignment(TextAlignmentType) {#setVAlignment-textalignmenttype-}
```javascript
setVAlignment(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
**Remarks**
Only Top, Center, Bottom is valid. Default is Top.
### getOffsetX() {#getOffsetX--}
```javascript
getOffsetX() : number;
```
### setOffsetX(number) {#setOffsetX-number-}
```javascript
setOffsetX(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getOffsetY() {#getOffsetY--}
```javascript
getOffsetY() : number;
```
### setOffsetY(number) {#setOffsetY-number-}
```javascript
setOffsetY(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
