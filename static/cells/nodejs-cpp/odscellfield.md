##OdsCellField
Represents the cell field of ods.
## OdsCellField class
Represents the cell field of ods.
```javascript
class OdsCellField;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [customFormat](#customFormat--)| string | Represents the custom format of the field's value. |
| [fieldType](#fieldType--)| OdsCellFieldType | Gets and sets the type of the field. |
| [row](#row--)| number | Get and sets the row index of the cell. |
| [column](#column--)| number | Get and sets the column index of the cell. |
## Methods
| Method | Description |
| --- | --- |
| [getCustomFormat()](#getCustomFormat--)| <b>@deprecated.</b> Please use the 'customFormat' property instead. Represents the custom format of the field's value. |
| [setCustomFormat(string)](#setCustomFormat-string-)| <b>@deprecated.</b> Please use the 'customFormat' property instead. Represents the custom format of the field's value. |
| [getFieldType()](#getFieldType--)| <b>@deprecated.</b> Please use the 'fieldType' property instead. Gets and sets the type of the field. |
| [setFieldType(OdsCellFieldType)](#setFieldType-odscellfieldtype-)| <b>@deprecated.</b> Please use the 'fieldType' property instead. Gets and sets the type of the field. |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Get and sets the row index of the cell. |
| [setRow(number)](#setRow-number-)| <b>@deprecated.</b> Please use the 'row' property instead. Get and sets the row index of the cell. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Get and sets the column index of the cell. |
| [setColumn(number)](#setColumn-number-)| <b>@deprecated.</b> Please use the 'column' property instead. Get and sets the column index of the cell. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### customFormat {#customFormat--}
Represents the custom format of the field's value.
```javascript
customFormat : string;
```
### fieldType {#fieldType--}
Gets and sets the type of the field.
```javascript
fieldType : OdsCellFieldType;
```
### row {#row--}
Get and sets the row index of the cell.
```javascript
row : number;
```
### column {#column--}
Get and sets the column index of the cell.
```javascript
column : number;
```
### getCustomFormat() {#getCustomFormat--}
```javascript
getCustomFormat() : string;
```
### setCustomFormat(string) {#setCustomFormat-string-}
```javascript
setCustomFormat(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getFieldType() {#getFieldType--}
```javascript
getFieldType() : OdsCellFieldType;
```
**Returns**
[OdsCellFieldType](../odscellfieldtype/)
### setFieldType(OdsCellFieldType) {#setFieldType-odscellfieldtype-}
```javascript
setFieldType(value: OdsCellFieldType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OdsCellFieldType](../odscellfieldtype/) | The value to set. |
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### setRow(number) {#setRow-number-}
```javascript
setRow(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### setColumn(number) {#setColumn-number-}
```javascript
setColumn(value: number) : void;
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
