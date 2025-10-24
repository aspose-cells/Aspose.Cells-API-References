##ContentTypePropertyCollection
A collection of ContentTypeProperty..contenttypeproperty objects that represent additional information.
## ContentTypePropertyCollection class
A collection of [ContentTypeProperty](../contenttypeproperty/) objects that represent additional information.
```javascript
class ContentTypePropertyCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the content type property by the specific index. |
| [get(string)](#get-string-)| Gets the content type property by the property name. |
| [add(string, string)](#add-string-string-)| Adds content type property information. |
| [add(string, string, string)](#add-string-string-string-)| Adds content type property information. |
### get(number) {#get-number-}
Gets the content type property by the specific index.
```javascript
get(index: number) : ContentTypeProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The content type property
### get(string) {#get-string-}
Gets the content type property by the property name.
```javascript
get(name: string) : ContentTypeProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The property name. |
**Returns**
The content type property
### add(string, string) {#add-string-string-}
Adds content type property information.
```javascript
add(name: string, value: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the content type property. |
| value | string | The value of the content type property. |
### add(string, string, string) {#add-string-string-string-}
Adds content type property information.
```javascript
add(name: string, value: string, type: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the content type property. |
| value | string | The value of the content type property. |
| type | string | The type of the content type property. |
