##QueryTable
Represents QueryTable information.
## QueryTable class
Represents QueryTable information.
```javascript
class QueryTable;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [connectionId](#connectionId--)| number | Readonly. Gets the connection id of the query table. |
| [externalConnection](#externalConnection--)| ExternalConnection | Readonly. Gets the relate external connection. |
| [name](#name--)| string | Readonly. Gets the name of querytable. |
| [resultRange](#resultRange--)| Range | Readonly. Gets the range of the result. |
| [preserveFormatting](#preserveFormatting--)| boolean | Returns or sets the PreserveFormatting of the object. |
| [adjustColumnWidth](#adjustColumnWidth--)| boolean | Returns or sets the AdjustColumnWidth of the object. |
## Methods
| Method | Description |
| --- | --- |
| [getConnectionId()](#getConnectionId--)| <b>@deprecated.</b> Please use the 'connectionId' property instead. Gets the connection id of the query table. |
| [getExternalConnection()](#getExternalConnection--)| <b>@deprecated.</b> Please use the 'externalConnection' property instead. Gets the relate external connection. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of querytable. |
| [getResultRange()](#getResultRange--)| <b>@deprecated.</b> Please use the 'resultRange' property instead. Gets the range of the result. |
| [getPreserveFormatting()](#getPreserveFormatting--)| <b>@deprecated.</b> Please use the 'preserveFormatting' property instead. Returns or sets the PreserveFormatting of the object. |
| [setPreserveFormatting(boolean)](#setPreserveFormatting-boolean-)| <b>@deprecated.</b> Please use the 'preserveFormatting' property instead. Returns or sets the PreserveFormatting of the object. |
| [getAdjustColumnWidth()](#getAdjustColumnWidth--)| <b>@deprecated.</b> Please use the 'adjustColumnWidth' property instead. Returns or sets the AdjustColumnWidth of the object. |
| [setAdjustColumnWidth(boolean)](#setAdjustColumnWidth-boolean-)| <b>@deprecated.</b> Please use the 'adjustColumnWidth' property instead. Returns or sets the AdjustColumnWidth of the object. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### connectionId {#connectionId--}
Readonly. Gets the connection id of the query table.
```javascript
connectionId : number;
```
### externalConnection {#externalConnection--}
Readonly. Gets the relate external connection.
```javascript
externalConnection : ExternalConnection;
```
### name {#name--}
Readonly. Gets the name of querytable.
```javascript
name : string;
```
### resultRange {#resultRange--}
Readonly. Gets the range of the result.
```javascript
resultRange : Range;
```
### preserveFormatting {#preserveFormatting--}
Returns or sets the PreserveFormatting of the object.
```javascript
preserveFormatting : boolean;
```
### adjustColumnWidth {#adjustColumnWidth--}
Returns or sets the AdjustColumnWidth of the object.
```javascript
adjustColumnWidth : boolean;
```
### getConnectionId() {#getConnectionId--}
```javascript
getConnectionId() : number;
```
### getExternalConnection() {#getExternalConnection--}
```javascript
getExternalConnection() : ExternalConnection;
```
**Returns**
[ExternalConnection](../externalconnection/)
### getName() {#getName--}
```javascript
getName() : string;
```
### getResultRange() {#getResultRange--}
```javascript
getResultRange() : Range;
```
**Returns**
[Range](../range/)
### getPreserveFormatting() {#getPreserveFormatting--}
```javascript
getPreserveFormatting() : boolean;
```
### setPreserveFormatting(boolean) {#setPreserveFormatting-boolean-}
```javascript
setPreserveFormatting(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAdjustColumnWidth() {#getAdjustColumnWidth--}
```javascript
getAdjustColumnWidth() : boolean;
```
### setAdjustColumnWidth(boolean) {#setAdjustColumnWidth-boolean-}
```javascript
setAdjustColumnWidth(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
