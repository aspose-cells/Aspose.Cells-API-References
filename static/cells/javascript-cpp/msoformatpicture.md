##MsoFormatPicture
Represents the picture format.
## MsoFormatPicture class
Represents the picture format.
```javascript
class MsoFormatPicture;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [topCropInch](#topCropInch--)| number | Represents the location of the top of the crop rectangle expressed, in unit of inches. |
| [bottomCropInch](#bottomCropInch--)| number | Represents the location of the bottom of the crop rectangle expressed, in unit of inches. |
| [leftCropInch](#leftCropInch--)| number | Represents the location of the left of the crop rectangle expressed, in unit of inches. |
| [rightCropInch](#rightCropInch--)| number | Represents the location of the right of the crop rectangle expressed, in unit of inches. |
| [topCrop](#topCrop--)| number | Represents the location of the top of the crop rectangle expressed, expressed as a ratio of the image's height. |
| [bottomCrop](#bottomCrop--)| number | Represents the location of the bottom of the crop rectangle expressed, expressed as a ratio of the image's height. |
| [leftCrop](#leftCrop--)| number | Represents the location of the left of the crop rectangle expressed, expressed as a ratio of the image's width. |
| [rightCrop](#rightCrop--)| number | Represents the location of the right of the crop rectangle expressed, expressed as a ratio of the image's width. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [transparentColor](#transparentColor--)| CellsColor | Gets and sets the transparent color of the picture. |
| [contrast](#contrast--)| number | Represents the contrast modification for the picture.in unit of percentage. |
| [brightness](#brightness--)| number | Represents the brightness modification for the picture in unit of percentage. |
| [gamma](#gamma--)| number | Represents gamma of the picture. |
| [isBiLevel](#isBiLevel--)| boolean | Indicates whether this picture should display in two-color black and white. |
| [isGray](#isGray--)| boolean | Indicates whether this picture should display in grayscale. |
## Methods
| Method | Description |
| --- | --- |
| [getHashCode()](#getHashCode--)| Gets the hash code. |
| [equals(VObject)](#equals-vobject-)|  |
### topCropInch {#topCropInch--}
Represents the location of the top of the crop rectangle expressed, in unit of inches.
```javascript
topCropInch : number;
```
### bottomCropInch {#bottomCropInch--}
Represents the location of the bottom of the crop rectangle expressed, in unit of inches.
```javascript
bottomCropInch : number;
```
### leftCropInch {#leftCropInch--}
Represents the location of the left of the crop rectangle expressed, in unit of inches.
```javascript
leftCropInch : number;
```
### rightCropInch {#rightCropInch--}
Represents the location of the right of the crop rectangle expressed, in unit of inches.
```javascript
rightCropInch : number;
```
### topCrop {#topCrop--}
Represents the location of the top of the crop rectangle expressed, expressed as a ratio of the image's height.
```javascript
topCrop : number;
```
### bottomCrop {#bottomCrop--}
Represents the location of the bottom of the crop rectangle expressed, expressed as a ratio of the image's height.
```javascript
bottomCrop : number;
```
### leftCrop {#leftCrop--}
Represents the location of the left of the crop rectangle expressed, expressed as a ratio of the image's width.
```javascript
leftCrop : number;
```
### rightCrop {#rightCrop--}
Represents the location of the right of the crop rectangle expressed, expressed as a ratio of the image's width.
```javascript
rightCrop : number;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### transparentColor {#transparentColor--}
Gets and sets the transparent color of the picture.
```javascript
transparentColor : CellsColor;
```
### contrast {#contrast--}
Represents the contrast modification for the picture.in unit of percentage.
```javascript
contrast : number;
```
**Remarks**
It is between -100% and 100%. It works same as Excel 2007 or above version.
### brightness {#brightness--}
Represents the brightness modification for the picture in unit of percentage.
```javascript
brightness : number;
```
**Remarks**
It is between -100% and 100%. It works same as Excel 2007 or above version.
### gamma {#gamma--}
Represents gamma of the picture.
```javascript
gamma : number;
```
### isBiLevel {#isBiLevel--}
Indicates whether this picture should display in two-color black and white.
```javascript
isBiLevel : boolean;
```
### isGray {#isGray--}
Indicates whether this picture should display in grayscale.
```javascript
isGray : boolean;
```
### getHashCode() {#getHashCode--}
Gets the hash code.
```javascript
getHashCode() : number;
```
### equals(VObject) {#equals-vobject-}
```javascript
equals(obj: VObject) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | VObject |  |
