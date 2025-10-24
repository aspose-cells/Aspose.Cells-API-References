##Top10
Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket as specified.
## Top10 class
Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.
```javascript
class Top10;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isPercent](#isPercent--)| boolean | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [isBottom](#isBottom--)| boolean | Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [rank](#rank--)| number | Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
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
