##VbaModuleCollection
Represents the list of VbaModule..vbamodule
## VbaModuleCollection class
Represents the list of [VbaModule](../vbamodule/)
```javascript
class VbaModuleCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [VbaModule](../vbamodule/) in the list by the index. |
| [get(string)](#get-string-)| Gets [VbaModule](../vbamodule/) in the list by the name. |
| [addDesignerStorage(string, Uint8Array)](#addDesignerStorage-string-uint8array-)|  |
| [getDesignerStorage(string)](#getDesignerStorage-string-)| Represents the data of Designer. |
| [add(Worksheet)](#add-worksheet-)| Adds module for a worksheet. |
| [add(VbaModuleType, string)](#add-vbamoduletype-string-)| Adds module. |
| [addUserForm(string, string, Uint8Array)](#addUserForm-string-string-uint8array-)| Inser user form into VBA Project. |
| [remove(Worksheet)](#remove-worksheet-)| Removes module for a worksheet. |
| [remove(string)](#remove-string-)| Remove the module by the name |
### get(number) {#get-number-}
Gets [VbaModule](../vbamodule/) in the list by the index.
```javascript
get(index: number) : VbaModule;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[VbaModule](../vbamodule/)
### get(string) {#get-string-}
Gets [VbaModule](../vbamodule/) in the list by the name.
```javascript
get(name: string) : VbaModule;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of module. |
**Returns**
[VbaModule](../vbamodule/)
### addDesignerStorage(string, Uint8Array) {#addDesignerStorage-string-uint8array-}
```javascript
addDesignerStorage(name: string, data: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |
| data | number[] |  |
### getDesignerStorage(string) {#getDesignerStorage-string-}
Represents the data of Designer.
```javascript
getDesignerStorage(name: string) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |
**Remarks**
We do not support to parse them. Just only for copying.
### add(Worksheet) {#add-worksheet-}
Adds module for a worksheet.
```javascript
add(sheet: Worksheet) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../worksheet/) | The worksheet |
### add(VbaModuleType, string) {#add-vbamoduletype-string-}
Adds module.
```javascript
add(type: VbaModuleType, name: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [VbaModuleType](../vbamoduletype/) | The type of module. |
| name | string | The name of module. |
### addUserForm(string, string, Uint8Array) {#addUserForm-string-string-uint8array-}
Inser user form into VBA Project.
```javascript
addUserForm(name: string, codes: string, designerStorage: Uint8Array) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of user form |
| codes | string | The codes for the user form |
| designerStorage | number[] | the designer setting about the user form |
### remove(Worksheet) {#remove-worksheet-}
Removes module for a worksheet.
```javascript
remove(sheet: Worksheet) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../worksheet/) | The worksheet |
### remove(string) {#remove-string-}
Remove the module by the name
```javascript
remove(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |
