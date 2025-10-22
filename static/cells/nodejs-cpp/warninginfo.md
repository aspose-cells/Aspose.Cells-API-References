##WarningInfo
Warning info
## WarningInfo class
Warning info
```javascript
class WarningInfo;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| ExceptionType | Readonly. Get warning type. |
| [description](#description--)| string | Readonly. Get description of warning info. |
| [errorObject](#errorObject--)| Object | Readonly. The error object. |
| [correctedObject](#correctedObject--)| Object | Gets and sets the corrected object. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Get warning type. |
| [getDescription()](#getDescription--)| <b>@deprecated.</b> Please use the 'description' property instead. Get description of warning info. |
| [getErrorObject()](#getErrorObject--)| <b>@deprecated.</b> Please use the 'errorObject' property instead. The error object. |
| [getCorrectedObject()](#getCorrectedObject--)| <b>@deprecated.</b> Please use the 'correctedObject' property instead. Gets and sets the corrected object. |
| [setCorrectedObject(Object)](#setCorrectedObject-object-)| <b>@deprecated.</b> Please use the 'correctedObject' property instead. Gets and sets the corrected object. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### type {#type--}
Readonly. Get warning type.
```javascript
type : ExceptionType;
```
### description {#description--}
Readonly. Get description of warning info.
```javascript
description : string;
```
### errorObject {#errorObject--}
Readonly. The error object.
```javascript
errorObject : Object;
```
### correctedObject {#correctedObject--}
Gets and sets the corrected object.
```javascript
correctedObject : Object;
```
### getType() {#getType--}
```javascript
getType() : ExceptionType;
```
**Returns**
[ExceptionType](../exceptiontype/)
### getDescription() {#getDescription--}
```javascript
getDescription() : string;
```
### getErrorObject() {#getErrorObject--}
```javascript
getErrorObject() : Object;
```
### getCorrectedObject() {#getCorrectedObject--}
```javascript
getCorrectedObject() : Object;
```
### setCorrectedObject(Object) {#setCorrectedObject-object-}
```javascript
setCorrectedObject(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
