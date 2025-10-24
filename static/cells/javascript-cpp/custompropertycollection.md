##CustomPropertyCollection
A collection of CustomProperty..customproperty objects that represent additional information.
## CustomPropertyCollection class
A collection of [CustomProperty](../customproperty/) objects that represent additional information.
```javascript
class CustomPropertyCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the custom property by the specific index. |
| [get(string)](#get-string-)| Gets the custom property by the property name. |
| [add(string, string)](#add-string-string-)| Adds custom property information. |
### get(number) {#get-number-}
Gets the custom property by the specific index.
```javascript
get(index: number) : CustomProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The custom property
### get(string) {#get-string-}
Gets the custom property by the property name.
```javascript
get(name: string) : CustomProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The property name. |
**Returns**
The custom property
### add(string, string) {#add-string-string-}
Adds custom property information.
```javascript
add(name: string, value: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the custom property. |
| value | string | The value of the custom property. |
