##DocumentProperty
Represents a custom or builtin document property.
## DocumentProperty class
Represents a custom or built-in document property.
```javascript
class DocumentProperty;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
//Instantiate a Workbook object
var workbook = new Workbook("input/CustomProperties.xlsx");
//Retrieve a list of all custom document properties of the Excel file
var customProperties = workbook.worksheets.customDocumentProperties;
//Accessng a custom document property by using the property index
var customProperty1 = customProperties.get(3);
//Accessng a custom document property by using the property name
var customProperty2 = customProperties.get("Owner");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Readonly. Returns the name of the property. |
| [value](#value--)| Object | Gets or sets the value of the property. |
| [isLinkedToContent](#isLinkedToContent--)| boolean | Readonly. Indicates whether this property is linked to content |
| [source](#source--)| string | Readonly. The linked content source. |
| [type](#type--)| PropertyType | Readonly. Gets the data type of the property. |
| [isGeneratedName](#isGeneratedName--)| boolean | Readonly. Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
## Methods
| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Returns the name of the property. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets or sets the value of the property. |
| [setValue(Object)](#setValue-object-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets or sets the value of the property. |
| [isLinkedToContent()](#isLinkedToContent--)| <b>@deprecated.</b> Please use the 'isLinkedToContent' property instead. Indicates whether this property is linked to content |
| [getSource()](#getSource--)| <b>@deprecated.</b> Please use the 'source' property instead. The linked content source. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the data type of the property. |
| [isGeneratedName()](#isGeneratedName--)| <b>@deprecated.</b> Please use the 'isGeneratedName' property instead. Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
| [toInt()](#toInt--)| Returns the property value as integer. |
| [toDouble()](#toDouble--)| Returns the property value as double. |
| [toDateTime()](#toDateTime--)| Returns the property value as DateTime in local timezone. |
| [toBool()](#toBool--)| Returns the property value as bool. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toString()](#toString--)| Returns the property value as a string. |
### name {#name--}
Readonly. Returns the name of the property.
```javascript
name : string;
```
### value {#value--}
Gets or sets the value of the property.
```javascript
value : Object;
```
### isLinkedToContent {#isLinkedToContent--}
Readonly. Indicates whether this property is linked to content
```javascript
isLinkedToContent : boolean;
```
### source {#source--}
Readonly. The linked content source.
```javascript
source : string;
```
### type {#type--}
Readonly. Gets the data type of the property.
```javascript
type : PropertyType;
```
### isGeneratedName {#isGeneratedName--}
Readonly. Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API.
```javascript
isGeneratedName : boolean;
```
### getName() {#getName--}
```javascript
getName() : string;
```
### getValue() {#getValue--}
```javascript
getValue() : Object;
```
### setValue(Object) {#setValue-object-}
```javascript
setValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
### isLinkedToContent() {#isLinkedToContent--}
```javascript
isLinkedToContent() : boolean;
```
### getSource() {#getSource--}
```javascript
getSource() : string;
```
### getType() {#getType--}
```javascript
getType() : PropertyType;
```
**Returns**
[PropertyType](../propertytype/)
### isGeneratedName() {#isGeneratedName--}
```javascript
isGeneratedName() : boolean;
```
### toInt() {#toInt--}
Returns the property value as integer.
```javascript
toInt() : number;
```
**Remarks**
Throws an exception if the property type is not PropertyType.Number.
### toDouble() {#toDouble--}
Returns the property value as double.
```javascript
toDouble() : number;
```
**Remarks**
Throws an exception if the property type is not PropertyType.Float.
### toDateTime() {#toDateTime--}
Returns the property value as DateTime in local timezone.
```javascript
toDateTime() : Date;
```
**Remarks**
Throws an exception if the property type is not PropertyType.Date.
### toBool() {#toBool--}
Returns the property value as bool.
```javascript
toBool() : boolean;
```
**Remarks**
Throws an exception if the property type is not PropertyType.Boolean.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### toString() {#toString--}
Returns the property value as a string.
```javascript
toString() : string;
```
**Remarks**
Converts a number property using Object.ToString(). Converts a boolean property into "Y" or "N". Converts a date property into a short date string.
