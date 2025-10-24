##OdsPageBackground
Represents the page background of ods.
## OdsPageBackground class
Represents the page background of ods.
```javascript
class OdsPageBackground;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| OdsPageBackgroundType | Gets and sets the page background type. |
| [color](#color--)| Color | Gets and sets the color of background. |
| [graphicType](#graphicType--)| OdsPageBackgroundGraphicType | Gets and sets the page background graphic type. |
| [graphicPositionType](#graphicPositionType--)| OdsPageBackgroundGraphicPositionType | Gets and set the background graphic position. |
| [isLink](#isLink--)| boolean | Readonly. Indicates whether it's a linked graphic. |
| [linkedGraphic](#linkedGraphic--)| string | Gets and sets the linked graphic path. |
| [graphicData](#graphicData--)| Uint8Array | Gets and sets the graphic data. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the page background type. |
| [setType(OdsPageBackgroundType)](#setType-odspagebackgroundtype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the page background type. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets and sets the color of background. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets and sets the color of background. |
| [getGraphicType()](#getGraphicType--)| <b>@deprecated.</b> Please use the 'graphicType' property instead. Gets and sets the page background graphic type. |
| [setGraphicType(OdsPageBackgroundGraphicType)](#setGraphicType-odspagebackgroundgraphictype-)| <b>@deprecated.</b> Please use the 'graphicType' property instead. Gets and sets the page background graphic type. |
| [getGraphicPositionType()](#getGraphicPositionType--)| <b>@deprecated.</b> Please use the 'graphicPositionType' property instead. Gets and set the background graphic position. |
| [setGraphicPositionType(OdsPageBackgroundGraphicPositionType)](#setGraphicPositionType-odspagebackgroundgraphicpositiontype-)| <b>@deprecated.</b> Please use the 'graphicPositionType' property instead. Gets and set the background graphic position. |
| [isLink()](#isLink--)| <b>@deprecated.</b> Please use the 'isLink' property instead. Indicates whether it's a linked graphic. |
| [getLinkedGraphic()](#getLinkedGraphic--)| <b>@deprecated.</b> Please use the 'linkedGraphic' property instead. Gets and sets the linked graphic path. |
| [setLinkedGraphic(string)](#setLinkedGraphic-string-)| <b>@deprecated.</b> Please use the 'linkedGraphic' property instead. Gets and sets the linked graphic path. |
| [getGraphicData()](#getGraphicData--)| <b>@deprecated.</b> Please use the 'graphicData' property instead. Gets and sets the graphic data. |
| [setGraphicData(Uint8Array)](#setGraphicData-uint8array-)| <b>@deprecated.</b> Please use the 'graphicData' property instead. Gets and sets the graphic data. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### type {#type--}
Gets and sets the page background type.
```javascript
type : OdsPageBackgroundType;
```
### color {#color--}
Gets and sets the color of background.
```javascript
color : Color;
```
### graphicType {#graphicType--}
Gets and sets the page background graphic type.
```javascript
graphicType : OdsPageBackgroundGraphicType;
```
### graphicPositionType {#graphicPositionType--}
Gets and set the background graphic position.
```javascript
graphicPositionType : OdsPageBackgroundGraphicPositionType;
```
### isLink {#isLink--}
Readonly. Indicates whether it's a linked graphic.
```javascript
isLink : boolean;
```
### linkedGraphic {#linkedGraphic--}
Gets and sets the linked graphic path.
```javascript
linkedGraphic : string;
```
### graphicData {#graphicData--}
Gets and sets the graphic data.
```javascript
graphicData : Uint8Array;
```
### getType() {#getType--}
```javascript
getType() : OdsPageBackgroundType;
```
**Returns**
[OdsPageBackgroundType](../odspagebackgroundtype/)
### setType(OdsPageBackgroundType) {#setType-odspagebackgroundtype-}
```javascript
setType(value: OdsPageBackgroundType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OdsPageBackgroundType](../odspagebackgroundtype/) | The value to set. |
### getColor() {#getColor--}
```javascript
getColor() : Color;
```
**Returns**
[Color](../color/)
### setColor(Color) {#setColor-color-}
```javascript
setColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getGraphicType() {#getGraphicType--}
```javascript
getGraphicType() : OdsPageBackgroundGraphicType;
```
**Returns**
[OdsPageBackgroundGraphicType](../odspagebackgroundgraphictype/)
### setGraphicType(OdsPageBackgroundGraphicType) {#setGraphicType-odspagebackgroundgraphictype-}
```javascript
setGraphicType(value: OdsPageBackgroundGraphicType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OdsPageBackgroundGraphicType](../odspagebackgroundgraphictype/) | The value to set. |
### getGraphicPositionType() {#getGraphicPositionType--}
```javascript
getGraphicPositionType() : OdsPageBackgroundGraphicPositionType;
```
**Returns**
[OdsPageBackgroundGraphicPositionType](../odspagebackgroundgraphicpositiontype/)
### setGraphicPositionType(OdsPageBackgroundGraphicPositionType) {#setGraphicPositionType-odspagebackgroundgraphicpositiontype-}
```javascript
setGraphicPositionType(value: OdsPageBackgroundGraphicPositionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OdsPageBackgroundGraphicPositionType](../odspagebackgroundgraphicpositiontype/) | The value to set. |
### isLink() {#isLink--}
```javascript
isLink() : boolean;
```
### getLinkedGraphic() {#getLinkedGraphic--}
```javascript
getLinkedGraphic() : string;
```
### setLinkedGraphic(string) {#setLinkedGraphic-string-}
```javascript
setLinkedGraphic(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getGraphicData() {#getGraphicData--}
```javascript
getGraphicData() : Uint8Array;
```
### setGraphicData(Uint8Array) {#setGraphicData-uint8array-}
```javascript
setGraphicData(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
