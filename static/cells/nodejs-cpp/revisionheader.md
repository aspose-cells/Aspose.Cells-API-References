##RevisionHeader
Represents a list of specific changes that have taken place for this workbook.
## RevisionHeader class
Represents a list of specific changes that have taken place for this workbook.
```javascript
class RevisionHeader;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [savedTime](#savedTime--)| Date | Gets and sets rhe date and time when this set of revisions was saved. |
| [userName](#userName--)| string | Gets and sets the name of the user making the revision. |
## Methods
| Method | Description |
| --- | --- |
| [getSavedTime()](#getSavedTime--)| <b>@deprecated.</b> Please use the 'savedTime' property instead. Gets and sets rhe date and time when this set of revisions was saved. |
| [setSavedTime(Date)](#setSavedTime-date-)| <b>@deprecated.</b> Please use the 'savedTime' property instead. Gets and sets rhe date and time when this set of revisions was saved. |
| [get_UserName()](#get_UserName--)| <b>@deprecated.</b> Please use the 'userName' property instead. Gets and sets the name of the user making the revision. |
| [setUserName(string)](#setUserName-string-)| <b>@deprecated.</b> Please use the 'userName' property instead. Gets and sets the name of the user making the revision. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### savedTime {#savedTime--}
Gets and sets rhe date and time when this set of revisions was saved.
```javascript
savedTime : Date;
```
### userName {#userName--}
Gets and sets the name of the user making the revision.
```javascript
userName : string;
```
### getSavedTime() {#getSavedTime--}
```javascript
getSavedTime() : Date;
```
### setSavedTime(Date) {#setSavedTime-date-}
```javascript
setSavedTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
### get_UserName() {#get_UserName--}
```javascript
get_UserName() : string;
```
### setUserName(string) {#setUserName-string-}
```javascript
setUserName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
