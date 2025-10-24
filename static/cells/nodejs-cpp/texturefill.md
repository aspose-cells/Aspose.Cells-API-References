##TextureFill
Encapsulates the object that represents texture fill format
## TextureFill class
Encapsulates the object that represents texture fill format
```javascript
class TextureFill;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| TextureType | Gets and sets the texture type |
| [imageData](#imageData--)| Uint8Array | Gets and sets the image data of the fill. |
| [isTiling](#isTiling--)| boolean | Indicates whether tile picture as texture. |
| [picFormatOption](#picFormatOption--)| PicFormatOption | Gets or sets picture format option. |
| [tilePicOption](#tilePicOption--)| TilePicOption | Gets or sets tile picture option. |
| [pictureFormatType](#pictureFormatType--)| FillPictureType | Gets and sets the picture format type. |
| [scale](#scale--)| number | Gets and sets the picture format scale. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the texture type |
| [setType(TextureType)](#setType-texturetype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the texture type |
| [getImageData()](#getImageData--)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets and sets the image data of the fill. |
| [setImageData(Uint8Array)](#setImageData-uint8array-)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets and sets the image data of the fill. |
| [isTiling()](#isTiling--)| <b>@deprecated.</b> Please use the 'isTiling' property instead. Indicates whether tile picture as texture. |
| [setIsTiling(boolean)](#setIsTiling-boolean-)| <b>@deprecated.</b> Please use the 'isTiling' property instead. Indicates whether tile picture as texture. |
| [getPicFormatOption()](#getPicFormatOption--)| <b>@deprecated.</b> Please use the 'picFormatOption' property instead. Gets or sets picture format option. |
| [setPicFormatOption(PicFormatOption)](#setPicFormatOption-picformatoption-)| <b>@deprecated.</b> Please use the 'picFormatOption' property instead. Gets or sets picture format option. |
| [getTilePicOption()](#getTilePicOption--)| <b>@deprecated.</b> Please use the 'tilePicOption' property instead. Gets or sets tile picture option. |
| [setTilePicOption(TilePicOption)](#setTilePicOption-tilepicoption-)| <b>@deprecated.</b> Please use the 'tilePicOption' property instead. Gets or sets tile picture option. |
| [getPictureFormatType()](#getPictureFormatType--)| <b>@deprecated.</b> Please use the 'pictureFormatType' property instead. Gets and sets the picture format type. |
| [setPictureFormatType(FillPictureType)](#setPictureFormatType-fillpicturetype-)| <b>@deprecated.</b> Please use the 'pictureFormatType' property instead. Gets and sets the picture format type. |
| [getScale()](#getScale--)| <b>@deprecated.</b> Please use the 'scale' property instead. Gets and sets the picture format scale. |
| [setScale(number)](#setScale-number-)| <b>@deprecated.</b> Please use the 'scale' property instead. Gets and sets the picture format scale. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### type {#type--}
Gets and sets the texture type
```javascript
type : TextureType;
```
### imageData {#imageData--}
Gets and sets the image data of the fill.
```javascript
imageData : Uint8Array;
```
### isTiling {#isTiling--}
Indicates whether tile picture as texture.
```javascript
isTiling : boolean;
```
### picFormatOption {#picFormatOption--}
Gets or sets picture format option.
```javascript
picFormatOption : PicFormatOption;
```
### tilePicOption {#tilePicOption--}
Gets or sets tile picture option.
```javascript
tilePicOption : TilePicOption;
```
### pictureFormatType {#pictureFormatType--}
Gets and sets the picture format type.
```javascript
pictureFormatType : FillPictureType;
```
### scale {#scale--}
Gets and sets the picture format scale.
```javascript
scale : number;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### getType() {#getType--}
```javascript
getType() : TextureType;
```
**Returns**
[TextureType](../texturetype/)
### setType(TextureType) {#setType-texturetype-}
```javascript
setType(value: TextureType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextureType](../texturetype/) | The value to set. |
### getImageData() {#getImageData--}
```javascript
getImageData() : Uint8Array;
```
### setImageData(Uint8Array) {#setImageData-uint8array-}
```javascript
setImageData(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### isTiling() {#isTiling--}
```javascript
isTiling() : boolean;
```
### setIsTiling(boolean) {#setIsTiling-boolean-}
```javascript
setIsTiling(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPicFormatOption() {#getPicFormatOption--}
```javascript
getPicFormatOption() : PicFormatOption;
```
**Returns**
[PicFormatOption](../picformatoption/)
### setPicFormatOption(PicFormatOption) {#setPicFormatOption-picformatoption-}
```javascript
setPicFormatOption(value: PicFormatOption) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PicFormatOption](../picformatoption/) | The value to set. |
### getTilePicOption() {#getTilePicOption--}
```javascript
getTilePicOption() : TilePicOption;
```
**Returns**
[TilePicOption](../tilepicoption/)
### setTilePicOption(TilePicOption) {#setTilePicOption-tilepicoption-}
```javascript
setTilePicOption(value: TilePicOption) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TilePicOption](../tilepicoption/) | The value to set. |
### getPictureFormatType() {#getPictureFormatType--}
```javascript
getPictureFormatType() : FillPictureType;
```
**Returns**
[FillPictureType](../fillpicturetype/)
### setPictureFormatType(FillPictureType) {#setPictureFormatType-fillpicturetype-}
```javascript
setPictureFormatType(value: FillPictureType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FillPictureType](../fillpicturetype/) | The value to set. |
### getScale() {#getScale--}
```javascript
getScale() : number;
```
### setScale(number) {#setScale-number-}
```javascript
setScale(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTransparency() {#getTransparency--}
```javascript
getTransparency() : number;
```
### setTransparency(number) {#setTransparency-number-}
```javascript
setTransparency(value: number) : void;
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
