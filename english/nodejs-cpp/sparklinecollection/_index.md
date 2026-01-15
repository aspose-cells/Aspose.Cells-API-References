---
title: SparklineCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of Sparkline..sparkline objects.
type: docs
url: /nodejs-cpp/sparklinecollection/
---

## SparklineCollection class

Encapsulates a collection of [Sparkline](../sparkline/) objects.

```javascript
class SparklineCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Sparkline](../sparkline/) element at the specified index. |
| [add(string, number, number)](#add-string-number-number-)| Add a sparkline. |
| [remove(Object)](#remove-object-)| Removes the sparkline |
| [removeSparkline(Sparkline)](#removeSparkline-sparkline-)| Removes the sparkline |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the [Sparkline](../sparkline/) element at the specified index.

```javascript
get(index: number) : Sparkline;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### add(string, number, number) {#add-string-number-number-}

Add a sparkline.

```javascript
add(dataRange: string, row: number, column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | string | Specifies the new data range of the sparkline. |
| row | number | The row index of the location. |
| column | number | The column index of the location. |

### remove(Object) {#remove-object-}

Removes the sparkline

```javascript
remove(o: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | Object |  |

**Remarks**

NOTE: This member is now obsolete. Instead, please use RemoveSparkline() method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### removeSparkline(Sparkline) {#removeSparkline-sparkline-}

Removes the sparkline

```javascript
removeSparkline(o: Sparkline) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | [Sparkline](../sparkline/) |  |

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



