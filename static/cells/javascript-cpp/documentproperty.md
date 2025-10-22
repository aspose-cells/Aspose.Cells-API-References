##DocumentProperty
Represents a custom or builtin document property.
## DocumentProperty class
Represents a custom or built-in document property.
```javascript
class DocumentProperty;
```
### Example
```javascript
const { Workbook } = AsposeCells;
//Instantiate a Workbook object
var workbook = new Workbook(data);
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
| [value](#value--)| VObject | Gets or sets the value of the property. |
| [isLinkedToContent](#isLinkedToContent--)| boolean | Readonly. Indicates whether this property is linked to content |
| [source](#source--)| string | Readonly. The linked content source. |
| [type](#type--)| PropertyType | Readonly. Gets the data type of the property. |
| [isGeneratedName](#isGeneratedName--)| boolean | Readonly. Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
## Methods
| Method | Description |
| --- | --- |
| [toInt()](#toInt--)| Returns the property value as integer. |
| [toDouble()](#toDouble--)| Returns the property value as double. |
| [toDateTime()](#toDateTime--)| Returns the property value as DateTime in local timezone. |
| [toBool()](#toBool--)| Returns the property value as bool. |
| [toString()](#toString--)| Returns the property value as a string. |
### name {#name--}
Readonly. Returns the name of the property.
```javascript
name : string;
```
### value {#value--}
Gets or sets the value of the property.
```javascript
value : VObject;
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
### toString() {#toString--}
Returns the property value as a string.
```javascript
toString() : string;
```
**Remarks**
Converts a number property using Object.ToString(). Converts a boolean property into "Y" or "N". Converts a date property into a short date string.
