##SlicerCacheItemCollection
Represent the collection of SlicerCacheItem
## SlicerCacheItemCollection class
Represent the collection of SlicerCacheItem
```javascript
class SlicerCacheItemCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of the SlicerCacheItem. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the SlicerCacheItem object by index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the count of the SlicerCacheItem. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### count {#count--}
Readonly. Gets the count of the SlicerCacheItem.
```javascript
count : number;
```
### get(number) {#get-number-}
Gets the SlicerCacheItem object by index.
```javascript
get(index: number) : SlicerCacheItem;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
[SlicerCacheItem](../slicercacheitem/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
