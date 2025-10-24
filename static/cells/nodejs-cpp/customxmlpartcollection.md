##CustomXmlPartCollection
Represents a Custom XML Data Storage Part custom XML data within a package.
## CustomXmlPartCollection class
Represents a Custom XML Data Storage Part (custom XML data within a package).
```javascript
class CustomXmlPartCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets an item at the specified index. |
| [add(Uint8Array, Uint8Array)](#add-uint8array-uint8array-)| Adds an item to the collection. |
| [selectByID(string)](#selectByID-string-)| Gets an item by id. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets an item at the specified index.
```javascript
get(index: number) : CustomXmlPart;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[CustomXmlPart](../customxmlpart/)
### add(Uint8Array, Uint8Array) {#add-uint8array-uint8array-}
Adds an item to the collection.
```javascript
add(data: Uint8Array, shemaData: Uint8Array) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | number[] | The XML content of this Custom XML Data Storage Part. |
| shemaData | number[] | The set of XML schemas that are associated with this custom XML part. |
### selectByID(string) {#selectByID-string-}
Gets an item by id.
```javascript
selectByID(id: string) : CustomXmlPart;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| id | string | Contains the GUID for the custom XML part. |
**Returns**
[CustomXmlPart](../customxmlpart/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
