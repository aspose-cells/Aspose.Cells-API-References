##DocumentPropertyCollection
Base class for BuiltInDocumentPropertyCollection..builtindocumentpropertycollection and CustomDocumentPropertyCollection..customdocumentpropertycollection collections.
## DocumentPropertyCollection class
Base class for [BuiltInDocumentPropertyCollection](../builtindocumentpropertycollection/) and [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) collections.
```javascript
class DocumentPropertyCollection;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
//Instantiate a Workbook object by calling its empty constructor
var workbook = new Workbook("input/CustomProperties.xlsx");
//Retrieve a list of all custom document properties of the Excel file
var customProperties = workbook.worksheets.customDocumentProperties;
//Accessng a custom document property by using the property index
var customProperty1 = customProperties.get(3);
//Accessng a custom document property by using the property name
var customProperty2 = customProperties.get("rox_Meta1");
console.log("Custom Properties: " + customProperties.count);
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Returns a [DocumentProperty](../documentproperty/) object by index. |
| [contains(string)](#contains-string-)| Returns true if a property with the specified name exists in the collection. |
| [indexOf(string)](#indexOf-string-)| Gets the index of a property by name. |
| [remove(string)](#remove-string-)| Removes a property with the specified name from the collection. |
| [removeAt(number)](#removeAt-number-)| Removes a property at the specified index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [get(string)](#get-string-)| Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
### get(number) {#get-number-}
Returns a [DocumentProperty](../documentproperty/) object by index.
```javascript
get(index: number) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | Zero-based index of the [DocumentProperty](../documentproperty/) to retrieve. |
**Returns**
[DocumentProperty](../documentproperty/)
### contains(string) {#contains-string-}
Returns true if a property with the specified name exists in the collection.
```javascript
contains(name: string) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |
**Returns**
True if the property exists in the collection; false otherwise.
### indexOf(string) {#indexOf-string-}
Gets the index of a property by name.
```javascript
indexOf(name: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |
**Returns**
The zero based index. Negative value if not found.
### remove(string) {#remove-string-}
Removes a property with the specified name from the collection.
```javascript
remove(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |
### removeAt(number) {#removeAt-number-}
Removes a property at the specified index.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### get(string) {#get-string-}
Returns a [DocumentProperty](../documentproperty/) object by the name of the property.
```javascript
get(name: string) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property to retrieve. |
**Returns**
[DocumentProperty](../documentproperty/)
**Remarks**
Returns null if a property with the specified name is not found.
