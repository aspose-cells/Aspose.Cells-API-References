##XmlMapCollection
A collection of XmlMap..xmlmap objects that represent XmlMap information.
## XmlMapCollection class
A collection of [XmlMap](../xmlmap/) objects that represent XmlMap information.
```javascript
class XmlMapCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the xml map by the specific index. |
| [add(string)](#add-string-)| Add a [XmlMap](../xmlmap/) by the url/path of a xml/xsd file. |
| [clear()](#clear--)| Removes all XmlMaps. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the xml map by the specific index.
```javascript
get(index: number) : XmlMap;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The xml map
### add(string) {#add-string-}
Add a [XmlMap](../xmlmap/) by the url/path of a xml/xsd file.
```javascript
add(url: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| url | string | url/path of a xml/xsd file. |
**Returns**
[XmlMap](../xmlmap/) object index.
### clear() {#clear--}
Removes all XmlMaps.
```javascript
clear() : void;
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
