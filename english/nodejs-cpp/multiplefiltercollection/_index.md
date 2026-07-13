---
title: MultipleFilterCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the multiple filter collection.
type: docs
url: /nodejs-cpp/multiplefiltercollection/
---

## MultipleFilterCollection class

Represents the multiple filter collection.

```javascript
class MultipleFilterCollection implements Iterable<FilterValue>;
```

### Remarks
NOTE: This class is now obsolete. Instead,please use [FilterValueCollection](../filtervaluecollection/) instead. This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructs one new instance. |
| [constructor(Object)](#constructor-object-)| Constructs from an Object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of the filter values. |
| [matchBlank](#matchBlank--)| boolean | Indicates whether to filter by blank. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [DateTimeGroupItem](../datetimegroupitem/) or a string value. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the count of the filter values. |
| [getMatchBlank()](#getMatchBlank--)| <b>@deprecated.</b> Please use the 'matchBlank' property instead. Indicates whether to filter by blank. |
| [setMatchBlank(boolean)](#setMatchBlank-boolean-)| <b>@deprecated.</b> Please use the 'matchBlank' property instead. Indicates whether to filter by blank. |
| [add(string)](#add-string-)| Adds a label filter criteria. |
| [add(DateTimeGroupingType, number, number, number)](#add-datetimegroupingtype-number-number-number-)| Adds a date filter criteria value. |
| [add(DateTimeGroupingType, number, number, number, number, number, number)](#add-datetimegroupingtype-number-number-number-number-number-number-)| Adds a date time filter criteria value. |
| [getEnumerator()](#getEnumerator--)| Get the enumerator for filter value, |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toObject()](#toObject--)| Gets the Object. |

## \[Symbol.iterator\](): Iterator\<FilterValue\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### constructor() {#constructor--}

Constructs one new instance.

```javascript
constructor();
```


**Remarks**

NOTE: This member is now obsolete. Instead,please set FilterColumn.FilterType as FilterType.MultipleFilters then get FilterColumn.MultipleFilters. This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### constructor(Object) {#constructor-object-}

Constructs from an Object convertible to this.

```javascript
constructor(obj: Object);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object. |

### count {#count--}

Readonly. Gets the count of the filter values.

```javascript
count : number;
```


### matchBlank {#matchBlank--}

Indicates whether to filter by blank.

```javascript
matchBlank : boolean;
```


### get(number) {#get-number-}

Gets [DateTimeGroupItem](../datetimegroupitem/) or a string value.

```javascript
get(index: number) : Object;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the count of the filter values.

```javascript
getCount() : number;
```


### getMatchBlank() {#getMatchBlank--}

<b>@deprecated.</b> Please use the 'matchBlank' property instead. Indicates whether to filter by blank.

```javascript
getMatchBlank() : boolean;
```


### setMatchBlank(boolean) {#setMatchBlank-boolean-}

<b>@deprecated.</b> Please use the 'matchBlank' property instead. Indicates whether to filter by blank.

```javascript
setMatchBlank(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### add(string) {#add-string-}

Adds a label filter criteria.

```javascript
add(filter: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filter | string | The filter data. |

### add(DateTimeGroupingType, number, number, number) {#add-datetimegroupingtype-number-number-number-}

Adds a date filter criteria value.

```javascript
add(type: DateTimeGroupingType, year: number, month: number, day: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [DateTimeGroupingType](../datetimegroupingtype/) | The type of date filter. |
| year | number | The year. |
| month | number | The month. |
| day | number | The day. |

### add(DateTimeGroupingType, number, number, number, number, number, number) {#add-datetimegroupingtype-number-number-number-number-number-number-}

Adds a date time filter criteria value.

```javascript
add(type: DateTimeGroupingType, year: number, month: number, day: number, hour: number, minute: number, second: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [DateTimeGroupingType](../datetimegroupingtype/) | The type of date filter. |
| year | number | The year. |
| month | number | The month. |
| day | number | The day. |
| hour | number | The hour. |
| minute | number | The minute. |
| second | number | The second. |

### getEnumerator() {#getEnumerator--}

Get the enumerator for filter value,

```javascript
getEnumerator() : FilterValueEnumerator;
```


**Returns**

[FilterValueEnumerator](../filtervalueenumerator/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### toObject() {#toObject--}

Gets the Object.

```javascript
toObject() : Object;
```



