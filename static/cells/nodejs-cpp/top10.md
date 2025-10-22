##Top10
Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket as specified.
## Top10 class
Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.
```javascript
class Top10;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isPercent](#isPercent--)| boolean | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [isBottom](#isBottom--)| boolean | Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [rank](#rank--)| number | Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
## Methods
| Method | Description |
| --- | --- |
| [isPercent()](#isPercent--)| <b>@deprecated.</b> Please use the 'isPercent' property instead. Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [setIsPercent(boolean)](#setIsPercent-boolean-)| <b>@deprecated.</b> Please use the 'isPercent' property instead. Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [isBottom()](#isBottom--)| <b>@deprecated.</b> Please use the 'isBottom' property instead. Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [setIsBottom(boolean)](#setIsBottom-boolean-)| <b>@deprecated.</b> Please use the 'isBottom' property instead. Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [getRank()](#getRank--)| <b>@deprecated.</b> Please use the 'rank' property instead. Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
| [setRank(number)](#setRank-number-)| <b>@deprecated.</b> Please use the 'rank' property instead. Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### isPercent {#isPercent--}
Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false.
```javascript
isPercent : boolean;
```
### isBottom {#isBottom--}
Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false.
```javascript
isBottom : boolean;
```
### rank {#rank--}
Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10.
```javascript
rank : number;
```
### isPercent() {#isPercent--}
```javascript
isPercent() : boolean;
```
### setIsPercent(boolean) {#setIsPercent-boolean-}
```javascript
setIsPercent(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isBottom() {#isBottom--}
```javascript
isBottom() : boolean;
```
### setIsBottom(boolean) {#setIsBottom-boolean-}
```javascript
setIsBottom(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRank() {#getRank--}
```javascript
getRank() : number;
```
### setRank(number) {#setRank-number-}
```javascript
setRank(value: number) : void;
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
