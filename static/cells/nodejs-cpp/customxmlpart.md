##CustomXmlPart
Represents a Custom XML Data Storage Part custom XML data within a package.
## CustomXmlPart class
Represents a Custom XML Data Storage Part (custom XML data within a package).
```javascript
class CustomXmlPart;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [data](#data--)| Uint8Array | Gets or sets the XML content of this Custom XML Data Storage Part. |
| [schemaData](#schemaData--)| Uint8Array | Gets or sets the XML content of this Custom XML Schema Data Storage Part. |
| [iD](#iD--)| string | Gets and sets the id of the custom xml part. |
## Methods
| Method | Description |
| --- | --- |
| [getData()](#getData--)| <b>@deprecated.</b> Please use the 'data' property instead. Gets or sets the XML content of this Custom XML Data Storage Part. |
| [setData(Uint8Array)](#setData-uint8array-)| <b>@deprecated.</b> Please use the 'data' property instead. Gets or sets the XML content of this Custom XML Data Storage Part. |
| [getSchemaData()](#getSchemaData--)| <b>@deprecated.</b> Please use the 'schemaData' property instead. Gets or sets the XML content of this Custom XML Schema Data Storage Part. |
| [setSchemaData(Uint8Array)](#setSchemaData-uint8array-)| <b>@deprecated.</b> Please use the 'schemaData' property instead. Gets or sets the XML content of this Custom XML Schema Data Storage Part. |
| [getID()](#getID--)| <b>@deprecated.</b> Please use the 'iD' property instead. Gets and sets the id of the custom xml part. |
| [setID(string)](#setID-string-)| <b>@deprecated.</b> Please use the 'iD' property instead. Gets and sets the id of the custom xml part. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### data {#data--}
Gets or sets the XML content of this Custom XML Data Storage Part.
```javascript
data : Uint8Array;
```
### schemaData {#schemaData--}
Gets or sets the XML content of this Custom XML Schema Data Storage Part.
```javascript
schemaData : Uint8Array;
```
### iD {#iD--}
Gets and sets the id of the custom xml part.
```javascript
iD : string;
```
### getData() {#getData--}
```javascript
getData() : Uint8Array;
```
### setData(Uint8Array) {#setData-uint8array-}
```javascript
setData(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### getSchemaData() {#getSchemaData--}
```javascript
getSchemaData() : Uint8Array;
```
### setSchemaData(Uint8Array) {#setSchemaData-uint8array-}
```javascript
setSchemaData(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### getID() {#getID--}
```javascript
getID() : string;
```
### setID(string) {#setID-string-}
```javascript
setID(value: string) : void;
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
