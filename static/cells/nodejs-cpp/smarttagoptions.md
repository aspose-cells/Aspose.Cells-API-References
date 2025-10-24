##SmartTagOptions
Represents the options of the smart tag.
## SmartTagOptions class
Represents the options of the smart tag.
```javascript
class SmartTagOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [embedSmartTags](#embedSmartTags--)| boolean | Indicates whether saving smart tags with the workbook. |
| [showType](#showType--)| SmartTagShowType | Represents the show type of smart tag. |
## Methods
| Method | Description |
| --- | --- |
| [getEmbedSmartTags()](#getEmbedSmartTags--)| <b>@deprecated.</b> Please use the 'embedSmartTags' property instead. Indicates whether saving smart tags with the workbook. |
| [setEmbedSmartTags(boolean)](#setEmbedSmartTags-boolean-)| <b>@deprecated.</b> Please use the 'embedSmartTags' property instead. Indicates whether saving smart tags with the workbook. |
| [getShowType()](#getShowType--)| <b>@deprecated.</b> Please use the 'showType' property instead. Represents the show type of smart tag. |
| [setShowType(SmartTagShowType)](#setShowType-smarttagshowtype-)| <b>@deprecated.</b> Please use the 'showType' property instead. Represents the show type of smart tag. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### embedSmartTags {#embedSmartTags--}
Indicates whether saving smart tags with the workbook.
```javascript
embedSmartTags : boolean;
```
### showType {#showType--}
Represents the show type of smart tag.
```javascript
showType : SmartTagShowType;
```
### getEmbedSmartTags() {#getEmbedSmartTags--}
```javascript
getEmbedSmartTags() : boolean;
```
### setEmbedSmartTags(boolean) {#setEmbedSmartTags-boolean-}
```javascript
setEmbedSmartTags(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowType() {#getShowType--}
```javascript
getShowType() : SmartTagShowType;
```
**Returns**
[SmartTagShowType](../smarttagshowtype/)
### setShowType(SmartTagShowType) {#setShowType-smarttagshowtype-}
```javascript
setShowType(value: SmartTagShowType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SmartTagShowType](../smarttagshowtype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
