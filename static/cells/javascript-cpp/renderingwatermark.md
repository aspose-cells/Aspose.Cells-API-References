##RenderingWatermark
Watermark for rendering.
## RenderingWatermark class
Watermark for rendering.
```javascript
class RenderingWatermark;
```
## Constructors
| Name | Description |
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
