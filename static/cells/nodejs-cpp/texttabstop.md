##TextTabStop
Represents tab stop.
## TextTabStop class
Represents tab stop.
```javascript
class TextTabStop;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [tabAlignment](#tabAlignment--)| TextTabAlignmentType | Specifies the alignment that is to be applied to text using this tab stop. |
| [tabPosition](#tabPosition--)| number | Specifies the position of the tab stop relative to the left margin. |
## Methods
| Method | Description |
| --- | --- |
| [getTabAlignment()](#getTabAlignment--)| <b>@deprecated.</b> Please use the 'tabAlignment' property instead. Specifies the alignment that is to be applied to text using this tab stop. |
| [setTabAlignment(TextTabAlignmentType)](#setTabAlignment-texttabalignmenttype-)| <b>@deprecated.</b> Please use the 'tabAlignment' property instead. Specifies the alignment that is to be applied to text using this tab stop. |
| [getTabPosition()](#getTabPosition--)| <b>@deprecated.</b> Please use the 'tabPosition' property instead. Specifies the position of the tab stop relative to the left margin. |
| [setTabPosition(number)](#setTabPosition-number-)| <b>@deprecated.</b> Please use the 'tabPosition' property instead. Specifies the position of the tab stop relative to the left margin. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### tabAlignment {#tabAlignment--}
Specifies the alignment that is to be applied to text using this tab stop.
```javascript
tabAlignment : TextTabAlignmentType;
```
### tabPosition {#tabPosition--}
Specifies the position of the tab stop relative to the left margin.
```javascript
tabPosition : number;
```
### getTabAlignment() {#getTabAlignment--}
```javascript
getTabAlignment() : TextTabAlignmentType;
```
**Returns**
[TextTabAlignmentType](../texttabalignmenttype/)
### setTabAlignment(TextTabAlignmentType) {#setTabAlignment-texttabalignmenttype-}
```javascript
setTabAlignment(value: TextTabAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextTabAlignmentType](../texttabalignmenttype/) | The value to set. |
### getTabPosition() {#getTabPosition--}
```javascript
getTabPosition() : number;
```
### setTabPosition(number) {#setTabPosition-number-}
```javascript
setTabPosition(value: number) : void;
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
