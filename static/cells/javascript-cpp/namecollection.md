##NameCollection
Represents a collection of all the Name..name objects in the spreadsheet.
## NameCollection class
Represents a collection of all the [Name](../name/) objects in the spreadsheet.
```javascript
class NameCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Name](../name/) element at the specified index. |
| [get(string)](#get-string-)| Gets the [Name](../name/) element with the specified name. |
| [add(string)](#add-string-)| Defines a new name. |
| [filter(NameScopeType, number)](#filter-namescopetype-number-)| Gets all defined name by scope. |
| [remove(string[])](#remove-stringarray-)| Remove an array of name |
| [remove(string)](#remove-string-)| Remove the name. |
| [removeAt(number)](#removeAt-number-)| Remove the name at the specific index. |
| [clear()](#clear--)| Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we only set Name.ReferTo as null and hide them. |
| [removeDuplicateNames()](#removeDuplicateNames--)| Remove the duplicate defined names |
| [sort()](#sort--)| Sorts defined names. |
### get(number) {#get-number-}
Gets the [Name](../name/) element at the specified index.
```javascript
get(index: number) : Name;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### get(string) {#get-string-}
Gets the [Name](../name/) element with the specified name.
```javascript
get(text: string) : Name;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | Name text. |
**Returns**
The element with the specified name.
### add(string) {#add-string-}
Defines a new name.
```javascript
add(text: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text to use as the name. |
**Returns**
[Name](../name/) object index.
**Remarks**
Name cannot include spaces and cannot look like cell references.
### filter(NameScopeType, number) {#filter-namescopetype-number-}
Gets all defined name by scope.
```javascript
filter(type: NameScopeType, sheetIndex: number) : Name[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [NameScopeType](../namescopetype/) | The scope type. |
| sheetIndex | number | The sheet index.         /// Only effects when scope type is [NameScopeType.Worksheet](../namescopetype.worksheet/) |
**Returns**
[Name](../name/)[]
### remove(string[]) {#remove-stringarray-}
Remove an array of name
```javascript
remove(names: string[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| names | string[] | The names' text. |
### remove(string) {#remove-string-}
Remove the name.
```javascript
remove(text: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The name text. |
### removeAt(number) {#removeAt-number-}
Remove the name at the specific index.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | index of the Name to be removed. |
**Remarks**
Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred, setting Name.RefersTo as null is better.
### clear() {#clear--}
Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we only set Name.ReferTo as null and hide them.
```javascript
clear() : void;
```
### removeDuplicateNames() {#removeDuplicateNames--}
Remove the duplicate defined names
```javascript
removeDuplicateNames() : void;
```
### sort() {#sort--}
Sorts defined names.
```javascript
sort() : void;
```
**Remarks**
If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving
