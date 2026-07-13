---
title: CustomFilterCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the custom filters.
type: docs
url: /nodejs-cpp/customfiltercollection/
---

## CustomFilterCollection class

Represents the custom filters.

```javascript
class CustomFilterCollection implements Iterable<CustomFilter>;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructs new instance. |
| [constructor(Object)](#constructor-object-)| Constructs from an Object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [and](#and--)| boolean | Indicates whether the two criteria have an "and" relationship. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the custom filter in the specific index. |
| [getAnd()](#getAnd--)| <b>@deprecated.</b> Please use the 'and' property instead. Indicates whether the two criteria have an "and" relationship. |
| [setAnd(boolean)](#setAnd-boolean-)| <b>@deprecated.</b> Please use the 'and' property instead. Indicates whether the two criteria have an "and" relationship. |
| [custom(FilterOperatorType, Object, boolean, FilterOperatorType, Object)](#custom-filteroperatortype-object-boolean-filteroperatortype-object-)| Filters a list with custom criteria. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toObject()](#toObject--)| Gets the Object. |

## \[Symbol.iterator\](): Iterator\<CustomFilter\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### constructor() {#constructor--}

Constructs new instance.

```javascript
constructor();
```


**Remarks**

NOTE: This member is now obsolete. Instead,please set FilterColumn.FilterType as FilterType.CustomFilters then get FilterColumn.CustomFilters. This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### constructor(Object) {#constructor-object-}

Constructs from an Object convertible to this.

```javascript
constructor(obj: Object);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object. |

### and {#and--}

Indicates whether the two criteria have an "and" relationship.

```javascript
and : boolean;
```


### get(number) {#get-number-}

Gets the custom filter in the specific index.

```javascript
get(index: number) : CustomFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[CustomFilter](../customfilter/)

### getAnd() {#getAnd--}

<b>@deprecated.</b> Please use the 'and' property instead. Indicates whether the two criteria have an "and" relationship.

```javascript
getAnd() : boolean;
```


### setAnd(boolean) {#setAnd-boolean-}

<b>@deprecated.</b> Please use the 'and' property instead. Indicates whether the two criteria have an "and" relationship.

```javascript
setAnd(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### custom(FilterOperatorType, Object, boolean, FilterOperatorType, Object) {#custom-filteroperatortype-object-boolean-filteroperatortype-object-}

Filters a list with custom criteria.

```javascript
custom(operatorType1: FilterOperatorType, criteria1: Object, isAnd: boolean, operatorType2: FilterOperatorType, criteria2: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| operatorType1 | [FilterOperatorType](../filteroperatortype/) |  |
| criteria1 | Object |  |
| isAnd | boolean |  |
| operatorType2 | [FilterOperatorType](../filteroperatortype/) |  |
| criteria2 | Object |  |

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


### toObject() {#toObject--}

Gets the Object.

```javascript
toObject() : Object;
```



