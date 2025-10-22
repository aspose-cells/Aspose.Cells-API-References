##CustomDocumentPropertyCollection
A collection of custom document properties.
## CustomDocumentPropertyCollection class
A collection of custom document properties.
```javascript
class CustomDocumentPropertyCollection extends DocumentPropertyCollection;
```
### Remarks
Each [DocumentProperty](../documentproperty/) object represents a custom property of a container document.
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
//Instantiate a Workbook object
var workbook = new Workbook("input/CustomProperties.xlsx");
//Retrieve a list of all custom document properties of the Excel file
var customProperties = workbook.worksheets.customDocumentProperties;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(DocumentPropertyCollection)](#constructor-documentpropertycollection-)| Constructs from a parent object convertible to this. |
## Methods
| Method | Description |
| --- | --- |
| [add(string, string)](#add-string-string-)| Creates a new custom document property of the <b>PropertyType.String</b> data type. |
| [add(string, number)](#add-string-number-)| Creates a new custom document property of the <b>PropertyType.Number</b> data type. |
| [add(string, Date)](#add-string-date-)| Creates a new custom document property of the <b>PropertyType.DateTime</b> data type. |
| [add(string, boolean)](#add-string-boolean-)| Creates a new custom document property of the <b>PropertyType.Boolean</b> data type. |
| [add(string, number)](#add-string-number-)| Creates a new custom document property of the <b>PropertyType.Float</b> data type. |
| [addLinkToContent(string, string)](#addLinkToContent-string-string-)| Creates a new custom document property which links to content. |
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--)| Updates values of all custom properties that are linked to content(use cell value of linked range to update value of custom property). |
| [updateLinkedRange()](#updateLinkedRange--)| Updates all ranges that are linked to custom properties(use the value of custom document property to update cell value of linked range). |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [get(number)](#get-number-)| Returns a [DocumentProperty](../documentproperty/) object by index. |
| [contains(string)](#contains-string-)| Returns true if a property with the specified name exists in the collection. |
| [indexOf(string)](#indexOf-string-)| Gets the index of a property by name. |
| [remove(string)](#remove-string-)| Removes a property with the specified name from the collection. |
| [removeAt(number)](#removeAt-number-)| Removes a property at the specified index. |
| [get(string)](#get-string-)| Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
### constructor(DocumentPropertyCollection) {#constructor-documentpropertycollection-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: DocumentPropertyCollection);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | DocumentPropertyCollection | The parent object. |
### add(string, string) {#add-string-string-}
Creates a new custom document property of the <b>PropertyType.String</b> data type.
```javascript
add(name: string, value: string) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property. |
| value | string | The value of the property. |
**Returns**
The newly created property object.
### add(string, number) {#add-string-number-}
Creates a new custom document property of the <b>PropertyType.Number</b> data type.
```javascript
add(name: string, value: number) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property. |
| value | number | The value of the property. |
**Returns**
The newly created property object.
### add(string, Date) {#add-string-date-}
Creates a new custom document property of the <b>PropertyType.DateTime</b> data type.
```javascript
add(name: string, value: Date) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property. |
| value | Date | The value of the property. |
**Returns**
The newly created property object.
### add(string, boolean) {#add-string-boolean-}
Creates a new custom document property of the <b>PropertyType.Boolean</b> data type.
```javascript
add(name: string, value: boolean) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property. |
| value | boolean | The value of the property. |
**Returns**
The newly created property object.
### add(string, number) {#add-string-number-}
Creates a new custom document property of the <b>PropertyType.Float</b> data type.
```javascript
add(name: string, value: number) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property. |
| value | number | The value of the property. |
**Returns**
The newly created property object.
### addLinkToContent(string, string) {#addLinkToContent-string-string-}
Creates a new custom document property which links to content.
```javascript
addLinkToContent(name: string, source: string) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property. |
| source | string | The source of the property. It should be the name of named range. |
**Returns**
The newly created property object.
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
Updates values of all custom properties that are linked to content(use cell value of linked range to update value of custom property).
```javascript
updateLinkedPropertyValue() : void;
```
### updateLinkedRange() {#updateLinkedRange--}
Updates all ranges that are linked to custom properties(use the value of custom document property to update cell value of linked range).
```javascript
updateLinkedRange() : void;
```
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
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
